# laravel10でLEMP環境を構築（備忘録）
Dockerを用いたLEMP環境を構築
### 使用技術
以下の技術を使用
- PHP8
- Laravel10
- Nginx
- MySQL8
- Docker docker-compose

### 手順
#### 1.このリポジトリをクローンする。
```
git clone git@github.com:ooooose/laravel10_setup.git 
```
#### 2.コンテナを起動（数分かかる）し、appサービスに入る。
```
docker-compose up -d
```
起動した状態で、以下のコマンドを実行。appサービスに入ることができる。
```
docker-compose exec app bach
```
#### 3.コンテナ（appサービス）に入った状態でLaravelプロジェクトを立ち上げる。
```
composer create-project --prefer-dist laravel/laravel laravel_project "10.*"
```
