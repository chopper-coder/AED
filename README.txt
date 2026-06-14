AED 模擬教學器 V2.3 GitHub CPR 手機音效修正版

修改重點：
1. 修正手機 GitHub Pages 上 CPR 階段可能沒有嗶嗶聲的問題。
2. CPR 節拍改成預先啟動 AudioContext 連續音訊引擎，再用 545ms 節拍控制音量脈衝。
3. 保留原本直接 oscillator 嗶聲作為備援。
4. 移除下方「教學提醒」顯示。
5. 更新 Service Worker 快取名稱，避免手機讀到舊版。

GitHub 使用方式：
請將 index.html、manifest.json、sw.js、aed-icon.svg、README.txt 上傳到 repository 根目錄。
上傳後建議用網址參數測試：?v=2.3
若手機仍讀到舊版，請清除網站資料或重新整理 GitHub Pages 快取。
