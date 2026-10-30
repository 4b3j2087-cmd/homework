# 韓系簡約風｜視覺傳達設計作品集

## 專案檔案
- `index.html`：網站內容與區塊
- `style.css`：版面、顏色、動畫與手機版樣式
- `script.js`：分類篩選、圖片燈箱、選單、游標與捲動動畫
- `images/`：請放入自己的作品圖片
- About 後的 Profile 區塊展示興趣、專長與證照，使用 `art02.JPG`、`art03.JPG` 和 `certificate.jpg`。

## 操作步驟
1. 將整個 `korean_minimal_portfolio` 資料夾解壓縮。
2. 使用 VS Code 開啟這個資料夾（不要只開單一 HTML 檔）。
3. 在 VS Code 左側檔案區，確認 `index.html`、`style.css`、`script.js` 都在同一層。
4. 安裝擴充功能 **Live Server**。
5. 在 `index.html` 上按右鍵，選擇 **Open with Live Server**。
6. 瀏覽器會開啟網站；修改並存檔後，瀏覽器通常會自動更新。

## 更換自己的圖片
將圖片放入 `images` 資料夾，並使用以下檔名（或同步修改 HTML 的圖片路徑）：
- `hero.jpg`：首頁主視覺
- `profile.jpg`：個人照片
- `illustration1.jpg`、`illustration2.jpg`：插畫
- `graphic1.jpg`、`graphic2.jpg`：平面設計
- `3d1.jpg`、`3d2.jpg`：立體作品
- `photo1.jpg`、`photo2.jpg`：攝影作品

建議使用 JPG、PNG 或 WebP。作品圖片盡量統一長寬比例，版面會更整齊。
目前資料夾內沒有預設作品圖，請自行放入圖片並使用上面的檔名。

## 修改個人資料
- 在 `index.html` 搜尋 `你好！我是`，把 `＿＿＿` 改成自己的名字。
- 搜尋 `YOURMAIL@EXAMPLE.COM` 和 `yourmail@example.com`，改成自己的電子郵件。
- 修改首頁標題、ABOUT 介紹文字即可。

## 增加作品
複製 `index.html` 裡任一個 `<button class="work-card ...">...</button>` 區塊，貼在 `work-grid` 裡，再修改：
- `data-category`：只能使用 `illustration`、`graphic`、`3d`、`photography`
- `data-title`：燈箱中顯示的作品名稱
- `data-image`：圖片路徑
- `<img src>`：同一張圖片路徑
- `alt`：圖片替代文字

點擊作品會放大圖片；可以用左右箭頭切換、Esc 關閉。作品沒有詳細介紹頁，僅顯示作品名稱。
