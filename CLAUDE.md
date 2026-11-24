# mathgame — 數學遊戲總專案

## 對話開始時請先讀
進度與最近更動都在 Obsidian：`mathgame/工作筆記.md`

## 工作模式
- **加新工具**：對 Claude 說「我想做一個 XXX 遊戲」→ Claude 會建 `tools/<工具名>/` 子資料夾並引導製作
- **結束工作**：對 Claude 說「**收工**」→ 自動 commit + push + 更新 Obsidian 工作筆記
- **接續工作**：對 Claude 說「**開工**」或「讀工作筆記、告訴我上次做到哪」

## 工作桌 + 三個家
- 📋 GDrive 工作桌：`H:\我的雲端硬碟\mathgame\`（自動跨電腦同步）
- 🐙 GitHub repo：`johnson611008/mathgame`（公開，網頁的家，GitHub Pages）
- 📘 Obsidian 駕駛艙：`mathgame/工作筆記.md`（想法的家）
- 🔥 Firebase 專案：（待指定，資料的家）

## 工具清單
（之後加新工具時會自動更新）
- （尚無）

## 工作注意事項
- 學生資料一律去識別化（只用座號 + 班級代號）
- commit 訊息要寫清楚做了什麼 + 為什麼
- 收工前說「收工」讓 Claude 同步三方
- `.claude/` 絕不 commit
