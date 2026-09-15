MoneyMate V8｜Gmail OAuth 正式串接版

本版本保留 V7 全部功能，並將 Email 自動偵測記帳改為 Gmail OAuth + Gmail API：
1. 帳戶 → Email 自動偵測記帳。
2. Gmail 使用 Google OAuth 2.0 授權，不要求使用者輸入 Gmail 密碼。
3. 使用 Gmail API 唯讀範圍 gmail.readonly。
4. 授權後搜尋近 30 天符合消費／付款／刷卡／LINE Pay／發票等條件的郵件。
5. 解析店家、金額、日期、付款方式與分類。
6. 偵測到的交易先進入首頁「📥 待確認交易」，使用者確認後才寫入正式帳本。
7. 支援寄件人關鍵字篩選與手動「立即檢查 Gmail」。
8. 已連接狀態與待確認交易保存在本機 localStorage；OAuth access token 不寫入 localStorage。

Google Cloud 設定：
- OAuth 用戶端類型：Web application
- JavaScript origin：https://t777r6jpsw-png.github.io
- 本版本 Client ID 已寫入 index.html。
- Google Auth Platform → Audience：測試階段請先加入你自己的 Gmail 為測試使用者。
- Google Auth Platform → Data Access：需加入 https://www.googleapis.com/auth/gmail.readonly。

注意：若 GitHub Pages 的實際「origin」不同，必須在 Google Cloud 的 OAuth Client 中加入實際 origin。不要把 Client Secret 放進前端。
