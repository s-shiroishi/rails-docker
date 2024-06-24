# 環境構築

## リポジトリの clone

好きなフォルダで以下のコマンドを実行してリポジトリの clone を行う。

```
git clone https://github.com/s-shiroishi/rails-docker.git
```

## アプリの起動

git clone を行ったフォルダで以下のコマンドを実行してコンテナを立てる。

```
docker compose up
```

## DB の初期化

```
docker-compose exec rails rake db:create db:migrate db:seed
```

http://localhost:3000 にアクセスすれば rails にアクセス出来る。
