# 版本紀錄

## v1.0 – 初版上線（2026-11-01）
- GitHub Release：v1.0
- Cloudflare Version ID：e5963bc2
- 網址：https://portfolio.rlzdesign.workers.dev
- 內容：11 個 UIUX 專案 + Graphic 作品集
- 頁面：Page_Home / Page_UIUX / Page_Graphic / Page_WorkFile、UIUX_01_SDK ～ UIUX_07_SD
- 共用元件：Com_Nav / Com_Project_Head / Com_Project_Hero / Com_Project_Section / Com_ToTop
- 圖片：assets/ 共 277 張 webp（1x / 2x）

## v1.1 – PH 儲值拆分 UX / UI（2026-11-01，第一段）
- UIUX_01_SDK.dc.html 改名為 UIUX_01_SDK_UI.dc.html
- 新增 UIUX_01_SDK_UX.dc.html：舊版問題蒐集、舊版痛點分析、競品 / 相關資料搜集、痛點與解決方向、新版設計、改版成果；新首圖、新頭像（user3 / user4）
- 長流程圖可橫向拖曳 / 滑動（可視範圍 1600）
- UI 頁：標題改 ( UI )、新引言、Before & After 換圖、UIUX 區塊改名 Landscape、Design System 換兩張新圖
- Page_UIUX：兩張卡片改標題 / 說明 / 標籤，UX 卡新封面
- 全站載入進度條修正（不再卡在 0%）
- 刪除：UIUX_01_SDK.dc.html、assets/uiux_img_block1(-1x).webp、assets/game_img_block6(-1x).webp

## v1.2 – UX 頁補完、Work File 拆頁、全站優化（2026-11-14 ～ 11-15）

### UX 頁（UIUX_01_SDK_UX）
- 「競品 / 相關資料搜集」：更新 What I think？圖（gameux_img_block3-1）、派對卡訂閱獨立頁參考圖（gameux_img_block3-4）
- 「痛點與解決方向」：新增設計探索與測試圖（gameux_img_block4-2，含內部易用性測試）
- 「新版設計」：更新名詞說明 / 派對卡會員福利 / 會員等級圖（gameux_img_block5-4）
- 新增區塊「回顧：加入 GA 追蹤」：引言 + 5 張黑底格線卡片（01 痛點對應方式、02 GA 指標、03 事件與參數、04 指標公式、05 數據判讀），表格為 HTML
- 指標名稱統一為「訂閱頁購買率」；04 補上〔計算方式〕以使用者數計算
- 4 張更換過的圖片加上 ?v=2 避免快取舊圖
- 可拖曳流程圖改用共用樣式 .flow-scroll；拖曳改為整頁一組監聽，張數不再寫死

### UIUX 列表頁（Page_UIUX）
- UX 卡：新說明、標籤改為 #app #ux #資訊架構 #易用性測試 #GA4
- UI 卡：新說明、新增 #design token

### Work File
- 導覽列 WORK FILE 改為下拉選單：Experience / About Me
- Page_WorkFile.dc.html 改名為 WorkFile_Experience.dc.html（標題改為 Experience）；舊網址失效
- 新增 WorkFile_AboutMe.dc.html：長篇自我介紹（6 段），半透明方塊、最寬 800px
- Experience：移除自我介紹段落、刪除日商艾鳴經歷、瑟菈職稱改 UIUX 設計師（職稱改 body1）、瑟菈與好玩兩筆新增工作內容說明與標籤、Software 標籤改黑底白字
- 首頁資料夾連結改指 WorkFile_Experience

### 全站優化
- 所有頁面加上 lang="zh-Hant"
- 導覽列 WORKS 改為可用鍵盤操作的按鈕，收合時選單連結不再能被 Tab 選到
- 莓卡頁修正合作者名稱 Mege Game → Mega Games
- 刪除 uploads/ 資料夾（31 個未使用的原始 PNG，約 28MB）
- 首頁只保留 index.html 一份內容；Page_Home.dc.html 改為自動跳轉，導覽列 / 換頁程式的 HOME 改指 index.html
