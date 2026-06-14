AED 模擬教學器 V2.2 GitHub CPR 嗶聲恢復版

本版重點：
1. 保留 V2 離線版，不使用 Tailwind CDN，可直接放到 GitHub Pages。
2. 取消畫面上的「放電危險勿靠近」覆蓋提示。
3. CPR 110 BPM 嗶嗶聲改回原本手機較穩定的 Web Audio 直接震盪器寫法。
4. Service Worker 快取名稱已更新為 V2.2，避免 GitHub Pages 手機端讀到舊快取。

GitHub Pages 更新方式：
1. 將本資料夾內所有檔案上傳到 repository 根目錄。
2. 確認 index.html、manifest.json、sw.js、aed-icon.svg 都在同一層。
3. 手機若仍讀到舊版，請到瀏覽器清除網站資料，或網址後加 ?v=2.2 測試。
4. iPhone 建議使用 Safari 開啟；Android 建議使用 Chrome 開啟。

操作：
1. 開啟網頁後先按「進入模擬教學（解鎖語音）」。
2. 按 ON/OFF 開機。
3. 拖曳兩片貼片到正確位置。
4. 進入 CPR 階段後，畫面會顯示「嗶！110 BPM」，並自動播放 CPR 節拍。
