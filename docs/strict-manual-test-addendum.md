# Strict Manual Test Addendum

Codex 側では手動テスト未実施です。

## 作業ディレクトリ

`D:\AI\AdobePlugin\Substance3D\pbr-asset-naming-qa-suite`

## 必要ファイル

- `samples/representative-suite.json`
- `src/product-profile/profile.json`
- `src/adobe/`
- `docs/manual-test.md`
- `dist/pbr-asset-naming-qa-suite-docs.zip`

## セットアップ手順

1. 作業ディレクトリ `D:\AI\AdobePlugin\Substance3D\pbr-asset-naming-qa-suite` で `npm test` を実行します。
2. 対象ホストは `Substance3D` です。推定根拠は README と `docs/source-idea-pack.json` を参照します。
3. Adobe UXP Developer Tool または対象ホストのスクリプト読み込み機能で `src/adobe` を読み込みます。
4. パネルまたはスクリプトの検品結果がサンプルと同じ分類になることを確認します。

## ローカルサーバーやホストアプリ起動手順

Substance3D と Adobe UXP Developer Tool または対象ホストのスクリプト実行機能を起動する。

## 実施手順

1. `npm test` を再実行する。
2. 実データ1件を `samples/representative-suite.json` と同じ形式で作成する。
3. CLIで検証する。
4. ホストUIまたは補助UIで表示する。
5. warning と fail の理由がユーザーに説明可能か確認する。

## 期待結果

- 自動テストが通る。
- docs ZIP が存在する。
- 実ホストまたは補助UIで最低1件の結果を確認できる。
- 未確認項目が release notes と一致する。

## 未実施の手動確認項目

- 実ホストUI表示
- 実素材/実ページ/実ファイルでの検査
- 配布導線のユーザー環境確認
- ストア/BOOTH向けスクリーンショット確認

