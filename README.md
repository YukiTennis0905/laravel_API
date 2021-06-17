## How to confirm on local
1. .env.sampleを.envにコピーする
```
cp .env.example .env
```

2. マイグレーション＆シード入れる
```
php artisan migrate
php artisan db:seed
```
3.アプリを立ち上げる
```
php artisan serve
```

## How to test　（Postman使用）

### 記事リスト取得
GET http://localhost:8000/api/articles

### 記事追加
POST http://localhost:8000/api/articles
下記カラムに値を入れる
title、body

### 特定の記事取得
GET http://localhost:8000/articles/api/{記事}ID

### 記事編集
PUT http://localhost:8000/articles/api/{記事ID}
下記カラムに値を入れる
title、body

### 記事削除
DELETE http://localhost:8000/articles/api/{記事ID}


