# オープンソースAIの定義
バージョン 0.0.5

:information_source:注：この文書は3つの部分から構成されている： この文書の意図を述べた前文、オープンソースAIの定義そのもの、そしてライセンスを評価するためのチェックリストである。

:information_source:この文書は、経済協力開発機構(OECD)が採用したAIシステムの定義に従っている。

    AIシステムとは、明示的または暗黙的な目的のために、受け取った入力から物理的または仮想的な環境に影響を与えることが
    できる予測、コンテンツ、推奨、または決定などの出力を生成する方法を推論する機械ベースのシステムである。
    AIシステムによって、自律性や導入後の適応性のレベルは異なる。

AIシステムの定義の詳細については、[OSIのブログ](https://blog.opensource.org/open-source-ai-establishing-a-common-ground/)をご覧ください。


## 前文
### オープンソースの人工知能(AI)が必要な理由

オープンソースは、ソフトウェア・システムの学習、使用、共有、改善の障壁を取り除けば、誰にでも多大な恩恵がもたらされることを実証してきた。これらの恩恵は、オープンソースの定義に準拠したライセンスを使用した結果もたらされるものです。その恩恵は、自律性、透明性、共同改善に集約される。

AIによるこれらの恩恵は誰もが必要としている。ユーザーが信頼性と透明性のあるAIシステムを構築し、展開できるようにするため、我々には本質的な自由を必要である。

### 範囲外の問題

オープンソースAIの定義は、倫理的で信頼でき、あるいは責任あるAIシステムを開発し、展開する方法については述べていないが、それを妨げるものではない。政府による適切な規制を含め、AIシステムの責任ある開発、展開、使用については、別の話として議論する努力を我々は支持する。

## オープンソースAIとは何か

オープンソースであるためには、AIシステムは以下の自由を認める法的条件の下で利用可能である必要がある：

- どのような目的であれ、許可を得ることなくシステムを使用すること。
- システムがどのように動作するかを研究し、そのコンポーネントを検査すること。
- 出力を変更することを含め、どのような目的であれシステムを改変すること。
- どのような目的であれ、改変の有無に関わらず、他者が使用できるようにシステムを共有すること。

## 法的文書を評価するためのチェックリスト

この表は現在作成中です。詳細は[このスライドの7ページ](https://opensource.org/wp-content/uploads/2024/01/osi_townhall_2.pdf)をご覧ください。

|  コンポーネント  | 使用に必要 | 研究に必要 | 改変に必要 | 共有に必要 |
| :---- | ---- | ---- | ---- | ---- |
| **コード**<br>以下を含むデータを解析し、処理するために使用される全てのコード： |  |  |  |  |
| - データ前処理コード |  |  |  |  |
| - トレーニングコード |  |  |  |  |
| - ベンチマークテストの推論に使用されるコード |  |  |  |  |
| - 検証コード |  |  |  |  |
| - 推論コード |  |  |  |  |
| - 評価コード |  |  |  |  |
| - トークナイザーやハイパーパラメーター検索コードなど、システムの一部であるその他のライブラリやコードの成果物 (使用された場合) |  |  |  |  |
| **データ**<br>以下を含む全てのデータセット： |  |  |  |  |
| - 学習用データセット |  |  |  |  |
| - テスト用データセット |  |  |  |  |
| - 検証用データセット |  |  |  |  |
| - ベンチマーク用データセット |  |  |  |  |
| - データカード |  |  |  |  |
| - 評価指標と結果 |  |  |  |  |
| - その他の全データ文書 |  |  |  |  |
| **モデル**<br>以下を含む全てのモデル要素： |  |  |  |  |
| - モデル・アーキテクチャ |  |  |  |  |
| - モデル・パラメータ(重みを含む) |  |  |  |  |
| - モデル・カード |  |  |  |  |
| - モデル出力のサンプル |  |  |  |  |
| **その他**<br>以下を含むその他の作成または使用した文書やツール |  |  |  |  |
| - 研究論文 |  |  |  |  |
| - 使用法の文書 |  |  |  |  |
| - テクニカルレポート |  |  |  |  |
| - サポートツール |  |  |  |  |