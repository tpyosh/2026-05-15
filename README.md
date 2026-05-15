# Camp Day

2026-05-15〜2026-05-16 の尾高高原キャンプ場キャンプを、当日に人が迷わず見るためのリポジトリです。

まず [docs/today.md](docs/today.md) を見てください。

## 今日の固定情報

| 項目 | 内容 |
| --- | --- |
| 日程 | 2026-05-15〜2026-05-16（1泊） |
| 参加者 | 達平、今井、平井 |
| 行き先 | 尾高高原キャンプ場（三重県三重郡菰野町） |
| 集合 | 名古屋市金山。イオンモール東員10:00着から逆算 |
| 買い出し | イオンモール東員、10:00開始 |
| チェックイン | 11:00〜16:00 |
| チェックアウト | 8:00〜10:00 |
| 予約 | 予約済み。控えは `local/` を見る |
| サイト | フリーサイト |
| 料金 | 入場料込み2,700円 |
| キャンプ場電話 | 059-396-3900 |

## まず潰す未決事項

| 優先 | 未決事項 | 見る場所 |
| --- | --- | --- |
| 高 | 出発時刻、車、ドライバー | [docs/today.md](docs/today.md), [docs/transport.md](docs/transport.md) |
| 高 | 夕食と朝食のメニュー | [docs/today.md](docs/today.md), [docs/meals.md](docs/meals.md) |
| 高 | 買い出し対象の食材 | [docs/today.md](docs/today.md), [docs/food-list.md](docs/food-list.md) |
| 高 | 担当未定の共有装備 | [docs/gear.md](docs/gear.md), [data/gear.csv](data/gear.csv) |
| 中 | 予約控え、支払い方法、車台数の追加連絡 | [docs/site-and-booking.md](docs/site-and-booking.md), [tasks/todo.md](tasks/todo.md) |

## 今日見る順

| 用途 | ドキュメント |
| --- | --- |
| 当日の入口 | [docs/today.md](docs/today.md) |
| 時間の流れ | [docs/schedule.md](docs/schedule.md) |
| 移動、集合、買い出し地点 | [docs/transport.md](docs/transport.md) |
| 食事とメニュー候補 | [docs/meals.md](docs/meals.md) |
| レシピ従属の食材一覧 | [docs/food-list.md](docs/food-list.md) |
| 共有装備 | [docs/gear.md](docs/gear.md), [data/gear.csv](data/gear.csv) |
| 受付、料金、現地ルール | [docs/site-and-booking.md](docs/site-and-booking.md) |
| 安全確認、緊急連絡 | [docs/safety.md](docs/safety.md) |
| 実行タスク | [tasks/todo.md](tasks/todo.md) |

## 用語

| 用語 | 意味 |
| --- | --- |
| `食材` | 米、塩など、買い出しや持ち物として持つときの粒度の単位 |
| `メニュー` | `食材` から作られる料理の単位。実際に食べるときの単位 |

## ファイルの役割

| 領域 | 役割 |
| --- | --- |
| `data/` | 確定情報と台帳 |
| `docs/` | 人が読む当日用メモと詳細 |
| `docs/recipes/` | レシピの正本 |
| `references/` | 外部情報の控え |
| `tasks/` | 今日処理するタスク |
| `assets/` | 地図、画像、公開してよい添付 |
| `local/` | 予約番号、個人連絡先、決済情報などGit管理しない情報 |

## 更新ルール

- 確定した事実は `data/` を先に更新する。
- 当日に見る情報は `docs/today.md` か、そこから1クリックの場所に置く。
- `docs/recipes/` を食材の正とし、レシピを追加、更新、削除したら `docs/food-list.md` も同じ変更で更新する。
- `docs/food-list.md` は全登録レシピの食材一覧であり、未確定メニューまで含む。買い出しでは選んだメニュー分だけ使う。
- レシピ上必須の調理器具が `data/gear.csv` で担当未定なら、誰が持ってくるか決めるタスクを `tasks/todo.md` に追加する。
