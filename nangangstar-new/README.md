# 南港之星 改版網站（靜態版）

純靜態網站，可直接用 GitHub Pages 部署，不需要建置步驟。

## 頁面
- `index.html` 首頁
- `reserve.html` 線上選房（35–37F）
- `grid.html` 銷控表
- `order.html` 預約單（潤泰預售收款憑證格式）

## 部署到 GitHub Pages
1. 建立新的 repository（例如 `nangangstar-new`），把這個資料夾內所有檔案（含 `.nojekyll`、`assets/`）上傳到根目錄。
2. 到 repository 的 Settings → Pages，Source 選 **Deploy from a branch**，Branch 選 `main`、資料夾選 `/ (root)`，按 Save。
3. 約 1–2 分鐘後，網址會是 `https://<帳號>.github.io/<repository 名稱>/`。

## 注意
- 戶別、價格、預約單資料為提案示意；「送出預約」不會傳送資料，尚未串接原站預約 API 與業務後台。
- `support.js` 是頁面的渲染程式，內含 morphdom（MIT License, © Patrick Steele-Idem）。
- 影片放在 `assets/video/`，單檔皆小於 12 MB，符合 GitHub 單檔 100 MB 限制。
