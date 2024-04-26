teleop_twist_joy
=======

概要
=======
このパッケージはジョイパッドでロボットを動かすためのパッケージである、[ros-teleop/teleop_twist_joy](https://github.com/ros-teleop/teleop_twist_joy)にPS4コントローラーで[Choreonoid](https://github.com/choreonoid/choreonoid)上で動作するロボットを操作ための更新を含んだパッケージです。
なお、動作確認に使用したrevisionは["4f61e6d853138b153aeda0984d2abeb7a04d87bb"](https://github.com/ros-teleop/teleop_twist_joy/commit/4f61e6d853138b153aeda0984d2abeb7a04d87bb)となります。

インストール方法
=======
### 1．ROSワークスペースのディレクトリに移動し、リポジトリをクローンし、ファイルを上書き
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/

# megarover_samplesのクローン
git clone https://github.com/ros-teleop/teleop_twist_joy.git

# 動作確認済みrevisionへのチェックアウト
cd teleop_twist_joy
git checkout 4f61e6d853138b153aeda0984d2abeb7a04d87bb

# 追加パッケージのクローン
mkdir ~/work
cd ~/work
git clone -b "2023年度成果物" https://github.com/jadsys/Update_existing_repositories.git

# ファイルの展開
cp -r Update_existing_repositories/teleop_twist_joy/ ~/{ROSワークスペースディレクトリ}/src/

```

### 2．Buildを行う
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/teleop_twist_joy
catkin build --this
```

### X. 依存関係
当パッケージでは外部パッケージとして以下を利用しております。
- [teleop_twist_joy](https://github.com/ros-teleop/teleop_twist_joy.git)

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
### [teleop_twist_joy](https://github.com/ros-teleop/teleop_twist_joy.git)
 [BSD License](https://opensource.org/licenses/bsd-3-clause)