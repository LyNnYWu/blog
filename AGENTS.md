# AGENTS.md

本 repo 是 Lyndon 的公開個人部落格，使用 Hexo 建置並發布至 GitHub Pages。

## 入口與權威

- 網站設定：`_config.yml`、`_config.landscape.yml`
- 公開內容：`source/`
- 維護紀錄：`docs/MEMO_blog.md`
- 公開網站：`https://lynnywu.github.io/blog/`

## 公開內容界線

- 可公開教育、研究、專案管理、資料分析、自動化與交通安全的通用方法及個人經驗。
- 不公開學生個資、內部帳號、憑證、私有 repo 名稱、機隊架構、內部網址或可利用的安全細節。
- 尚未完成的文章須清楚標示「內容撰寫中」與預計涵蓋範圍，不得把骨架冒充完整文章。

## 日期排序

- 所有含日期的文章、清單、表格與紀錄，預設依距離現在由近到遠排列：最新在前、最舊在後。
- 首頁及 archive 使用倒序日期；同日內容以時間明確固定順序。

## 修改與驗證

- 修改前先 `git pull --ff-only`，並確認目前分支與工作樹。
- 內容更新後至少執行 `npm ci`、`npm run clean`、`npm run build`。
- 發布後須從公開 GitHub Pages 讀回主標、副標、文章入口與正確 canonical／OG URL，並檢查手機版無橫向溢出。
- 任務完成須更新 `docs/MEMO_blog.md`，只暫存本次修改檔案，commit、push 後以 `git ls-remote` 回驗 SHA。

## 共用記憶與交接

- 本 repo 已登錄於 `~/Desktop/repos/ops-lessons/docs/INDEX.md`。
- 跨專案通用教訓才寫入 `ops-lessons/docs/LESSONS.md`；部落格內容策略與發布狀態留在本 repo memo。
