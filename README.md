# Rails Sample 2024

### Version
* Ruby version : 3.2.2
* Rails version : 7.2.1.1
* Sqlite3 version : 3.39.5
* MySQL version : 8.0.40

### How to Run
1. Ruby 3.2.2 설치
```shell
rbenv install 3.2.2
rbenv global 3.2.2
```
2. api-2024 branch로 이동
```shell
git checkout api-2024
```
2. Gem 설치
```shell
bundle install
```
3. rails credential 수정
```shell
EDITOR="vim" bin/rails credentials:edit --environment development
```
- database 정보 추가
```xml
mysql:
    username: <mysql username>
    password: <mysql password>
    database: <mysql database>
```
4. database migrate
```
bin/rails db:migrate
```
5. rails 실행
```shell
bin/rails server
```