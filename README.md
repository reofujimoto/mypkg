# mypkg


ロボットシステム学2023のROS2講義用リポジトリ

## このリポジトリで使用可能なノード
* talker

* listener

## インストール方法
下記のコードをホームディレクトリでクローンしてください
```
git clone https://github.com/yossyhira/mypkg.git
```
cdコマンドを使い、mypkgディレクトリに移動してください
```
cd mypkg
```
下記の方法でtalkerとlistenerを実行してください

## 各ノードの機能


### talker
* 機能


### listener
* 機能

  talkerからcountupというトピックを通じて、メッセージをサブスクライブしたものを端末に出力する。

## launch
* 機能

  talkerとlistenerを同時に実行する

* 実行方法

```bash
$ ros2 launch mypkg talk_listen.launch.py


```


## 動作環境
### 必要なソフトウェア　

* python
  * テスト済み：3.7 ~ 3.10

### テスト環境
* ubuntu 22.04.2 LTS
  * ROS2 humble

### テストに利用したコンテナ


を利用させていただきました。

## ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
  
  * このパッケージのtest.ymlのpythonのバージョンテスト部分以外のコードは，

のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです.

  * © 2023 Reo Fujimoto 
