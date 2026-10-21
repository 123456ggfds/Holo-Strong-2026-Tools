# Holo 強 2026 Tools

一個可部署到 GitHub Pages 的靜態網站/PWA，包含：
- `index.html`：工具首頁與使用說明
- `members.html`：64 強分組成員複製工具
- `countdown.html`：賽事結束即時倒數工具
- `manifest.webmanifest`、`sw.js`、`icons/`：主畫面安裝與離線快取設定

## 發布到 GitHub Pages

1. 在 GitHub 建立新的 **Public** repository，例如 `holo-strong-tools`。
2. 把本資料夾內的**所有檔案與資料夾**上傳到 repository 根目錄（不是只上傳兩個 HTML）。
3. 到 repository 的 **Settings → Pages**。
4. 在 Build and deployment 選擇 **Deploy from a branch**，Branch 選 `main`，資料夾選 `/(root)`，儲存。
5. 等待 GitHub Pages 完成部署。若 repository 名稱是 `holo-strong-tools`，網站首頁網址會是 `https://<你的 GitHub 使用者名稱>.github.io/holo-strong-tools/`。

> 上面的網址只是格式示例，實際網址須由 GitHub Pages 部署完成後確認。

## 加入手機主畫面

- **iPhone**：用 Safari 開啟部署後的 HTTPS 網址 → 分享 → 加入主畫面。
- **Android**：用 Chrome 開啟部署後的 HTTPS 網址 → 選單 → 加到主畫面/安裝應用程式。

PWA 的完整安裝及 Service Worker 離線快取需透過 HTTPS 或 localhost 執行，不會在本機直接點開 HTML 時完整啟用。

## 更新賽事結束時間

在 `countdown.html` 內，預設時間目前是 `2026-11-13 23:59`（台灣時間，暫定）。頁面內也提供設定欄位供使用者調整。若需要變更預設值，請同步修改日期輸入框預設值及 JavaScript 中的預設日期。

## 名單提示

成員名單沿用目前對話中的暫定 64 強分組；正式晉級資格尚未重新核對。
