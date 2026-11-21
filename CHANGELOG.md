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

## v1.3 – 內部推動專案、Greon 新頁（2026-11-16 ～ 11-21）

### B2B 頁（UIUX_02_B2B）
- 更新 Problem & Solution 圖（b2b_img_block1）、AI Collaboration 圖（b2b_img_block2），加上 ?v=2 避免快取舊圖
- User Flow 上方新增兩個區塊：Functional Map（b2b_img_block5）、IA（b2b_img_block6）
- Functional Map 上方新增區塊「使用者需求」：Vendor / Official 兩張黑底格線卡片，保留樹狀結構（├ └ 連接線），功能以文字列出
- 更新 Functional Map、IA 圖；使用者需求卡片四邊加上淡光暈（比照圖片卡片邊緣）
- Functional Map 標題下方新增說明：以目標、功能、資訊為三個節點來進行發想。
- User Flow 換成新圖（Vendor 上架新遊戲送出審核、Official 審核上架新遊戲），加上 ?v=2
- AI Collaboration 移到使用者需求上方；換新圖（b2b_img_block2，?v=3），標題下方新增說明（後台以操作需求與製作效率為優先、全流程使用 Claude Design 與 shadcn/ui）
- UIUX 區塊改版：後台主頁、新增遊戲資料兩張黑底卡片（標示 Vendor）；後台主頁加上 4 點說明與程式碼繪製的篩選 / 排序 / 欄位示意（隨畫面縮放）
- 新增遊戲資料：Before / After 滑桿加上步驟按鈕，標籤改為「企劃需求 / 設計介面架構調整」；新增 4 點說明（整體、遊戲介紹分頁、社群連結分頁、遊戲發布分頁）與第 3、4 點前後對照圖（b2b_img_note3 / note4）
- 用字統一「後臺」→「後台」；程式碼整理（共用樣式合併、移除未使用樣式）

### UIUX 列表頁（Page_UIUX）
- 卡片分成兩組：「推動團隊內部設計系統化」（在上）、「專案」（在下）
- 新增 3 張內部推動卡片：Figma Team 檔案歸納、導入 Design Token、共用元件整合（新封面 uiux_img_cardover_file / token / com）
- B2B 卡片標題改為「PH B2B 後台」
- 新增 Greon 專案卡片（接在 B2B 後面），新封面 uiux_img_cardover_greon，標籤 #ux #leadership #learning project
- 內部推動卡片說明、標籤更新（導入 Design Token、共用元件整合）
- 預先載入加入 UIUX_IN_01 ～ 03、UIUX_08_Greon

### 內部推動專案（新增 3 頁）
- UIUX_IN_01：Figma Team 檔案歸納。Problem（引言 + 2 張圖）、Solution（外層資料夾／中層檔案封面／內層頁面結構，含 HTML 分類表）、Result（引言 + BEFORE / AFTER）
- UIUX_IN_02：導入 Design Token。Problem（引言 + 舊規範圖）、Solution（訂定規範、建置工具）、Result（引言 + 莓卡官網 / PlayHorny SDK 兩組 Token 圖，附「前往專案 ↗」連結）
- UIUX_IN_03：共用元件整合。Problem（引言 + 程式碼繪製的 Copy & Paste 示意圖）、Solution（階段一：釐清規格 3 步驟，含一改即同步樹狀圖、Header / Footer 樣式卡片；階段二：建立元件，含使用文件與元件圖）、Result（大數字 3 / 2 / 1）
- 三頁共用黑底格線卡片、引號引言樣式；圖片加上寬高屬性、窄螢幕自動直排
- UIUX_IN_02：Solution 刪除第三張卡片；規範圖兩張等高、工具圖上下排；Problem 圖修正透明邊角變黑
- UIUX_IN_03：步驟小標改為「My Chara：…」「企劃：統整規格」；Header / Footer 樣式卡片改為橫向並排、加上「適用頁面」標籤；階段二四張圖縮小置中、文件圖在右；Result 改為大數字呈現並移除 BEFORE / AFTER；文字層級依設計系統調整
- 三頁 Head（引言、簡介、標籤、時間）與封面更新

### Greon 頁（新增 UIUX_08_Greon）
- 學習計畫專案，擔任五人團隊組長（Team Lead (Me)）
- 區塊：UX Exploration（5 步驟：產品方向研究、使用者情境卡、User Story Map、功能盤點與分工、Flow Chart）、方向調整（導師回饋 / 團隊檢視 / 團隊調整 + 2 張簡報）、UI 階段支援、成果提交（封面 + 12 張簡報）、反思（3 點）
- 新封面 greon_img_cover（去除浮水印版本）

### 莓卡頁（UIUX_04_Mega）
- Design System 標題下方新增說明（以 Design Token 建立三層設計系統、為團隊首次導入的專案）與「延伸閱讀：導入 Design Token ↗」連結
- UIUX_IN_02 Result 同步改為三層 Token
- Design Token 圖換成兩張：mega_img_designtoken1（三層架構）、mega_img_designtoken2（實際應用：以按鈕為例）
- 刪除：assets/mega_img_designtoken(-1x).webp

### PH 儲值 UI 頁（UIUX_01_SDK_UI）
- Design System 標題右側新增「延伸閱讀：導入 Design Token ↗」連結
- 標題下方新增說明：延續莓卡官網的 Token 架構，擴充至 Dimension（邊距、圓角、間距）

### PH 登入頁（UIUX_03_PH_Login）
- 更換 log_img_block01（登入、註冊、忘記密碼畫面優化，含 Before / After），加上 ?v=2

### 人員欄
- 自己的職稱統一為「Designer (Me)」（SDK UI、Login、IN_01 ～ 03 等頁）

### 共用元件（Com_Project_Head）
- Device 欄位為空時自動隱藏
- 新增 tag-fill 屬性：標籤寬度填滿、文字置中（預設不開，其他頁不受影響）
