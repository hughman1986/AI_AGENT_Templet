# README

本範本包含：

* `AGENTS.md`
* `memory-bank/` 五個核心文件
* `templates/` 候選技術範例（未核准，不會自動生效）

本文件僅說明「開發者需要做的事情」。

參考: [Ultimate Guide to Vibe Coding](https://github.com/EnzeD/vibe-coding.git)

---

# 一、初始化專案

1️⃣ 將 `AGENTS.md` 放在專案根目錄。

2️⃣ 建立資料夾：

```
memory-bank/
```

3️⃣ 在 memory-bank 內建立五個檔案：

* `game-design-document.md`
* `tech-stack.md`
* `architecture.md`
* `implementation-plan.md`
* `progress.md`

可直接複製本儲存庫的五份文件。`architecture.md`、`progress.md` 與計畫中的「本儲存庫維護任務」含本樣板的維護紀錄；套用新專案時清除或替換，保留欄位結構。

---

# 二、實際使用步驟

### Step 1 – 撰寫專案願景

填寫 `game-design-document.md`：

* 問題定義
* 預期成果
* Out of Scope

---

### Step 2 – 確認技術棧

填寫 `tech-stack.md`：

* 使用技術
* 套件政策
* 安全與效能要求

需要範例時參考 `templates/tech-stack-dotnet.md` 或 `templates/tech-stack-python.md`，只將已確認內容整理至 `memory-bank/tech-stack.md`。不要將候選檔放進 memory-bank，也不要把範例中的套件、安全方案或效能數字當成核准需求。記錄核准來源；效能門檻需包含環境、資料量與量測方式。未知項目標示「待確認」，不適用項目明確註明。

---

### Step 3 – 規劃第一個可運行步驟

填寫 `implementation-plan.md`：

* 第一個可完成的小功能
* 可驗證成果

只規劃「下一步」，不要規劃整個未來。

---

### Step 4 – 開發與測試

* 執行當前步驟
* 確認功能可運行
* 執行相關自動化測試，記錄命令、實際結果與未驗證項目
* 無法自動化時，記錄原因、人工驗證證據與後續補測需求

---

### Step 5 – 更新進度

完成一個可運行功能後：

* 更新 `progress.md`
* 在 `implementation-plan.md` 更新任務狀態與驗收結果
* 若系統結構改變，再更新 `architecture.md`

`progress.md` 保留目前狀態、最近證據、阻礙與下一步，避免複製完整任務清單；壓縮過時紀錄時保留未解阻礙與測試例外，歷史由版本控制保存。架構文件只記錄已實作結構，提案留在計畫中。

---

# 文件最小填寫門檻（Minimum Required Before Coding）

開始開發前，至少完成以下內容：

* `game-design-document.md`：填寫「問題定義」、「主要成果」、「可量化成功標準」、「Out of Scope」
* `tech-stack.md`：確認使用技術與依賴政策
* `implementation-plan.md`：至少填完「任務 1」（目標 / 交付成果 / 驗收條件 / 自動化測試方式 / 狀態）

若以上與當前任務相關的必要資訊未完成，先依既有專案與已授權決策補齊；涉及未決產品行為、資料語意、架構或新依賴時，先釐清再進行相依實作。局部實作可沿用既有程式與測試慣例，不必為無關欄位阻擋工作，也不可捏造內容填滿文件。

---

# 三、使用原則

* 每次只做一個小步驟
* 每次都要可運行
* 文件必須反映實際狀態
* 不做過度預測規劃

---

# 快捷提示（CLI Intent Shortcuts）

* `status`：摘要目前狀態
* `next`：執行下一個最小有意義步驟
* `fix`：重現問題、實作最小修正並執行回歸測試；受阻時回報證據與缺少的前提
* `optimize`：在不改變行為下改善效能
* `refactor`：在不改變行為下改善結構

---

# 核心循環

Outcome → Small Step → Test → Update → Repeat
