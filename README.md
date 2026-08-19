# HoYo Daily Sign-in Desktop

Windows 桌面工具，透過 HoYoLAB 官方網頁／API 流程處理每日簽到與公開兌換碼。它不修改遊戲檔案、不注入 DLL、不讀取遊戲記憶體，也不自動操作遊戲內客戶端。

## 本機桌面版

- 多帳號與原神、星穹鐵道、絕區零。
- HoYoLAB 視窗登入或手動 Cookie；秘密使用 Windows DPAPI 保存。
- 每日簽到排程、Windows 開機啟動、公開兌換碼輪詢與 Discord Webhook。
- 兌換碼之間固定間隔 10 秒，執行紀錄不會記錄 Cookie、Token 或 Webhook URL。
- 「方案與授權」頁可離線驗證 7 天、1 個月與 1 年的 Premium 簽章授權碼；不需後端。

若要看使用教學請前往 [HoYo_Daily_Sign-in_使用教學.docx](HoYo_Daily_Sign-in_使用教學.docx)

### 免費版與 Premium

| 功能 | 免費版 | Premium／7 天體驗 |
| --- | --- | --- |
| 帳號數 | 1 | 多帳號 |
| 簽到與兌換 | 手動 | 手動與自動 |
| 每日排程、公開 Code 輪詢 | — | ✓ |
| Discord、Windows 開機啟動 | — | ✓ |
| 本機日誌 | ✓ | ✓ |

因本專案依 AGPL 發布，取得原始碼的人可自行修改程式；這些限制是產品方案功能，而非用來剝奪 AGPL 使用者的權利。

```powershell
npm install
npm test
npm start
```

建立 Windows 可攜版：

```powershell
npm run dist
```

## 授權

本專案整合 AGPL-3.0 元件，因此整個合併作品依 **GNU Affero General Public License v3.0 or later** 發布。請閱讀 [LICENSE](LICENSE)、`THIRD_PARTY_NOTICES.md`、`THIRD_PARTY_CHANGES.md` 與 `THIRD_PARTY_LICENSES/`。

每一個 EXE 發行版本都必須在同一個下載頁面，免費提供可對應該版本的原始碼 ZIP。發行時請將下載連結、版本與 SHA-256 填入 [SOURCE_CODE.md](SOURCE_CODE.md)。
