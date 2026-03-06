# README

本範本包含：

* `AGENTS.md`
* `memory-bank/` 五個核心文件

本文件僅說明「開發者需要做的事情」。

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

---

### Step 5 – 更新進度

完成一個可運行功能後：

* 更新 `progress.md`
* 若系統結構改變，再更新 `architecture.md`

---

# 文件最小填寫門檻（Minimum Required Before Coding）

開始開發前，至少完成以下內容：

* `game-design-document.md`：填寫「問題定義」、「主要成果」、「可量化成功標準」、「Out of Scope」
* `tech-stack.md`：確認使用技術與依賴政策
* `implementation-plan.md`：至少填完「任務 1」（目標 / 交付成果 / 測試方式 / 狀態）

若以上未完成，先補文件再開始實作，避免方向漂移與重工。

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
* `fix`：分析錯誤並提出最小修正

---

# 核心循環

Outcome → Small Step → Test → Update → Repeat
