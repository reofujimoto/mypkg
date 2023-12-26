# mypkg
[![test](https://github.com/reofujimoto/robosys2023/actions/workflows/test.yml/badge.svg)](https://github.com/reofujimoto/mypkg/actions)

ロボットシステム学2023の練習リポジトリ
授業で作成したプログラム

## リポジトリの内容
* talker.py
  * 1から順に数字をカウントして`countup`というトピック名でトピック通信するノード。

* listener.py
  * `talker.py`から`countup`というトピック名でトピック通信し、メッセージを貰って表示するノード。  これを実行するには、新しいターミナルを開いて実行。  

## launch
* 機能

`talker.py`と`listener.py`の２つのノードを同時に実行できるノード。

* 実行例

```bash
$ ros2 launch mypkg talk_listen.launch.py


```


## 動作環境
### 必要なソフトウェア　

* python
  * テスト済み：3.7 ~ 3.10

### テスト環境
* ubuntu 22.04.3 LTS

## 著作権・ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
  
* このパッケージのコードは，下記のGitHub上のコードを参照し，本人の許可を得て自身の著作としたものです． 
  * [ryuichiueda/robosys2023](https://github.com/ryuichiueda/robosys2023)

  * © 2023 Reo Fujimoto 
