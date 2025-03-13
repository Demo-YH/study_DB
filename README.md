# DB個人学習用  
## 環境  
<img alt="Static Badge" src="https://img.shields.io/badge/wsl2-w?style=plastic&logo=linux&logoColor=000000&labelColor=%23FCC624&color=%23FCC624">　<img alt="Static Badge" src="https://img.shields.io/badge/Docker-d?style=plastic&logo=docker&logoColor=%23ffffff&labelColor=%232496ED&color=%232496ED">　<img alt="Static Badge" src="https://img.shields.io/badge/MySQL-m?style=plastic&logo=mysql&logoColor=%23ffffff&labelColor=%234479A1&color=%234479A1">

## 構築手順  
#### 1. wsl使用の為、仮想マシン プラットフォームを有効化  
####  (wslがインストールされていない場合:Linuxカーネル更新プログラムパッケージを  
####  インストールする)  
#### 2. wsl --set-default-version 2 コマンドでLinuxを標準でWSL2上で動くように設定  
#### 3. wsl --list --verbose　コマンドでLinuxがWSL1とWSL2のどちらで動いているかを確認  
#### 4. ubuntuをインストール  
#### 5. terminalにてアカウント作成  
※WSLにて環境構築済みの場合、6から作業実施  
#### 6. 任意のフォルダ作成  
#### 7. Docker Desktopインストール  
#### 8. dockerでwslを使用する設定に変更  
#### 9. terminalに戻りdockerで使用するイメージのフォルダ構成作成 
※mysql配下にmy.cnf作成 
#### 10. docker-composer.ymlにて作成するコンテナの初期状態を
#### 「ports:」「volumes:」などYAML形式を用いて定義。  
#### 11. その他の使用するイメージの設定ファイル(my.cnf)作成  
#### 12. docker compose up -d　コマンドを実行してコンテナの作成・起動  
#### 13. docker exec -it container ID  bashでコンテナにはいる  
#### 14. mysql -u[ユーザー名] -p -h localhost -p [ポート番号] --protocol=tcpコマンドでMySQLにログイン
