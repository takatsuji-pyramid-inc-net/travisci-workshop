[![Build Status](https://travis-ci.org/takatsuji-pyramid-inc-net/travisci-workshop.svg?branch=master)](https://travis-ci.org/takatsuji-pyramid-inc-net/travisci-workshop)


# TravisCI勉強会

## ゴール

以下の要件を満たすCI環境を構築してください。

### 要件

- 対象リポジトリの全ブランチへのPushを契機にCIが実行される

---

- CIとして下記を実行
	* css/内の各*.cssファイルを bin/yuicompressor-2.4.8.jar を使ってminify
	* minifyされたファイル郡をS3にデプロイする
		*  デプロイ先は下記の命名規則に沿うようにする
			* **s3://<任意のバケット名>/<Gitブランチ名>/<ビルド回数>/**
		* S3にアクセスするためのAWSクレデンシャルは環境変数経由で指定すること
	* ビルドの成否をslackに通知する

---

- リポジトリのREADME.mdにビルドバッジを貼り付ける

