# 引き継ぎドキュメント — SavannaSite（共有インフラ）

> 別のAIがこのプロジェクトを引き継ぐための現状サマリ。最終更新: 2026-06-29

---

## 1. 概要

- これは個別アプリではなく、**Savannaブランド全アプリ共通の GitHub Pages サイト**。
- 各アプリの App Store 審査に必須の **プライバシーポリシー / サポートページ** をホスティングする。
- 公開アカウント: GitHub `savanna1043` のリポジトリ（GitHub Pages）。

## 2. 現在の構成

```
index.html              # トップ
kanzo-kun/privacy.html  # 肝臓くんと減酒
kanzo-kun/support.html
oshi-log/privacy.html   # 推しログ
oshi-log/support.html
```

## 3. ステータス & TODO ⭐

- **肝臓くん・推しログ** のページは掲載済み。
- **⚠ ペタログ(petalog) のページが未作成** — App Store提出前に `petalog/privacy.html`・`support.html` を追加する必要あり。
- **⚠ ふりログ(furilog) のページが未掲載** — HTMLは `FuriLog/release/privacy_policy_ja.html`・`support_page_ja.html` に作成済み。これを `furilog/` ディレクトリにコピーして公開する。
- ページ追加後、各アプリの App Store Connect「Appのプライバシー」にURLを設定する。

## 4. 運用方針

- 新アプリをリリースするたびに `<app-slug>/privacy.html` と `support.html` を追加する運用（数十アプリ量産前提のため雛形を使い回す）。
- スラッグはハイフン区切り（例: `kanzo-kun`, `oshi-log`）。

## 5. 関連アプリ

肝臓くん(iOSAPP) / 推しログ(OshiApp) / ペタログ(PetaLog) / ふりログ(FuriLog)。各フォルダの `HANDOFF.md` 参照。
