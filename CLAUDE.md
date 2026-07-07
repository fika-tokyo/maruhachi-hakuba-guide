# CLAUDE.md — はたご丸八 現地ガイドサイト

## このリポジトリは何か
はたご丸八（白馬）の**宿泊者向け現地ガイド**サイト。素のHTML（フレームワーク無し）。
公式サイトとは別物で、宿泊者に向けた情報表示ページ。

## 公開とデプロイ（最重要）
- ホスティング = **GitHub Pages**。公開URL: https://fika-tokyo.github.io/maruhachi-hakuba-guide/
- リポジトリ: https://github.com/fika-tokyo/maruhachi-hakuba-guide
- pushアカウント: **Tsugaike-fika**（編集権限付与済み）
- **main ブランチに push すると、1〜2分で自動的に本番サイトへ反映**される
- ⚠ 旧 **Netlify版はもう使わない**。Netlifyには触らない・デプロイしない。更新はこのGitHubリポジトリだけで行う

## ファイル構成
日本語ページと英語ページが**別ファイル**になっている（全7ページ）：

| 内容 | 日本語 | 英語 |
|---|---|---|
| トップ | index.html（日英トグル併記） | （同左） |
| 宿泊案内 | stay.html | stay-en.html |
| 白馬ガイド | hakuba.html | hakuba-en.html |
| グリーンシーズン詳細 | green-season.html | green-season-en.html |

- `images/` … サイト内で使う画像（相対パス `images/xxx.jpg` で参照）
- CSS/JS は基本的に各HTML内に直書き
- `dog-consent.pdf`, `dog-rules.pdf`, `cake-price.pdf` … 宿泊者向け添付資料

## 編集時のルール
- ⚠ **日本語ページを直したら、対応する英語ページ（-en.html）も必ず直す**（逆も同様）。片方だけ直すと言語切替で内容が食い違う
- 画像を足すときは `images/` に置き、相対パスで参照する
- 編集が終わったら **commit → push**（= 自動で本番反映）

## ブランド・トーン
- はたご丸八のブランドに合わせたトーン
