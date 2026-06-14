AED 模擬教學器 V2 離線穩定版
================================

版本日期：2026-06-14

檔案內容：
1. index.html       主程式，已移除外部 CDN，單檔即可開啟
2. manifest.json    PWA 安裝資訊
3. sw.js            Service Worker 離線快取
4. aed-icon.svg     PWA 圖示

使用方式：
- 最簡單：直接用 Chrome / Edge / Safari 開啟 index.html。
- 內網教學：可將整個資料夾放到內網 Web Server，開啟 index.html。
- PWA 離線快取：Service Worker 需要 localhost、http 內網主機或 https 環境；file:// 直接開啟時，頁面仍可使用，但瀏覽器不會啟用 Service Worker。

V2 修正重點：
- 移除 Tailwind CDN，避免無網路時樣式失效。
- 補上 manifest.json、sw.js、aed-icon.svg。
- 補上電擊按鈕閃爍 CSS。
- LINE 內建視窗改成提醒，可手動關閉，不會讓使用者誤以為卡住。
- 改用 Pointer Events，提升手機、平板、電腦拖曳穩定性。
- 重構狀態機與計時器清理，降低重複播放與狀態殘留。
- 保留 AED 教學流程：開機、貼片、分析、建議電擊、不建議電擊、CPR 110 BPM、觸電防錯。
- 加入基本 Content Security Policy，避免誤連外部資源。

注意事項：
- 手機瀏覽器通常需要先點「進入模擬教學」才能解鎖語音與節拍音。
- LINE 內建瀏覽器可能限制語音，建議改用 Safari / Chrome。
- 本系統是教學模擬器，不可取代真實 AED 操作訓練與正式醫療指引。
