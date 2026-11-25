# mathgame — 數學遊戲總專案

## 專案定位
- 本專案是**主專案**，專門製作各式各樣與數學有關的遊戲。
- 每個遊戲都是附屬於主專案的**子專案**，放在 `games/<遊戲英文名>/`（小寫加連字號）。
- 每個子專案各自獨立：有自己的 `index.html`（入口）與 `README.md`（年級、學習目標、玩法）。
- 主專案根目錄的 `index.html` 是遊戲大廳，列出所有遊戲連結。
- 全部遊戲共用同一個 repo 與 GitHub Pages：`https://johnson611008.github.io/mathgame/games/<遊戲名>/`

## 對話開始時請先讀
進度與最近更動都在 Obsidian：`mathgame/工作筆記.md`

## 工作模式
- **加新遊戲**：對 Claude 說「我想做一個 XXX 遊戲」→ Claude 會建 `games/<遊戲名>/` 子專案、更新大廳與遊戲清單
- **結束工作**：對 Claude 說「**收工**」→ 自動 commit + push + 更新 Obsidian 工作筆記
- **接續工作**：對 Claude 說「**開工**」或「讀工作筆記、告訴我上次做到哪」

## 工作桌 + 三個家
- 📋 GDrive 工作桌：`H:\我的雲端硬碟\mathgame\`（自動跨電腦同步）
- 🐙 GitHub repo：`johnson611008/mathgame`（公開，網頁的家，GitHub Pages）
- 📘 Obsidian 駕駛艙：`mathgame/工作筆記.md`（想法的家）
- 🔥 Firebase 專案：（待指定，資料的家）

## 遊戲清單
（之後加新遊戲時會自動更新，並同步更新大廳 index.html）
- （尚無）

## 數學式顯示規範
- 方程式、分數、根號等數學式一律用 **LaTeX 語法** 撰寫，以 **KaTeX** 渲染（不用 MathJax、不用純文字或圖片）。
- 行內數學式用 `\( ... \)`，獨立一行用 `$$ ... $$`（KaTeX auto-render）。
- 程式動態產生的題目用 `katex.render(latex, element)` 顯示。
- KaTeX 版本統一用 `katex@0.16.11`（jsDelivr CDN）；需離線使用時改放本地檔案。
- 使用臺灣常用數學符號（例：乘號 `\times`、除號 `\div`）。

## 工作注意事項
- 學生資料一律去識別化（只用座號 + 班級代號）
- commit 訊息要寫清楚做了什麼 + 為什麼
- 收工前說「收工」讓 Claude 同步三方
- `.claude/` 絕不 commit
