velodyne
=======

概要
=======
このパッケージはVelodyne社のLiDARである、VLP-16をROSで動かすためのパッケージである、[ros-drivers/velodyne](https://github.com/ros-drivers/velodyne)に弊社自律移動システムで動作させるための設定を記載した起動用launchを含んでます。
なお、動作確認に使用したrevisionは["29abd0e1361cb7f5eda451d2b51c35eeca45e0d5"](https://github.com/ros-drivers/velodyne/commit/29abd0e1361cb7f5eda451d2b51c35eeca45e0d5)となります。

インストール方法
=======
### 1．ROSワークスペースのディレクトリに移動し、リポジトリをクローンし、ファイルを上書き
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/

# megarover_samplesのクローン
git clone https://github.com/ros-drivers/velodyne.git

# 動作確認済みrevisionへのチェックアウト
cd velodyne
git checkout 29abd0e1361cb7f5eda451d2b51c35eeca45e0d5

# 追加パッケージのクローン
mkdir ~/work
cd ~/work
git clone -b "2023年度成果物" https://github.com/jadsys/Update_existing_repositories.git

# ファイルの展開
cp -r Update_existing_repositories/velodyne/ ~/{ROSワークスペースディレクトリ}/src/

```

### 2．Buildを行う
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/velodyne
catkin build --this
```

### X. 依存関係
当パッケージでは外部パッケージとして以下を利用しております。
- [velodyne](https://github.com/ros-drivers/velodyne.git)

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
### [velodyne](https://github.com/ros-drivers/velodyne.git)
 [BSD License](https://opensource.org/licenses/bsd-3-clause)