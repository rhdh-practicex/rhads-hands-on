# RHADS Hands-on

Red Hat Advanced Developer Suite（RHADS）と中核コンポーネントである Red Hat Developer Hub（RHDH）を、短いハンズオンで体験するための資料リポジトリです。

社内勉強会・社外ワークショップのどちらでも使えるように、**機密・顧客名・実クラスタ情報は含めません**。環境固有の値はプレースホルダで扱います。

## 目的

- RHADS の製品群と役割分担を短時間で把握する
- RHDH を起点に「開発者ポータル × サプライチェーン信頼」の価値を体験する
- 社内では知見共有とコミュニティ活性化、社外では再現可能なハンズオンとして再利用する

## 対象

| 対象 | 想定 |
|------|------|
| 社内 | プラットフォーム／アプリ／セキュリティに関心のあるエンジニア、プリセールス、伴走メンバー |
| 社外 | 顧客・パートナー向けの概要ハンズオン（検証済み手順の延長） |

前提知識: Kubernetes / OpenShift の基本用語、Git の基本操作。RHADS 未経験でも参加可。

## 社内 / 社外の使い分け

| | 社内 | 社外 |
|--|------|------|
| ゴール | [docs/GOALS.md](docs/GOALS.md) の「社内向け」 | 同ファイルの「社外向け」 |
| トーン | 認知向上・共有・フィードバック歓迎 | 再現性・完了条件・次アクション重視 |
| 禁止事項 | 顧客名・案件名・社内専用 URL を資料に固定しない | 同上＋検証クラスタの実接続情報を貼らない |

詳細アジェンダ: [docs/AGENDA.md](docs/AGENDA.md)  
製品概要: [docs/RHADS_OVERVIEW.md](docs/RHADS_OVERVIEW.md)  
SMART ゴール: [docs/GOALS.md](docs/GOALS.md)

## クイックスタート

1. 本リポジトリを clone する
2. [docs/RHADS_OVERVIEW.md](docs/RHADS_OVERVIEW.md) で製品群を 5〜10 分確認する
3. [docs/AGENDA.md](docs/AGENDA.md) に沿って進行する（目安 90〜120 分）
4. 終了時に [docs/GOALS.md](docs/GOALS.md) の完了チェックを満たす

ハンズオン実施者は、使用する OpenShift / RHDH 環境を別途用意し、接続情報は参加者向けに当日共有してください（本リポジトリには書かない）。

## リポジトリ構成

```text
rhads-hands-on/
├── README.md
└── docs/
    ├── AGENDA.md
    ├── GOALS.md
    └── RHADS_OVERVIEW.md
```

## ライセンス・取り扱い

社内外でのハンズオン利用を想定した資料です。公開範囲は主催側のポリシーに従ってください。
