# 小鯨魚娘 · Whale Girl Pet

深藍色長髮、鯨魚尾同側鰭嘅 Q 版女僕小鯨魚。呢個公開素材包包含完整透明動畫圖、九種狀態動畫，以及 16 個望向周圍嘅方向姿勢。

![小鯨魚娘九種動作](previews/motion.gif)

## 下載

- **[完整素材包 ZIP](https://github.com/makcheunghei/whale-girl-pet/releases/download/v1.0.0/whale-girl-pet-v1.0.0.zip)** — 動畫圖、逐狀態預覽、影片及格式說明。
- **[透明動畫圖 PNG](https://github.com/makcheunghei/whale-girl-pet/releases/download/v1.0.0/whale-girl-v2.png)** — `1536 × 2288`，完整 v2 sprite sheet。
- [動畫影片 MP4](https://github.com/makcheunghei/whale-girl-pet/releases/download/v1.0.0/whale-girl-motion.mp4)
- [Release 頁面](https://github.com/makcheunghei/whale-girl-pet/releases/tag/v1.0.0)

直接瀏覽：[全部姿勢](previews/contact-sheet.png) · [16 個方向](previews/directions.png) · [四個時間點嘅預覽](previews/motion-stills.png)

## 新版動畫

- 長髮同尾巴收近身體，預留安全邊距，保持每個姿勢完整。
- 左右移動分別面向正確方向，加入交替步姿。
- 待機有呼吸及眨眼；另外包含揮手、失敗、等待輸入、思考及檢查動作。
- 跳躍包含準備、蹲低、騰空、下降及落地。
- 身體比例、腳底位置及方向列之間嘅大小已統一。

素材由 AI 輔助生成，再作逐格提取、排列、比例對齊及驗證。

## 動畫圖格式

| 項目 | 數值 |
| --- | --- |
| 檔案 | `assets/whale-girl-v2.png` |
| 格式 | PNG，透明背景 |
| 版本 | Sprite sheet v2 |
| 整張尺寸 | 1536 × 2288 px |
| 每格尺寸 | 192 × 208 px |
| 排列 | 8 欄 × 11 列 |
| 使用中嘅格 | 73 |
| 留空透明格 | 15 |

每列由最左邊開始放置有效姿勢。以下列號由 **0** 開始：

| 列 | 狀態 | 格數 | GIF 預覽 |
| --- | --- | ---: | --- |
| 0 | 待機 `idle` | 6 | [查看](previews/states/idle.gif) |
| 1 | 向右移動 `running-right` | 8 | [查看](previews/states/running-right.gif) |
| 2 | 向左移動 `running-left` | 8 | [查看](previews/states/running-left.gif) |
| 3 | 揮手 `waving` | 4 | [查看](previews/states/waving.gif) |
| 4 | 跳躍 `jumping` | 5 | [查看](previews/states/jumping.gif) |
| 5 | 失敗 `failed` | 8 | [查看](previews/states/failed.gif) |
| 6 | 等待輸入 `waiting` | 6 | [查看](previews/states/waiting.gif) |
| 7 | 思考／處理工作 `running` | 6 | [查看](previews/states/running.gif) |
| 8 | 檢查 `review` | 6 | [查看](previews/states/review.gif) |
| 9 | 望向周圍，000°–157.5° | 8 | [查看完整方向循環](previews/look.gif) |
| 10 | 望向周圍，180°–337.5° | 8 | [查看完整方向循環](previews/look.gif) |

方向使用畫面座標：**000° 向上、090° 向右、180° 向下、270° 向左**，每格順時針增加 22.5°。`running` 代表處理工作時嘅思考動作。

## 使用素材

1. 下載完整 PNG，保留原有尺寸及透明背景。
2. 使用支援上述 v2 格式嘅動畫工具，按每格 `192 × 208` 提取姿勢。
3. 各狀態只讀取表中指定格數，跳過該列其餘透明格。
4. 如需格式資料，可讀取 [pet.json](pet.json)。

GIF／MP4 係方便瀏覽嘅動畫示範；完整可用素材係 PNG。實際播放節奏會由使用素材嘅程式決定。

## 驗證摘要

- 所有 73 格通過尺寸、透明背景及格位驗證。
- 跳躍最高離地 **36 px**；落地同待機腳底位置差 **1 px**。
- 四個主方向、全身完整度及兩列方向姿勢嘅比例通過獨立視覺審查。
- 部分相鄰斜角嘅轉頭幅度較細，保留視覺審查提示。
- 詳細數值及檔案 SHA-256：[validation.json](validation.json)。

![待機到跳躍再返回待機](previews/idle-jump.gif)
