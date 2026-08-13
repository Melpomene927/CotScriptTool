# CotScriptTool 版本摘要

本檔為**對外、玩家向**的 release notes 摘要，隨公開倉庫 [Melpomene927/CotScriptTool](https://github.com/Melpomene927/CotScriptTool) 的 `CHANGELOG.md` 同步。

- **完整開發紀錄**（含實作細節、內部路線圖）位於 mod 包內的 `develop.md`（§10 版本歷程），或私有維護 repo；公開 repo **不包含** CoT 原始碼目錄。
- **維護約定**：每次發布 CotScriptTool 時，在私有 CoT 更新本檔正本 `scripts/cot-script-tool-public-changelog.md`（新增對應版本小節），再執行 **CotScriptTool: Sync public docs (README + CHANGELOG)**（或 `scripts/sync_public_readme.ps1`）推至公開 repo。
- **表述原則**：對外摘要維持**全齡、中性**功能描述，不列露骨項目名稱或 18+ 行銷用語；細節僅見 mod 包 `develop.md`。

格式：新版本加在**表上方**（倒序）。

---

## 2.28.0

- **內建自定義服裝與預設套裝擴充**：新增多件 bundled 服裝與對應款式選項；內建自定義服裝預設 **90 → 104** 件，預設套裝 **309 → 315** 套。

---

## 2.27.2

- **安裝檔體積優化**：模組封裝流程改進，安裝檔案更小、下載更快，功能與前一版相同。

---

## 2.27.0

- **預設套裝改為疊加套用**：套用預設套裝到草裝時不再整批取代，而是依序疊加，方便組合多套穿搭（例如先套內衣、再疊加外出服、再疊加配件）。

---

## 2.26.0

- **預設套裝大幅擴充**：內建套裝由 62 套增加至 309 套，新增多種風格分類，選擇更豐富。

---

## 2.25.0

- **創作內容管理擴充**：美術／攝影作品與寫作書籍新增逐件檢視與調整，並提供批次一鍵操作，方便管理累積的創作成果。

---

## 2.24.0

- **「副業與社團」模組更名擴充**：整合直播、社團相關狀態管理；作弊面板精簡，移除重複的舊版狀態區塊。

---

## 2.23.0

- **新增「打工與社團」管理模組**：可集中檢視與調整打工、校隊等課餘生活相關狀態。

---

## 2.22.12

- **自定義服裝鞋類分層修正**：修復部分自定義鞋類服裝的分層判定問題。
- **玩家狀態面板調整**：技能顯示區分主要／次要技能，並新增特徵分頁。

---

## 2.22.11

- **自定義服裝 subs 編輯器**：sub 群組動作（從模板還原、從其他模板套用、清空、新增選項）移至 `sub-options` 區域頂部，與選項列同一區塊，操作更直覺。

---

## 2.22.10

- **內建自定義服裝預設擴充**：新增多件 bundled 服裝；內建自定義服裝預設 **80 → 90** 件。

---

## 2.22.9 — 2.22.7（精選）

- 自定義服裝 catalog 拆分與驗證修正；修飾符與 catalog 驗證改進。
- **選用原生服裝 config** catalog 擴充（201 → 205 件），供選用 runtime patch（預設關閉）。

---

## 2.22.6 — 2.22.0（精選）

- 自定義服裝管理器分類順序與選取器一致；斜挎包等 **wear style** 驗證修復。
- **Phase 7 Batch 3** 結案：bundled 自定義服裝 **65 → 73** 件；新增多套 preset-outfits。

---

## 2.21.x（精選）

- **跨存檔資源庫**：自定義服裝藍圖與已存套裝可存於 `localStorage`，跨存檔槽匯入匯出。
- **選用原生服裝 config** 大規模 catalog（選用開關）；pre-restore／bundled 早注入修復讀檔 crash。
- 預設套裝 picker UX 與編輯器模板／config 匯入改進。

---

## 2.20.x — 2.19.x（精選）

- **選用原生服裝 config**（CotScriptTool-only，作弊面板開關）。
- bundled 自定義服裝 **configurations 全件補齊**與 stale 升級修復；legacy 衣櫥遷移。
- **配件預設套裝**分類；preset-outfits 總量提升。

---

## 2.18.x — 2.14.x（精選）

- **原生＋自定義 preset-outfits** 大量新增（校園、約會、主題套裝 batch 等）。
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
- **外觀編輯、特殊道具、宿舍設備、卡牌**等獨立管理視窗。
- UI 統一（picker 主題、75vh 視窗、布局 localStorage、重置浮動視窗）。

更早版本的逐項修正請見 mod 包內 `develop.md` §10。
