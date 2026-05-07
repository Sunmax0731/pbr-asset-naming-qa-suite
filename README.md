# PBR素材検品・命名スイート

pbr-asset-naming-qa-suite は PBR素材を制作、販売、Unity/Blenderへ渡す制作者 向けの closed alpha プロダクトです。PBRチャンネル、命名、解像度、用途、販売前チェックを同じ検品モデルにまとめる。

## Source

- PICKUP Rank: 52
- Domain / Idea No: AdobePlugin / 8
- Repository: pbr-asset-naming-qa-suite
- 主な公開先: BOOTH / GitHub Release
- created_idea: `D:/AI/AdobePlugin/created_idea_008_pbr-asset-naming-qa-suite`
- 同梱ZIP: `D:/AI/AdobePlugin/created_idea_008_pbr-asset-naming-qa-suite/idea_008_pbr-asset-naming-qa-suite.zip`
- 開始時 README: 存在しない
- Adobe host: Substance3D
- Host inference: PBR素材の命名、チャンネル、テクスチャセット検品はSubstance 3D系制作フローに最も近いため。

## Alpha Scope

- 代表シナリオ4件の自動検証
- 必須項目不足、警告、混在バッチの分類
- src/adobe/ のホスト連携シェル
- QCDS、security/privacy、traceability、release checklist、manual test docs
- docs ZIP: `dist/pbr-asset-naming-qa-suite-docs.zip`

## Commands

```powershell
npm test
node src/cli/index.js samples/representative-suite.json
npm run build:docs
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` にあります。

