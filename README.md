# テーブル設計

## users テーブル

| Column             | Type   | Options     |
| ------------------ | ------ | ----------- |
| name               | string | null: false |
| email              | string | null: false, unique:
| profile            | text   | null: false, unique: 
| email              | string | null: false, unique: 
 true |
| encrypted_password | string | null: false |

## prototypes テーブル

| Column | Type   | Options     |
| ------ | ------ | ----------- |
| name   | string | null: false |


## comments テーブル

| Column  | Type       | Options                        |
| ------- | ---------- | ------------------------------ |
| content | string     |                                |
| user    | references | null: false, foreign_key: true |
| room    | references | null: false, foreign_key: true |