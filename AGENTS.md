# AGENTS

この repo は `pbr-asset-naming-qa-suite` の closed alpha 実装単位です。

## Scope

- Root: `D:\AI\AdobePlugin\Substance3D\pbr-asset-naming-qa-suite`
- Domain: AdobePlugin
- Product kind: adobe-plugin
- Source pack: `D:/AI/AdobePlugin/created_idea_008_pbr-asset-naming-qa-suite/idea_008_pbr-asset-naming-qa-suite.zip`
- Public repo: `https://github.com/Sunmax0731/pbr-asset-naming-qa-suite`

## Working Rules

- README、AGENTS、SKILL、docs を同じ変更単位で更新する。
- created_idea は `D:/AI/AdobePlugin/created_idea_008_pbr-asset-naming-qa-suite` を正とし、同梱 ZIP の `metadata.json` と repo 名が一致することを確認する。
- ZIPサイズや生成時刻のように揺れる値を QCDS の固定評価根拠にしない。
- mojibake 判定は `npm test` 内の `scripts/check-mojibake.js` で行う。
- 手動テストは Codex では実施しない。未実施項目を docs に残して release notes にも転記する。
- 作業ブランチは `codex/closed-alpha-release` の1本だけを使い、完了後にローカル/リモートから削除する。

