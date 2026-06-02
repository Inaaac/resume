# Ina Chen — Resume (HTML)

通用版履歷，以靜態 HTML 呈現，可透過 [GitHub Pages](https://pages.github.com/) 公開瀏覽。

## 線上瀏覽

啟用 GitHub Pages 後，網址通常為：

- **首頁（建議分享）：** `https://<你的 GitHub 帳號>.github.io/<repo 名稱>/`
- **或直接：** `https://<你的 GitHub 帳號>.github.io/<repo 名稱>/resume.html`

`index.html` 與 `resume.html` 內容相同；更新履歷時請同步兩者，或執行：

```bash
cp resume.html index.html
```

## 本機預覽

在專案資料夾開啟 `resume.html` 或 `index.html`，或使用：

```bash
python3 -m http.server 8080
# 瀏覽 http://localhost:8080/
```

## 檔案說明

| 檔案 | 說明 |
|------|------|
| `resume.html` | 通用版履歷（主檔） |
| `index.html` | GitHub Pages 首頁（與 `resume.html` 同步） |
| `resume.css` | 樣式 |
| `resume-LineBank.html` | Line Bank 投遞變體（不對外預設） |
| `base-0522.md` | Markdown 來源（通用版） |

## 首次推送到 GitHub

1. 在 GitHub 建立新 repository（例如 `resume`），**不要**勾選加入 README（避免衝突）。
2. 在本機執行（將 `<帳號>`、`<repo>` 換成你的）：

```bash
cd /path/to/resume
git remote add origin https://github.com/<帳號>/<repo>.git
git branch -M main
git push -u origin main
```

3. 到 repo **Settings → Pages**：Source 選 **Deploy from a branch**，Branch 選 **main**、資料夾 **/ (root)**，儲存。
4. 約 1–2 分鐘後即可用上面的網址開啟履歷。
