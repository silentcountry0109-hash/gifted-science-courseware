# 資優自然 互動課件（電子白板版）

典陸教育集團｜資優自然主題式講義 主課程 20 堂的 16:9 電子白板課件。

- `index.html`：主頁，點選進入各堂。
- `g01.html`～`g20.html`：各堂課件（單一檔案，字型內嵌，可離線開啟）。

## 部署到 GitHub Pages

1. 在 GitHub 建一個**空的** repository（不要勾選建立 README）。
2. 在這個資料夾執行：
   ```
   git remote add origin https://github.com/<帳號>/<repo 名稱>.git
   git push -u origin main
   ```
3. GitHub 上該 repo → Settings → Pages → Build and deployment：Source 選「Deploy from a branch」，Branch 選 `main`、資料夾 `/ (root)`，按 Save。
4. 約 1～2 分鐘後網址會出現在同一頁：`https://<帳號>.github.io/<repo 名稱>/`。

## 更新

課件重建後，把新的 `index.html`、`gNN.html` 複製進來覆蓋，然後：
```
git add -A
git commit -m "更新課件"
git push
```

## 注意

- 課件頁面裡含有全部答案（點擊才顯示，但看原始碼看得到）。公開的 GitHub Pages 任何人拿到網址都能開。
- 筆跡存在各台電腦的瀏覽器（localStorage），不會上傳、不跨裝置。
