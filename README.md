# Camp Plan

キャンプ計画を、事実・判断・実行タスクに分けて管理するリポジトリです。

## クイックリファレンス

| 項目 | 内容 | 詳細 |
| --- | --- | --- |
| 日程 | 2026-05-15〜2026-05-16（1泊） | [全体像](docs/overview.md), [当日スケジュール](docs/schedule.md) |
| 目的地 | 尾高高原キャンプ場 | [予約・キャンプ場](docs/site-and-booking.md) |
| 参加者 | 達平、今井、平井 | [参加者台帳](data/participants.csv) |
| サイト | フリーサイト | [予約・キャンプ場](docs/site-and-booking.md) |
| サイト料金 | 入場料込み2,700円 | [予算](docs/budget.md), [費用台帳](data/budget.csv) |
| スタート | 名古屋市金山。イオンモール東員10:00着から逆算して出発 | [移動と買い出し](docs/transport.md), [当日スケジュール](docs/schedule.md) |
| 買い出し | イオンモール東員で10:00開始 | [移動と買い出し](docs/transport.md), [食事計画](docs/meals.md) |
| 予約 | 未実施。電話予約 | [予約前チェック](docs/site-and-booking.md), [ToDo](tasks/todo.md) |
| 食事 | レシピ・必要食材が未確定のメニューはTODO扱い | [食事計画](docs/meals.md), [ToDo](tasks/todo.md) |

## 用語定義

| 用語 | 意味 |
| --- | --- |
| `食材` | 米、塩など、買い出しや持ち物として持つときの粒度の単位 |
| `メニュー` | `食材` から作られる料理の単位。実際に食べるときの単位 |

## ナビゲーション

| 用途 | ドキュメント |
| --- | --- |
| 全体像、決定事項、未決事項 | [docs/overview.md](docs/overview.md) |
| 当日の流れ | [docs/schedule.md](docs/schedule.md) |
| キャンプ場、予約、現地ルール | [docs/site-and-booking.md](docs/site-and-booking.md) |
| 移動、集合、買い出し地点 | [docs/transport.md](docs/transport.md) |
| 共有装備の確認 | [docs/gear.md](docs/gear.md), [data/gear.csv](data/gear.csv) |
| 食事計画、レシピ、買い出し観点 | [docs/meals.md](docs/meals.md) |
| レシピ従属の必要食材リスト | [docs/food-list.md](docs/food-list.md) |
| 食べたいもの候補 | [docs/food-wishlist.md](docs/food-wishlist.md) |
| 予算と精算 | [docs/budget.md](docs/budget.md), [data/budget.csv](data/budget.csv) |
| 安全確認、緊急連絡 | [docs/safety.md](docs/safety.md) |
| 実行タスク | [tasks/todo.md](tasks/todo.md) |
| 外部情報の控え | [references/odaka-camp.md](references/odaka-camp.md), [references/shopping.md](references/shopping.md) |
| 画像、予約控え、添付資料 | [assets/README.md](assets/README.md) |

## 情報の置き方

スクラッチで作るなら、同じ事実を複数ファイルに書かず、次の責務で分けます。

| 領域 | 役割 | 例 |
| --- | --- | --- |
| `data/` | 確定情報と台帳。表計算、集計、更新の正本 | `trip.yaml`, `gear.csv`, `budget.csv` |
| `docs/` | 人が読む計画書。判断、段取り、チェック観点 | `overview.md`, `schedule.md`, `meals.md` |
| `references/` | 外部情報の控え。確認日と参照元を残す | キャンプ場情報、買い出し情報 |
| `tasks/` | 実行タスク。未決事項を完了まで追う | `todo.md` |
| `assets/` | 画像、PDF、予約控えなどのファイル | 地図、スクリーンショット |

## 更新ルール

- 確定した事実は `data/` を先に更新する。
- 判断理由、手順、当日の使いやすさは `docs/` に書く。
- 外部情報を写した場合は `references/` に確認日を残す。
- `docs/recipes/` を食材の正とし、レシピを追加、更新、削除したら `docs/food-list.md` も同じ変更で更新する。
- レシピ上必須の調理器具が `data/gear.csv` で担当未定なら、誰が持ってくるか決めるタスクを `tasks/todo.md` に追加する。
- 予約番号、個人連絡先、決済情報は `local/` に置き、Git管理しない。

## ディレクトリ

```text
.
├── assets/       # 地図画像、予約控え、写真など
├── data/         # 更新しやすい台帳データ
├── docs/         # 人が読む計画書
├── references/   # 外部資料メモ
└── tasks/        # ToDoと進行管理
```
