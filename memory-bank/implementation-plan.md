## 📌 迭代策略（Iteration Strategy）

* 部署頻率：每完成一個可運行功能即本機部署測試（Continuous Local Deployment）
* 完成定義（Definition of Done）：
	* 功能可正常執行且無阻斷性錯誤
	* 通過與變更相關的自動化測試及任務驗收條件；測試例外須記錄原因、人工驗證與後續補測
	* 無未處理例外（Unhandled Exception）
	* 已更新 progress.md
	* 不破壞既有功能（No Regression）
	* 在 progress.md 記錄驗證命令、實際結果與未驗證項目

任務狀態以本檔為準。Doing 表示進行中；Blocked 須記錄阻礙；Done 須有驗收證據。只細化下一個有意義步驟，後續任務可暫列目標；範例與空白欄位不代表已核准需求。

## 🧩 任務拆解（Task Breakdown）

> 說明（Hint）：
> * `目標（Goal）`：描述這個大任務要解決的問題或想達成的結果，聚焦「為什麼做」。
> * `交付成果（Deliverable）`：描述完成後實際會產出的功能、模組、流程或頁面，聚焦「做完會看到什麼」。
> * `任務複雜度提示（Complexity Hint）`：快速判斷執行任務時應優先使用哪一類模型。
>   * `Simple`：單一且明確的步驟、低風險、少量檔案變更；優先使用簡單模型。
>   * `Medium`：涉及多個檔案，或需要基本分析與驗證；依任務上下文選擇模型。
>   * `Complex`：跨模組或架構、需求不明、風險高，或需要多輪驗證；優先使用複雜模型。
> * 建議寫法：
>   * 目標：讓[誰/哪個系統]可以[完成什麼事]，以解決[什麼問題]
>   * 交付成果：完成[功能/模組 A]、[功能/模組 B]、[流程/頁面/API C]
>
> 範例（Example）：
> ### 大任務範例：建立登入功能
> * 目標（Goal）：讓使用者可以安全登入系統，進入受保護功能
> * 交付成果（Deliverable）：完成登入頁、帳密驗證流程、登入成功後導向主畫面
> * 任務複雜度提示（Complexity Hint）：Medium
> * 狀態（Status）：Todo / Doing / Done / Blocked
>
> 小任務（Checklist）：
> - [ ] 建立登入頁 UI
> - [ ] 串接帳號密碼驗證
> - [ ] 登入成功後導向主畫面
>
> 驗證方式（Test Method）：
> * 輸入正確帳密可登入，錯誤帳密會顯示錯誤訊息
> * 自動化測試：覆蓋正確帳密、錯誤帳密與未登入存取受保護資源；填入實際測試位置及命令
> * 驗收結果：執行後填寫，證據記錄於 progress.md

### 大任務 1：<名稱>
* 目標（Goal）：
* 交付成果（Deliverable）：
* 任務複雜度提示（Complexity Hint）：Simple / Medium / Complex
* 狀態（Status）：Todo / Doing / Done / Blocked

小任務（Checklist）：
- [ ] 小任務 1
- [ ] 小任務 2
- [ ] 小任務 3

驗證方式（Test Method）：
* 驗收條件（可觀察的成功 / 錯誤行為）：
* 自動化測試位置與命令：
* 驗收結果 / 證據連結（執行後填寫）：
* 測試例外（若有，記錄於 progress.md）：

### 大任務 2：<名稱>
* 目標（Goal）：
* 交付成果（Deliverable）：
* 任務複雜度提示（Complexity Hint）：Simple / Medium / Complex
* 狀態（Status）：Todo / Doing / Done / Blocked

小任務（Checklist）：
- [ ] 小任務 1
- [ ] 小任務 2

驗證方式（Test Method）：
* 驗收條件：
* 自動化測試位置與命令：
* 驗收結果 / 證據連結（執行後填寫）：





## 🧪 測試策略（Testing Strategy）
* 測試層級（Test Levels）：
  * 單元測試（Unit Tests）：依核心邏輯與資料轉換需求選擇
  * 整合測試（Integration Tests）：依資料儲存與外部整合邊界選擇
  * 端到端 / API 測試（E2E / API Tests）：依使用者可見流程選擇
* 工具與共用命令：以 `tech-stack.md` 已核准設定為準，不預設新增測試套件
* 驗收標準（Acceptance Criteria）：
  * 核心流程可通過驗收案例
  * 關鍵錯誤路徑有覆蓋
  * 無阻斷性回歸（No Blocking Regression）
* 人工操作案例不等於自動化測試；需要手動測試時說明原因與步驟
* 純文件調整可使用結構、引用與差異檢查，無須為此新增測試框架

## 本儲存庫維護任務（套用新專案時移除）

* 任務：治理樣板一致性調整（2026-09-13）
* 目標 / 交付成果：分離候選設定、補齊交接欄位、統一決策與驗收規則。
* 狀態：Done
* 驗收條件：memory-bank 僅五份核心文件；候選範例標明未核准；正式設定不預選技術；README 與 AGENTS 的 fix 語意一致。
* 驗證方式：PowerShell 文件結構與必要內容斷言、`git diff --check`。
* 驗收結果：文件結構與必要內容斷言、差異檢查皆通過，詳見 `progress.md`。


## ⚠️ 風險紀錄（Risk Log）
* 風險項目（Risk Item）：
  * 風險描述（Description）：
  * 影響程度（Impact: High/Medium/Low）：
  * 緩解方案（Mitigation）：
  * 目前狀態（Status: Open/Mitigated/Closed）：

