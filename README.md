# Camp Plan

キャンプ計画のためのリポジトリです。計画の全体像、予約、移動、装備、食事、予算、安全確認、振り返りを分けて管理します。

## 使い方

1. `data/trip.yaml` に日程、場所、参加者、集合情報を入力する。
2. `docs/overview.md` で目的、前提、決定事項を整理する。
3. `docs/schedule.md`、`docs/site-and-booking.md`、`docs/transport.md` を埋めて当日の流れを固める。
4. `data/gear.csv`、`data/meal-plan.csv`、`data/budget.csv` を更新して準備状況を管理する。
5. 出発前に `tasks/todo.md` と `docs/safety.md` を確認する。
6. 終了後に `docs/retrospective.md` に次回への改善点を残す。

## 構成

```text
.
├── README.md
├── assets/              # 地図画像、予約控え、写真など
├── data/                # 更新しやすい台帳データ
├── docs/                # 人が読む計画書
├── references/          # キャンプ場情報、規約、外部資料メモ
└── tasks/               # ToDoと進行管理
```

## 重要ファイル

- `data/trip.yaml`: 計画の基本情報
- `docs/overview.md`: 全体サマリと意思決定
- `docs/schedule.md`: 当日のタイムライン
- `docs/site-and-booking.md`: キャンプ場・予約情報
- `docs/gear.md`: 装備方針
- `data/gear.csv`: 装備チェックリスト
- `docs/meals.md`: 食事計画
- `data/meal-plan.csv`: 食材・献立管理
- `docs/budget.md`: 予算方針
- `data/budget.csv`: 費用台帳
- `docs/safety.md`: 安全・緊急時対応
- `tasks/todo.md`: 作業一覧

## 運用ルール

- 事実として確定した情報は `data/` に記録する。
- 判断理由や補足は `docs/` に記録する。
- 予約番号、個人連絡先、決済情報などの機密情報は公開リポジトリに置かない。
- 天気、交通、営業状況は出発前に最新情報を確認する。
# 2026-05-15
