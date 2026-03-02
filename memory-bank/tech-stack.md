## 🏗 核准技術棧（Approved Tech Stack）

### 後端（Backend）

* 語言：C#
* 框架：.NET
* 執行環境版本：.NET 8.0
* 常見搭配（Common Integrations）：
  * ORM：Entity Framework Core 8
  * 輕量資料存取：Dapper
  * PostgreSQL Driver：Npgsql
  * 驗證框架：FluentValidation
  * 日誌框架：Serilog
  * 依賴注入：內建 DI Container

### 桌面應用程式（Desktop Application）

* UI 框架：WinForms / WPF（依專案選擇）
* 架構模式：MVVM（若使用 WPF）
* UI 元件庫：依專案需求評估
* 狀態管理：ViewModel / 事件驅動模式

### 資料庫（Database）

* 引擎：PostgreSQL
* 版本：17.x（或依實際環境指定）

### 基礎設施（Infrastructure）

* 開發環境：Windows 11
* IDE：Visual Studio 2022

## 📦 套件使用政策（Dependency Policy）

* 允許套件原則（Allowed Criteria）：
  * 僅使用活躍維護（Active Maintenance）且有穩定版本的套件。
  * 優先選擇 .NET 官方或社群主流套件。
  * 必須相容 .NET 8.0。
  * 不得引入高風險或無維護之第三方套件。

* 禁止類型（Disallowed Categories）：
  * 已停止維護（Deprecated）套件。
  * 無明確授權（License 不明）套件。
  * 會強制綁定商業授權之套件（除非經批准）。

* 新增套件審核流程（Approval Process）：
  1. 說明引入目的與替代方案比較。
  2. 評估安全風險與維護狀態。
  3. 記錄於 `tech-stack.md`。
  4. 經專案負責人批准後方可使用。

## 🔐 安全與合規需求（Security & Compliance Requirements）

* 身分驗證方式（Authentication Method）：
  * 桌面應用程式以 Windows 身分驗證（Windows Authentication）為主。
  * 若需帳密驗證，必須使用安全雜湊（例如 BCrypt）。

* 授權模型（Authorization Model）：
  * 基於角色存取控制（RBAC）。
  * 不允許前端單獨控制權限判斷。
  
* 資料保護規範（Data Protection Rules）：
  * 不得以明文儲存敏感資料。
  * 必須使用參數化查詢（Parameterized Query）避免 SQL Injection。
  * 日誌不得記錄敏感資訊。

## ⚡ 效能基準（Performance Baseline）

* 預期回應時間（Expected Response Time）：
  * 本機資料查詢 < 200ms。

* 最大可接受延遲（Max Acceptable Latency）：
  * 重型查詢或批次處理 < 2 秒。

* 吞吐量目標（Throughput Target）：
  * 支援單機同時 10–20 個操作流程無明顯效能下降。
