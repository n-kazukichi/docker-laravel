# docker-laravel

### 前提
- docker for mac最新版入れておいてください。

### チェックアウトしたらやること  
1. イメージをビルドして起動します   
1. app コンテナに入ります
1. composer でphp関連の諸々を入れます
1. laravel の .env を作成します
1. .env の APP_KEY を生成して設定します
----
1. [mac] $ docer compose up -d --build   
1. [mac] $ docker compose exec app bash
1. [app] $ composer install
1. [app] $ cp .env.example .env
1. [app] $ php artisan key:generate
