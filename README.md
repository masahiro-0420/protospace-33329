# テーブル設計

## users テーブル

| Column     | Type   | Options     |
| --------   | ------ | ----------- |
| email      | string | null: false |
| password   | string | null: false |
| name       | string | null: false |
| profile    | text   | null: false |
| occupation | text   | null: false |
| position   | text   | null: false |


## prototype テーブル

| Column     | Type          | Options     |
| --------   | ------        | ----------- |
| title      | string        | null: false |
| catch_copy | text          | null: false |
| concept    | text          | null: false |
| image      | ActiveStorage |             |
| user       | references    |             |


## comments テーブル

| Column | Type       | Options     |
| ------ | ---------- | ----------- |
| user   | text       | null: false |
| user   | references |             |
| room   | references |             |

