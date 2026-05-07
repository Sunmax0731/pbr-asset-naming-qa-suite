# 手動テスト

Codex 側では手動テスト未実施です。

## 作業ディレクトリ

`D:\AI\AdobePlugin\Substance3D\pbr-asset-naming-qa-suite`

## 必要ファイル

- `package.json`
- `samples/representative-suite.json`
- `src/product-profile/profile.json`
- `src/adobe/`
- `docs/release-checklist.md`

## セットアップ手順

1. 作業ディレクトリ `D:\AI\AdobePlugin\Substance3D\pbr-asset-naming-qa-suite` で `npm test` を実行します。
2. 対象ホストは `Substance3D` です。推定根拠は README と `docs/source-idea-pack.json` を参照します。
3. Adobe UXP Developer Tool または対象ホストのスクリプト読み込み機能で `src/adobe` を読み込みます。
4. パネルまたはスクリプトの検品結果がサンプルと同じ分類になることを確認します。

## 実施手順

1. `npm test` が通ることを確認する。
2. `node src/cli/index.js samples/representative-suite.json` を実行する。
3. 出力された Markdown レポートで4シナリオの分類を確認する。
4. Substance3D のホスト上で panel または script shell が読み込めることを確認する。

## 期待結果

- happy-path は pass。
- missing-required は fail。
- warning は warning。
- mixed-batch は pass 1、warning 1、fail 1。
- docs ZIP が `dist/pbr-asset-naming-qa-suite-docs.zip` に存在する。

## 未実施の手動確認項目

- 実ホスト上の表示確認
- 実データでの分類妥当性確認
- BOOTHまたはChrome Web Store向け説明文の最終確認
- ユーザー環境でのインストール手順確認

