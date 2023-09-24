# 記録

## exp1:baseline
チュートリアルを基本的には、自分の環境・コードに置き換え  
run blocksで若干選んでいる特徴を増やしている。  (ex 市区町村コード)  
誤ってgroup_colを市区町村名 → 都道府県にしたが そのままsub

* CV条件 : Hold out（チュートリアルと同じ）
* model : lightgbm
  * param : チュートリアルと同じ

### スコア
mae
| train | val    | test  |
| ----- | ------ | ----- |
|       | 0.0773 | 0.088 |

* best iteration : 5300

### 備考
過学習気味  
baselineができたのでまずはCVの切り方を検証


## exp2:CVの切り方
