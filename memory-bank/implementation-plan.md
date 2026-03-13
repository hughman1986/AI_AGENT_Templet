## 📌 迭代策略（Iteration Strategy）

* 部署頻率：每完成一個可運行功能即本機部署測試（Continuous Local Deployment）
* 完成定義（Definition of Done）：
	* 功能可正常執行且無阻斷性錯誤
	* 通過基本單元測試
	* 無未處理例外（Unhandled Exception）
	* 已更新 progress.md
	* 不破壞既有功能（No Regression）

## 🧩 任務拆解（Task Breakdown）

> 說明（Hint）：
> * `目標（Goal）`：描述這個大任務要解決的問題或想達成的結果，聚焦「為什麼做」。
> * `交付成果（Deliverable）`：描述完成後實際會產出的功能、模組、流程或頁面，聚焦「做完會看到什麼」。
> * 建議寫法：
>   * 目標：讓[誰/哪個系統]可以[完成什麼事]，以解決[什麼問題]
>   * 交付成果：完成[功能/模組 A]、[功能/模組 B]、[流程/頁面/API C]
>
> 範例（Example）：
> ### 大任務範例：建立登入功能
> * 目標（Goal）：讓使用者可以安全登入系統，進入受保護功能
> * 交付成果（Deliverable）：完成登入頁、帳密驗證流程、登入成功後導向主畫面
> * 狀態（Status）：Todo / Doing / Done / Blocked
>
> 小任務（Checklist）：
> - [ ] 建立登入頁 UI
> - [ ] 串接帳號密碼驗證
> - [ ] 登入成功後導向主畫面
>
> 驗證方式（Test Method）：
> * 輸入正確帳密可登入，錯誤帳密會顯示錯誤訊息

### 大任務 1：<名稱>
* 目標（Goal）：
* 交付成果（Deliverable）：
* 狀態（Status）：Todo / Doing / Done / Blocked

小任務（Checklist）：
- [ ] 小任務 1
- [ ] 小任務 2
- [ ] 小任務 3

驗證方式（Test Method）：
* 

### 大任務 2：<名稱>
* 目標（Goal）：
* 交付成果（Deliverable）：
* 狀態（Status）：Todo / Doing / Done / Blocked

小任務（Checklist）：
- [ ] 小任務 1
- [ ] 小任務 2

驗證方式（Test Method）：
* 





## 🧪 測試策略（Testing Strategy）
* 測試層級（Test Levels）：
  * 單元測試（Unit Tests）: xUnit + FluentAssertions
  * 整合測試（Integration Tests）: Testcontainers（PostgreSQL）
  * 端到端 / API 測試（E2E / API Tests）: Postman / REST Client
* 驗收標準（Acceptance Criteria）：
  * 核心流程可通過驗收案例
  * 關鍵錯誤路徑有覆蓋
  * 無阻斷性回歸（No Blocking Regression）
* 需要手動測試時請提示 


## ⚠️ 風險紀錄（Risk Log）
* 風險項目（Risk Item）：
  * 風險描述（Description）：
  * 影響程度（Impact: High/Medium/Low）：
  * 緩解方案（Mitigation）：
  * 目前狀態（Status: Open/Mitigated/Closed）：

