# README




This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


## usersテーブル

|Column|Type|Options|
|------|----|-------|
|user_id|references|null: false, foreign_key: true|
|user_name|string|null: false, foreign_key: true|
|birthday|datetime|null: false, foreign_key: true|
|mail_address|string|null: false, foreign_key: true|
|login_password|string|null: false, foreign_key: true|
|sales|integer|foreign_key: true|
|point|integer|foreign_key: true|

### Association

## goodsテーブル
|goods_id|references|null: false, foreign_key: true|
|goods_name|string|null: false, foreign_key: true|
|exhibitor_id|integer|null: false, foreign_key: true|
|exhibitor_name|string|null: false, foreign_key: true|
|image|string|null: false, foreign_key: true|
|point|integer|null: false, foreign_key: true|
|buyer_id|integer|foreign_key: true|
|buyer_name|string|foreign_key: true|

### Association
- belongs_to :users
