# Name（リポジトリ/プロジェクト/OSSなどの名前）

DockerでシンプルなMySQLを環境構築します。
MySQLのDBをとりあえず作りたいときに使用します。

# Features

MySQL:8.0.28
コンテナを停止してもデータは永続化される

# Requirement


# Installation

* 起動
docker compose up -d

* コンテナイメージ一覧
docker image ls

* 実行中のコンテナ一覧
docker ps


# Usage

* 起動後にコンテナにログイン
docker exec -it mysql-container bash

* ログインユーザの確認
id

* Linuxカーネルの確認
uname -a

* Linuxディストリビューションの確認
cat /etc/os-release

* MySQLバージョンの確認
mysql --version

* ルートユーザでMySQLにログイン。パスワードを聞かれるのでrootと入力
mysql -u root -p

*　なお、通常は「user」「password」で接続する

# Note

* コンテナの停止。コンテナの削除も同時に行う
docker compose down

* 設定を変えたいときは、my.cnfを修正

# Author

# License
