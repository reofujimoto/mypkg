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
* talk_listen.launch.py
  * `talker.py`と`listener.py`の２つのノードを同時に実行可能とし表示させる。

* 実行例

```bash
$ ros2 launch mypkg talk_listen.launch.py
[INFO] [launch]: All log files can be found below /home/reo/.ros/log/2023-12-26-16-30-48-665078-DESKTOP-V4N2IEO-2454
[INFO] [launch]: Default logging verbosity is set to INFO
[INFO] [talker-1]: process started with pid [2455]
[INFO] [listener-2]: process started with pid [2457]
[listener-2] [INFO] [1703575849.635908220] [listener]: Listen: 0
[listener-2] [INFO] [1703575850.115017370] [listener]: Listen: 1
[listener-2] [INFO] [1703575850.615238309] [listener]: Listen: 2
[listener-2] [INFO] [1703575851.115211547] [listener]: Listen: 3
[listener-2] [INFO] [1703575851.617064785] [listener]: Listen: 4
[listener-2] [INFO] [1703575852.117637124] [listener]: Listen: 5
[listener-2] [INFO] [1703575852.617066063] [listener]: Listen: 6
[listener-2] [INFO] [1703575853.117288801] [listener]: Listen: 7
[listener-2] [INFO] [1703575853.617367940] [listener]: Listen: 8
[listener-2] [INFO] [1703575854.117196479] [listener]: Listen: 9
[listener-2] [INFO] [1703575854.617290738] [listener]: Listen: 10
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
