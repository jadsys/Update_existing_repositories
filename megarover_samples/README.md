megarover_samples
=======

概要
=======
このパッケージは[Vstone社メガローバーのGazebo用に構築されたモデルデータ及びURDF](https://github.com/vstoneofficial/megarover_samples)を[Choreonoid](https://github.com/choreonoid/choreonoid)上で動作させるための更新を含んだパッケージです。
なお、動作確認に使用したrevisionは["b7efaae40d3ed7f99905e1f38a6cab97b30c8e12"](https://github.com/vstoneofficial/megarover_samples/commit/b7efaae40d3ed7f99905e1f38a6cab97b30c8e12)となります。

インストール方法
=======
### 1．ROSワークスペースのディレクトリに移動し、リポジトリをクローンし、ファイルを上書き
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/

# megarover_samplesのクローン
git clone https://github.com/vstoneofficial/megarover_samples.git

# 動作確認済みrevisionへのチェックアウト
cd megarover_samples
git checkout b7efaae40d3ed7f99905e1f38a6cab97b30c8e12

# 追加パッケージのクローン
mkdir ~/work
cd ~/work
git clone -b "2023年度成果物" https://github.com/jadsys/Update_existing_repositories.git

# ファイルの展開
cp -r Update_existing_repositories/megarover_samples/ ~/{ROSワークスペースディレクトリ}/src/

```
### X. 依存関係
当パッケージでは外部パッケージとして以下を利用しております。
- [megarover_samples](https://github.com/vstoneofficial/megarover_samples.git)

### 2．Buildを行う
```bash 
cd ~/{ROSワークスペースディレクトリ}/src/megarover_samples
catkin build --this
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
### [megarover_samples](https://github.com/vstoneofficial/megarover_samples.git)
 [MIT License](https://opensource.org/licenses/MIT)