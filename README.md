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

## user テーブル

|Column|Type|Options|
|------|----|-------|
|id|integet|
|email|string|
|password|string|
|username|string|

### Association

- has many :tweets
- has many :comments

## tweets テーブル

|Column|Type|Options|
|------|----|-------|
|id|integet|
|text|text｜
|image|integet|
|user_id|integet|

### Association

- belongs_to :user
- has_many :comments

## comments テーブル

|Column|Type|Options|
|------|----|-------|
|id|integet|
|text|text|
|user_id|integet|
|tweets_id|integet|

### Association

- belongs_to :tweets
- belongs_to :user







