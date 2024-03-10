# オープンソースAIの定義
### バージョン 0.0.6

:information_source: 注：この文書は3つの部分から構成されている： この文書の意図を述べた前文、オープンソースAIの定義そのもの、そして法的文書を評価するためのチェックリストである。

:information_source: この文書は、[経済協力開発機構(OECD)](https://legalinstruments.oecd.org/en/instruments/OECD-LEGAL-0449)が採用したAIシステムの定義に従っている。

> AIシステムとは、明示的または暗黙的な目的のために、受け取った入力から物理的または仮想的な環境に影響を与えることができる予測、コンテンツ、推奨、または決定などの出力を生成する方法を推論する機械ベースのシステムである。AIシステムによって、自律性や導入後の適応性のレベルは異なる。

AIシステムの定義の詳細については、[OSIのブログ](https://blog.opensource.org/open-source-ai-establishing-a-common-ground/)をご覧ください。


# 前文

## オープンソースの人工知能(AI)が必要な理由
オープンソースは、ソフトウェア・システムの学習、使用、共有、改善の障壁を取り除けば、誰にでも多大な恩恵がもたらされることを実証してきた。これらの恩恵は、オープンソースの定義に準拠したライセンスを使用した結果もたらされるものです。その恩恵は、自律性、透明性、共同改善に集約される。

AIによるこれらの恩恵は誰もが必要としている。ユーザーが信頼性と透明性のあるAIシステムを構築し、展開できるようにするため、我々には本質的な自由が必要である。

## 範囲外の問題
オープンソースAIの定義は、倫理的で信頼でき、あるいは責任あるAIシステムを開発し、展開する方法については述べていないが、それを妨げるものではない。政府の適切な規制を含め、AIシステムの責任ある開発、展開、使用について議論する取り組みは、別の話となる。

# オープンソースAIとは何か

オープンソースAIとは、以下のような自由を認める条件のもとで一般に公開されるAIシステムのことである：

* **使用**：どのような目的であれ、許可を得ることなくシステムを使用すること。
* **研究**：システムがどのように動作するかを研究し、そのコンポーネントを検査すること。
* **改変**：出力を変更することを含め、どのような目的であれシステムを改変すること。
* **共有**：どのような目的であれ、改変の有無に関わらず、他者が使用できるようにシステムを共有すること。

これらの自由を行使するための前提条件は、システムに修正を加えるための好ましい形式へのアクセス権を持っていることである。機械学習システムの場合、それは一般に公開されているものにアクセスできることを意味する：

* **データ**：学習方法および技術、使用された学習用データセット、それらのデータセットの出所およびその範囲と特徴に関する情報を含むシステムの学習方法に関する十分に詳細な情報。データがどのように取得と選択がされたか、ラベリングの手順とデータクリーニングの方法。
* **コード**：データの前処理に使用されたコード、学習と検証およびテストに使用されたコード、(使用されている場合)トークナイザーやハイパーパラメータ検索コード等のサポートライブラリ、推論コード、モデルアーキテクチャ。
* **モデル**：重みを含むモデル・パラメータ。適用可能な場合は、最終的なオプティマイザの状態だけでなく学習の重要な中間的段階も含める。

# 法的文書を評価するためのチェックリスト

この表は現在作成中です。詳細は1月26日のタウンホールの[スライドの7ページ目](https://opensource.org/wp-content/uploads/2024/01/osi_townhall_2.pdf)をご覧ください。


| 必須コンポーネント     |      法的枠組み          |
| ------------------------| ------------------------------ |
| **コード**  |
|  - データ前処理 | OSI準拠のライセンスで利用可能 |
|  - 学習、検証、テスト | OSI準拠のライセンスで利用可能 |
|  - 推論コード | OSI準拠のライセンスで利用可能 |
|  - サポート用のライブラリとツール | OSI準拠のライセンスで利用可能 |
| **モデル** |
|  - モデル・アーキテクチャ | OSI準拠のライセンスで利用可能 |
|  - モデル・パラメータ(重みを含む) | 次のフェーズで定義予定 |

以下のコンポーネントは必須ではありませんが、公開リリースに含めることを推奨します。

| オプションのコンポーネント |
|----------------------|
|  - ベンチマークテストの推論に使用されるコード |
|  - 評価コード |
| **データ** 以下を含む全てのデータセット： |
|  - 学習用データセット |
|  - テスト用データセット |
|  - 検証用データセット |
|  - ベンチマーク用データセット |
|  - データカード |
|  - 評価指標と結果 |
|  - その他の全データ文書 |
| **モデル** 以下を含む全てのモデル要素： |
|  - モデル・カード |
|  - モデル出力のサンプル |
| **その他**  以下を含むその他の作成または使用した文書やツール： |
|  - 研究論文 |
|  - 使用法の文書 |
|  - テクニカルレポート |
|  - サポートツール |