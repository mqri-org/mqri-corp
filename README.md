# mqri-corp

MQRI（一般社団法人 松石量子再生研究所）コーポレートサイト。

## Domain
- 本番: www.mqri.or.jp（Vercel経由で配信予定）

## v1 構成
静的HTMLによる最小構成。

| ページ        | パス            | ファイル        |
| ------------- | --------------- | --------------- |
| トップ        | `/`             | `index.html`    |
| お問い合わせ  | `/contact`      | `contact.html`  |

`vercel.json` で `cleanUrls: true` を有効化しており、`.html` は付与しないURLで配信されます。

## ローカルプレビュー
```bash
# 任意の静的サーバでOK
python3 -m http.server 8000
# → http://localhost:8000
```

## デプロイ（Vercel）
1. Vercel ダッシュボードで本リポジトリ `mqri-org/mqri-corp` をインポート
2. Framework Preset は **Other**（自動検出）
3. Build Command / Output Directory は **未設定（空）**
4. Root Directory は **`./`**
5. main へのマージで自動デプロイ

## ディレクトリ
```
.
├── index.html      # トップページ
├── contact.html    # 問い合わせ
├── vercel.json     # cleanUrls 設定
└── README.md
```

## Status
v1 公開準備中
