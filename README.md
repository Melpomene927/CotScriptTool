# CotScriptTool

**CotScriptTool** 是《Course of Temptation（誘惑之課）》的 **ModLoader 輔助模組**，在遊戲內提供浮動工具箱：作弊調整、服裝／物品管理、套裝編輯、外觀與狀態編輯等。本倉庫**僅提供 Releases 下載**（`.mod.zip`），不含原始碼或建置腳本。

> 版本更新摘要請見 **[CHANGELOG.md](./CHANGELOG.md)**。各 Release 頁面亦會列出 ModLoader 依賴版本。

---

## 簡介

CotScriptTool 將常用調試與便利功能整合在單一 Mod 中，介面以繁體中文為主（需搭配 **ModI18N** 等中文 mod 時，遊戲內文案與標籤會更完整）。設計上盡量**不直接破壞存檔結構**：多數操作可逆，但仍建議在重要存檔前自行備份。

---

## 主要功能

| 區塊 | 說明 |
| --- | --- |
| **作弊面板** | 時間快轉、各類開關、事件瀏覽、NPC 關係、劇情相關工具等 |
| **玩家狀態** | 現金、需求、技能、身材、聲望、癖好、學業等集中編輯 |
| **服裝選取／穿著／衣櫥** | 依分類瀏覽原生服裝、篩選、詳情、穿上／存放、覆蓋部位檢視 |
| **套裝編輯** | 草稿編輯、已存套裝載入、匯入／匯出 JSON、一鍵穿上／脫光至衣櫥 |
| **預設套裝** | 模組內建多套 preset（含校園、約會、配件等），可匯入套裝草稿 |
| **自定義服裝** | 以遊戲模板建立／編輯服裝藍圖，含內建預設服裝包、JSON 匯入匯出、跨存檔資源庫 |
| **物品選取** | 快速檢索並授予道具／消耗品等 |
| **特殊道具管理** | 管理遊戲內特殊類道具持有、新增與相關選項 |
| **宿舍設備** | 已持有 dorm 物品維護、可展示項目收藏 |
| **外觀編輯** | 穿環、紋身、化妝、毛髮等獨立管理視窗 |
| **卡牌（TCG）** | 收藏與卡片數量管理 |
| **地點傳送** | 依地圖列表跳轉 passage（含返回上一 passage） |
| **記憶模組（預存指令）** | 保存並執行常用 JavaScript 片段；浮動 🧪 右鍵可跑「當前 JS」 |
| **快速 JS** | 編輯器內嵌腳本編輯與執行，方便測試 |
| **浮動視窗** | 各面板可拖曳、縮放；支援一鍵重置所有視窗布局 |

部分進階選項（例如選用的原生服裝 config 擴充）預設關閉，可在作弊面板開關中啟用。

---

## 使用說明

### 前置需求

- 已安裝 **[ModLoader](https://github.com/Lyoko-Jeremie/sugarcube-2-ModLoader)**，版本建議 **^2.17.0**（與各 Release 說明一致；以 `boot.json` / Release notes 為準）。
- 遊戲本體需為 ModLoader 版 HTML（例如 `CourseOfTemptation-ModLoader-*.html`）。
- 中文介面建議一併啟用 **ModI18N**（或其他中文 mod），非必須但體驗較完整。

### 安裝步驟

1. 開啟本倉庫 **[Releases](https://github.com/Melpomene927/CotScriptTool/releases)**。
2. 下載對應版本的 **`CotScriptTool-{version}.mod.zip`**（勿解壓成散檔再手動拼目錄）。
3. 將 `.mod.zip` 放入 ModLoader 指定的 **Mod 目錄**（依你使用的 ModLoader 文件為準）。
4. 在 ModLoader 管理介面**啟用 CotScriptTool**，並確認依賴 **ModLoader** 已滿足版本要求。
5. 重新載入或啟動遊戲。

### 遊戲內如何開啟

1. 進入遊戲後，畫面**左下角**會出現浮動按鈕 **🧪**。
2. **左鍵 🧪**：若尚未開啟任何工具視窗，會開啟 **CoT 工具**首頁（功能列表）；若已有視窗，則切換全部 Cot 視窗的顯示／隱藏。
3. 從首頁進入 **🎮 作弊面板**、**👗 服裝選取**、**✏️ 自定義服裝** 等項目；各視窗標題列可拖曳移動、右下角可縮放。
4. **右鍵 🧪**：執行「記憶模組」中保存的當前 JavaScript（進階用途）。
5. 亦可透過開發者主控台呼叫 `CotTools.showCheatPanel()` 等 API（需已載入模組）。

作弊面板仍可從工具首頁進入；部分舊版 CotCheatMod 的側欄捷徑已移除，以本工具箱為主。

### 常見注意

- **備份存檔**：作弊、批量授予物品、時間快轉等仍可能改變遊戲進度，請自行備份 `.save` 或遊戲內存檔槽。
- **Mod 順序**：若與其他作弊／服裝 mod 並存，行為可能衝突；以單獨測試 CotScriptTool 為佳。
- **語系**：UI 字串以工具內建中文為主；服裝名稱、passage 內容仍依遊戲與 ModI18N。
- **更新**：安裝新版本前可關閉舊 mod zip，再啟用新 zip；詳細變更見 [CHANGELOG.md](./CHANGELOG.md) 與 Release 說明。

---

## 取得協助

- **問題與功能請求**：請在 [Melpomene927/CotScriptTool](https://github.com/Melpomene927/CotScriptTool) 使用 GitHub Issues（若已開放）。
- **版本歷程**：[CHANGELOG.md](./CHANGELOG.md)
