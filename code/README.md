# ディレクトリ構成

第4章実験で使用したcodeは下記ディレクトリに保存
# 二値分類

**実験コード**

./experiment1_binary/binary_gridsearch.py

**実験コード説明**

*   def split_loov: train/testが同じデータ（フォーミュラリ）の場合，leave one out 法で分割.trainデータを標準化し，testデータをtrainデータの平均・分散で標準化

*   def split: trainデータを標準化し，testデータをtrainデータの平均・分散で標準化

*   def gridsearch: gridsearchによるハイパーパラメータ探索


# ランキング学習

**実験コード**

./experiment2_lerning_to_rank/ranklib_model_test_f6.py

**実験コード説明**

*   各defで14分割した各Foldに対して実行

*   def save_model: 各モデルを保存

*   def load_ivd: RabklibによるnDCGの値を保存

*   def load_score: ランキング学習結果のスコアを保存

**実験結果ファイルの命名規則**

*   model file: [train/test]_[model]-[Fold].txt

*   result file: [train/test]_[model]-[Fold]_result.txt

*   score file: [train/test]_[model]-[Fold]_score.txt

<略称>

*   g: 学会フォーミュラリ

*   k: 医療機関フォーミュラリデータ

*   model: rankerで示している．code参照


