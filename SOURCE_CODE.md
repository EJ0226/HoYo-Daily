# HoYo Daily Sign-in 的原始碼取得方式

本文件是隨 HoYo Daily Sign-in 二進位檔發布的原始碼通知。

本程式整合 AGPL-3.0 授權的 `hoyolab-auto`。因此，對應此 EXE 的完整可修改原始碼，依 GNU Affero General Public License v3.0 or later 提供，且不得額外收費。

## 發行者必填資料

在每次公開發布前，請將下列內容替換為實際資料；不可保留示意網址。

- 產品版本：`0.1.0`
- 對應原始碼封存檔：`HoYo-Daily-Sign-in-Source-0.1.0.zip`
- 下載網址：`https://github.com/EJ0226/HoYo-Daily/releases/download/v1.0.0/HoYo_Daily_Sign-in_Portable_0.1.0_Subscription.exe`
- SHA-256：請在上傳來源 ZIP 後，將該檔案的 SHA-256 貼到網站下載頁面。
- 原始碼提供期限：在您持續發布此二進位檔期間，至少於同一下載頁面提供。

## 原始碼內容

封存檔包含桌面應用程式、測試、建置設定、獨立授權／ECPay 後端範例、`hoyolab-auto` 的未修改來源、第三方通知、變更紀錄及 AGPL 授權全文。

封存檔刻意不包含 `node_modules/`、`dist/`、本機 SQLite 資料庫、Cookie、Token、Webhook URL、ECPay 密鑰或任何使用者資料。

## 建置

請使用 Node.js 20 或更高版本：

```powershell
npm install
npm test
npm run dist
```

原始碼收到者可以依 AGPL-3.0-or-later 的條款執行、研究、修改與散布本程式。
