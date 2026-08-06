# CotScriptTool 版本摘要

本檔為**對外、玩家向**的 release notes 摘要，隨公開倉庫 [Melpomene927/CotScriptTool](https://github.com/Melpomene927/CotScriptTool) 的 `CHANGELOG.md` 同步。

- **完整開發紀錄**（含實作細節、內部路線圖）位於 mod 包內的 `develop.md`（§10 版本歷程），或私有維護 repo；公開 repo **不包含** CoT 原始碼目錄。
- **維護約定**：每次發布 CotScriptTool 時，在私有 CoT 更新本檔正本 `scripts/cot-script-tool-public-changelog.md`（新增對應版本小節），再執行 **CotScriptTool: Sync public docs (README + CHANGELOG)**（或 `scripts/sync_public_readme.ps1`）推至公開 repo。

格式：新版本加在**表上方**（倒序）。

---

## 2.22.11

- **自定義服裝 subs 編輯器**：sub 群組動作（從模板還原、從其他模板套用、清空、新增選項）移至 `sub-options` 區域頂部，與選項列同一區塊，操作更直覺。

---

## 2.22.10

- **經典裸視洋裝擴充 +10**：新增多件紅毯／檔案致敬款 bundled 服裝；內建自定義服裝預設 **80 → 90** 件。

---

## 2.22.9 — 2.22.7（精選）

- **裸視洋裝**拆為多件獨立致敬款；修正 sheer 修飾符與 catalog 驗證。
- **原生暴露 config** catalog 擴充（201 → 205 件），供選用 runtime patch（預設關閉）。

---

## 2.22.6 — 2.22.0（精選）

- 自定義服裝管理器分類順序與選取器一致；斜挎包等 **wear style** 驗證修復。
- **Phase 7 Batch 3** 結案：bundled 暴露主題服裝 **65 → 73** 件；新增多套 preset-outfits。

---

## 2.21.x（精選）

- **跨存檔資源庫**：自定義服裝藍圖與已存套裝可存於 `localStorage`，跨存檔槽匯入匯出。
- **原生暴露 config** 大規模 catalog（選用開關）；pre-restore／bundled 早注入修復讀檔 crash。
- 預設套裝 picker UX 與編輯器模板／config 匯入改進。

---

## 2.20.x — 2.19.x（精選）

- **原生服裝暴露 configurations**（CotScriptTool-only，作弊面板開關）。
- bundled 自定義服裝 **configurations 全件補齊**與 stale 升級修復；legacy 衣櫥遷移。
- **配件預設套裝**分類；preset-outfits 總量提升。

---

## 2.18.x — 2.14.x（精選）

- **原生＋自定義 preset-outfits** 大量新增（校園、約會、暴露主題 batch 等）。
- configurations 稽核 P0／P1 結案；**Phase 7 Batch 1–2** bundled 擴充。
- 衣櫥 meta／tag 顯示、Wardrobe 相關 bypass 改 runtime hook（減少 TweeReplacer 依賴）。

---

## 2.13.x — 2.11.x（精選）

- **預設套裝**建置管線（`preset-outfits` → 套裝編輯器 📋 匯入）。
- **自定義服裝**模組上線：編輯器、JSON IO、內建 bundled 預設、pre-restore 讀檔修復。
- 對齊 CotCheatMod 部分能力（作弊面板、時間快轉、事件／NPC 工具）；**玩家狀態**獨立視窗。

---

## 2.10.x 及更早（精選）

- 模組化 **Tampermonkey → ModLoader** 打包；浮動 🧪 工具箱、服裝／套裝／物品 picker。
- **穿環、紋身、化妝、毛髮、卡牌、情趣物品、宿舍設備**等獨立管理視窗。
- UI 統一（picker 主題、75vh 視窗、布局 localStorage、重置浮動視窗）。

更早版本的逐項修正請見 mod 包內 `develop.md` §10。
