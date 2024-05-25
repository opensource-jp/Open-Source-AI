# オープンソースAIの定義
### バージョン 0.0.8

:information_source: 注：この文書は3つの部分から構成されている： この文書の意図を述べた前文、オープンソースAIの定義そのもの、そして法的文書を評価するためのチェックリストである。

:information_source: この文書は、[経済協力開発機構(OECD)](https://legalinstruments.oecd.org/en/instruments/OECD-LEGAL-0449)が採用したAIシステムの定義に従っている。



> AIシステムとは、明示的または暗黙的な目的のために、受け取った入力から物理的または仮想的な環境に影響を与えることができる予測、コンテンツ、推奨、または決定などの出力を生成する方法を推論する機械ベースのシステムである。AIシステムによって、自律性や導入後の適応性のレベルは異なる。

AIシステムの定義の詳細については、[OSIのブログ](https://blog.opensource.org/open-source-ai-establishing-a-common-ground/)をご覧ください。


# 前文

## オープンソースの人工知能(AI)が必要な理由
オープンソースは、ソフトウェア・システムの学習、使用、共有、改善の障壁を取り除けば、誰にでも多大な恩恵がもたらされることを実証してきた。これらの恩恵は、オープンソースの定義に準拠したライセンスを使用した結果もたらされるものです。その恩恵は、自律性、透明性、軋轢が生じない再利用、共同改善に集約される。

AIによるこれらの恩恵は誰もが必要としている。ユーザーが信頼性と透明性のあるAIシステムを構築し、展開できるようにするため、我々には本質的な自由が必要である。

# オープンソースAIとは何か

オープンソースAIとは、以下のような自由を与える条件の下で利用できるAIシステムのことである：

* **使用**：どのような目的であれ、許可を得ることなくシステムを使用すること。
* **研究**：システムがどのように動作するかを研究し、そのコンポーネントを検査すること。
* **改変**：出力を変更することを含め、どのような目的であれシステムを改変すること。
* **共有**：どのような目的であれ、改変の有無に関わらず、他者が使用できるようにシステムを共有すること。

これらの自由を行使するための前提条件は、システムに修正を加えるための好ましい形式へのアクセス権を持っていることである。

## 機械学習システムに改変を加えるための推奨される形式

機械学習のオープンソースAIを改変する好ましい形式には、以下のものが含まれている必要がある：

* **データの情報**：熟練者が同一または類似のデータを使用して実質的に同等のシステムを再作成できるように、システムの学習に使用したデータに関する十分に詳細な情報
  * 例えば、使用されている場合、学習方法方法および技術、使用された学習用データセット、それらのデータセットの出所および範囲と特徴、データの取得方法と選択方法、ラベリングの手順とデータクリーニング方法に関する情報が含まれる。
* **コード**：システムのトレーニングおよび実行に使用されたソースコード
  * 例えば、使用されている場合、データの前処理に使用されたコード、学習と検証およびテストに使用されたコード、トークナイザーやハイパーパラメーター検索コード等のサポートライブラリ、推論コード、モデルアーキテクチャなどが含まれる。
* **モデル**：モデル・パラメータ
  * 例えば、最終的なオプティマイザの状態だけでなく、学習の主要な中間段階からのチェックポイントも含まれる。


# 機械学習システムを評価するためのチェックリスト

このチェックリストは、2024年3月21日に発行された論文[「The Model Openness Framework: Promoting Completeness and Openness for Reproducibility, Transparency and Usability in AI」](https://arxiv.org/abs/2403.13784)に基づいている。

### デフォルトの必須コンポーネントの表

| 必須コンポーネント     |      法的枠組み          |
| ------------------------| ------------------------------ |
| **データの情報** |
|  - 学習の方法論と技術 | OSD準拠のライセンスで利用可能 |
|  - 学習データの範囲と特徴 | OSD準拠のライセンスで利用可能 |
|  - 学習データの出所（データの入手方法、選択方法等） | OSD準拠のライセンスで利用可能 |
|  - 学習データのラベリング手順（使用する場合） | OSD準拠のライセンスで利用可能 |
|  - 学習データのクリーニング技法 | OSD準拠のライセンスで利用可能 |
| **コード**  |
|  - データ前処理 | OSI承認のライセンスで利用可能 |
|  - 学習、検証、テスト | OSI承認のライセンスで利用可能 |
|  - 推論 | OSI承認のライセンスで利用可能 |
|  - サポート用のライブラリとツール | OSI承認のライセンスで利用可能 |
| **モデル** |
|  - モデル・アーキテクチャ | OSI承認のライセンスで利用可能 |
|  - モデル・パラメータ | OSDに適合した条件で利用可能 |

以下のコンポーネントは改変を加えるための好ましい形式として必須ではないが、公開リリースに含めることを推奨される。

| オプションのコンポーネント |      法的枠組み          |
|----------------------| ------------------------------ |
| **データの情報** 以下を含む全てのデータセット： |
|  - 学習用データセット | OSD準拠のライセンスで利用可能 |
|  - テスト用データセット | OSD準拠のライセンスで利用可能 |
|  - 検証用データセット | OSD準拠のライセンスで利用可能 |
|  - ベンチマーク用データセット | OSD準拠のライセンスで利用可能 |
|  - データカード | OSD準拠のライセンスで利用可能 |
|  - 評価データ | OSD準拠のライセンスで利用可能 |
|  - 評価結果 | OSD準拠のライセンスで利用可能 |
|  - その他のデータ文書 | OSD準拠のライセンスで利用可能 |
| **コード** |
|  - ベンチマークテストの推論を実行するために使用されるコード | OSI承認のライセンスで利用可能 |
|  - 評価コード | OSI承認のライセンスで利用可能 |
| **モデル** 以下を含む全てのモデル要素： |
|  - モデル・カード | OSD準拠のライセンスで利用可能 |
|  - モデル出力のサンプル | OSD準拠のライセンスで利用可能 |
|  - モデルのメタデータ | OSD準拠のライセンスで利用可能 |
| **その他**  以下を含むその他の作成または使用した文書やツール： |
|  - 研究論文 | OSD準拠のライセンスで利用可能 |
|  - テクニカルレポート | OSD準拠のライセンスで利用可能 |