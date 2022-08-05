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

* Deployment instruct

###usersテーブル

| Colum                | Type     | options                 |
|--------------------- |----------|-------------------------|
| nickname             | string   | null:false              |
| email                | string   | null:false,unique: true |
| encrypted_password   | string   | null:false              |

#ASSOCIATION
has_many:targets


###targetテーブル

| Colum                | Type     | options                 |
|--------------------- |----------|-------------------------|
| meal                 | string   | null:false              |
| calorie              | string   | null:false              |
| motion               | string   | null:false              |

#association
has_many:users