MoneyMate V8｜Email 自動偵測記帳 Prototype

本版本保留 V7 全部功能，新增 Email 自動偵測記帳介面：
1. 帳戶／設定可開啟「Email 自動記帳」。
2. 可選 Gmail、iCloud、Outlook（目前為 Prototype 介面，尚未真的登入信箱）。
3. 可設定銀行／信用卡、LINE Pay、電子發票等來源開關。
4. 可貼上消費通知 Email 測試解析，或模擬收到 2 封新消費 Email。
5. Email 交易先進入「待確認交易」，確認後才寫入正式帳本。
6. 待確認交易會出現在首頁，可逐筆記帳。

重要：一般網頁 Prototype 不能直接讀取使用者 Gmail/iCloud/Outlook 信箱。正式版需使用合法的 OAuth／郵件 API 並取得使用者明確授權。Apple 的 MailKit 是 Mail App Extension 框架，不等同於第三方 App 可任意讀取所有郵件；正式產品應依實際郵件服務 API 與 Apple 平台規範設計。
