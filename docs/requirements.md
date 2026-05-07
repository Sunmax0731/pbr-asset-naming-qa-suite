# 要件定義

## 目的

PBR素材検品・命名スイート は、PBR素材を制作、販売、Unity/Blenderへ渡す制作者 が PBRチャンネル、命名、解像度、用途、販売前チェックを同じ検品モデルにまとめる。

## Source

- PICKUP Rank: 52
- Domain / Idea No: AdobePlugin / 8
- Repository: pbr-asset-naming-qa-suite
- created_idea: `D:/AI/AdobePlugin/created_idea_008_pbr-asset-naming-qa-suite`
- ZIP: `D:/AI/AdobePlugin/created_idea_008_pbr-asset-naming-qa-suite/idea_008_pbr-asset-naming-qa-suite.zip`
- README確認: 開始時点では正式 repo が存在しないため、README.md は存在しない。

## Functional Requirements

- R1: materialName、channel、textureFile、namingRule を必須項目として検査する。
- R2: 必須項目不足は fail として分類する。
- R3: `nonStandardChannel` が true の場合は warning として分類し、手動確認理由を返す。
- R4: 複数アイテムの mixed-batch を pass / warning / fail に集計する。
- R5: 結果を CLI と docs/release evidence で再利用できる形にする。

## Non Functional Requirements

- UTF-8 で Markdown / JSON / JS / HTML / Python を保存する。
- 外部通信を既定で行わず、サンプルとローカル入力だけで検証できる。
- 手動テスト未実施であることを release 前 docs に明記する。

