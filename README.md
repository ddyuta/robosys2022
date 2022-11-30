[![test](https://github.com/yuutadoumen/robosys2022/actions/workflows/test.yml/badge.svg)](https://github.com/yuutadoumen/robosys2022/actions/workflows/test.yml)

# robosys2022
ロボットシステム学の練習リポジトリ

# plusコマンド
標準入力から読み込んだ数字を足す。

## インストール方法
```
git clone https://github.com/yuutadoumen/robosys2022.git
```
## plusコマンド詳細
* 標準入力に使うseqコマンドは1から指定した数まで1つずつ加算されていく連続する数字を>列挙するものでseqコマンドの性質上、標準入力する数字は1以上の整数と限定される。　　  
* 有限小数を標準入力する際は小数が切り捨てされた数字が実行される。(実行例2)
* 1より小さい数で実行すると出力は必ず0になる。(実行例3)
### 実行例
##### 基本
標準入力
```
seq 5 | ./plus
```

出力
```
15
```
### 実行例2
##### 有限小数で実行したとき
標準入力
```
seq 5.55　| ./plus
```
出力
```
15
```
### 実行例3
##### 1より小さい数で実行したとき
標準入力
```
seq -5.5 | ./plus
```
出力
```
0
```
## 動作確認済み環境
- Ubuntu 18.04
- Python 3.7~3.10

## ライセンス
  * このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
  * このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
      * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)
  * ⓒ 2022 Yuta Domen```
