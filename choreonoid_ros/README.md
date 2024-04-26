choreonoid_ros
=======

概要
=======
このパッケージは[Choreonoid](https://github.com/choreonoid/choreonoid)とROSのメッセージを変換するためのパッケージである、[choreonoid_ros](https://github.com/choreonoid/choreonoid_ros)へ複数台のロボットを対応させるためのソースコードです。
なお、動作確認に使用したrevisionは["fa7369b8ad27cf0de98e9759cd912de0b6488a9a"](https://github.com/choreonoid/choreonoid_ros/commit/fa7369b8ad27cf0de98e9759cd912de0b6488a9a)となります。

インストール方法
=======
### 1．ROSワークスペースのディレクトリに移動し、リポジトリをクローンし、ファイルを上書き
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/

# Choreonoid_rosのクローン
git clone https://github.com/choreonoid/choreonoid_ros.git

# 動作確認済みrevisionへのチェックアウト
cd choreonoid_ros
git checkout fa7369b8ad27cf0de98e9759cd912de0b6488a9a

# 追加パッケージのクローン
mkdir ~/work
cd ~/work
git clone -b "2023年度成果物" https://github.com/jadsys/Update_existing_repositories.git

# ファイルの展開
cp -r Update_existing_repositories/choreonoid_ros/ ~/{ROSワークスペースディレクトリ}/src/

```
※1 [公式ドキュメント](https://choreonoid.org/ja/manuals/latest/ros/build-choreonoid.html#id16)を参照

### 2．Buildを行う
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/choreonoid_ros
catkin build --this
```
### X. 依存関係
当パッケージでは外部パッケージとして以下を利用しております。
- [Choreonoid](https://github.com/choreonoid/choreonoid.git)
- [Choreonoid_ros](https://github.com/choreonoid/choreonoid_ros.git)

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
### [Choreonoid](https://github.com/choreonoid/choreonoid.git)
 [MIT License](https://opensource.org/licenses/MIT): 
 Copyright (c) 2019-2024 Choreonoid Inc.
 Copyright (c) 2007-2019
    Shin'ichiro Nakaoka and the Choreonoid development team,
    Intelligent Systems Research Institute,
    National Institute of Advanced Industrial Science and Technology (AIST)
### [Choreonoid_ros](https://github.com/choreonoid/choreonoid.git)
 [MIT License](https://opensource.org/licenses/MIT): 