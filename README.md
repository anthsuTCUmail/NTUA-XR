# 台藝大演講：手機體驗網頁

- `index.html` 目錄頁（投影這頁的 QR code）
- `ar.html` 體驗一：AR 把雕塑放進教室
- `ink.html` 體驗二：吹墨（點擊滴墨、吹氣、傾斜）
- `models/` 三件示範雕塑（.glb）
- `lib/` model-viewer（Google，Apache 2.0），已內建，不依賴外部 CDN

## 部署（一定要 HTTPS，否則手機不給麥克風／感測器）
最簡單：打開 https://app.netlify.com/drop ，把整個資料夾拖進去，取得網址。
或：GitHub Pages。

## 換成自己的作品
1. 用 Polycam 等 App 掃描實體作品，匯出 .glb，放進 `models/`
2. 修改 `ar.html` 裡的 `WORKS` 陣列（檔名、標題、材質、說明）
3. 單一模型建議 5 MB 以下，現場網路才撐得住

## 事前測試清單
- iPhone Safari 與 Android Chrome 各測一次
- AR：iPhone 會開啟 Quick Look；Android 需支援 ARCore
- 吹墨：對著手機下方（麥克風位置）短促吹氣效果最好
