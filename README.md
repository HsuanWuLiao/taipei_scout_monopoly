# 雙北捷運鐵道・童軍大富翁實境遊戲

以大富翁為基底的多人線上連線實境遊戲網頁，限縮於臺北與新北範圍，結合捷運及台鐵車站、公告土地現值換算地價、雙領域問答（童軍知識與文史知識）及 Google Sheet 雲端資料庫。

## 檔案結構
- `index.html`：完整單頁式遊戲應用程式（GitHub Pages 預設入口）
- `.nojekyll`：停用 Jekyll 解析以加速靜態網頁載入

## 雲端資料庫與連線設定
1. 開啟對應的 Google Sheet 資料庫：[捷運鐵道童軍大富翁＿遊戲資料庫](https://docs.google.com/spreadsheets/d/1yWTz1Utv-SwPYaeTrc6rgU4x-eoDsG1q682eLBv7wBA/edit)
2. 在試算表上方點選 **擴充功能 → Apps Script**。
3. 從網頁右上角「**Google Sheet 設定**」按鈕複製內附的 `Code.gs` 程式碼貼上並儲存。
4. 點選 **部署 → 新增部署作業 → 類型選擇「網頁應用程式」**，將「誰可以存取」設為 **所有人 (Anyone)**，複製產生的 Web App URL。
5. 回到遊戲網頁右上角「**Google Sheet 設定**」，貼上該 URL 並點擊「**連線測試**」，即可啟用跨裝置多人即時同步。

## GitHub Pages 佈署方式
1. 在 GitHub 建立一個新的公開儲存庫（Repository）。
2. 將本資料夾內的 `index.html`、`.nojekyll` 與 `README.md` 上傳或推播至 `main` 分支根目錄。
3. 前往儲存庫的 **Settings → Pages**，將 **Source** 設為 **Deploy from a branch**，分支選擇 `main` / `/ (root)` 後儲存，約 1–2 分鐘即可取得公開網址。
