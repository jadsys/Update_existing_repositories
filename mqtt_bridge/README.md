mqtt_bridge
=======

概要
=======
このパッケージはMQTT-ROS間のメッセージをブリッジするためのパッケージである、[groove-x/mqtt_bridge](https://github.com/groove-x/mqtt_bridge)をロボットで動作させるための起動用launchファイル及びメッセージ通信用コンフィグを含んだパッケージです。
なお、動作確認に使用したrevisionは["21b6ff56b428cd15ae2b01783a1d2fee028fc431"](https://github.com/groove-x/mqtt_bridge/commit/21b6ff56b428cd15ae2b01783a1d2fee028fc431)となります。

インストール方法
=======
### 1．ROSワークスペースのディレクトリに移動し、リポジトリをクローンし、ファイルを上書き
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/

# megarover_samplesのクローン
git clone https://github.com/groove-x/mqtt_bridge.git

# 動作確認済みrevisionへのチェックアウト
cd mqtt_bridge
git checkout 21b6ff56b428cd15ae2b01783a1d2fee028fc431

# 追加パッケージのクローン
mkdir ~/work
cd ~/work
git clone -b "2023年度成果物" https://github.com/jadsys/Update_existing_repositories.git

# ファイルの展開
cp -r Update_existing_repositories/mqtt_bridge/ ~/{ROSワークスペースディレクトリ}/src/

```

### 2．Buildを行う
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/mqtt_bridge
catkin build --this
```

### X. 依存関係
当パッケージでは外部パッケージとして以下を利用しております。
- [mqtt_bridge](https://github.com/groove-x/mqtt_bridge.git)
- [uoa_poc4_msgs](https://github.com/jadsys/uoa_poc4_msgs.git)
- [uoa_poc6_msgs](https://github.com/jadsys/uoa_poc6_msgs.git)

それぞれのインストールを行います。
```bash
# vcsツールのインストール（既にインストール済みの場合スキップ）
sudo pip install -U vcstool

# 依存関係のインストール
cd ~/{ROSワークスペースディレクトリ}/src
vcs import  < mqtt_bridge/dependency.rosinstall
catkin build
```

ライセンス
=======
## BSD 3-Clause License

Copyright (c) 2023, Japan Advanced System,Ltd.
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.

* Neither the name of the copyright holder nor the names of its contributors 
   may be used to endorse or promote products derived from this software 
   without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

* * *
## 使用ライブラリ関係
### [mqtt_bridge](https://github.com/groove-x/mqtt_bridge.git)
 [MIT License](https://opensource.org/licenses/MIT):
 Copyright (c) 2016 GROOVE X, Inc.