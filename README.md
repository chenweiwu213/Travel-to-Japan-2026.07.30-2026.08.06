# 福岡・山口・廣島・神戶・大阪 旅遊手冊

北九州到關西的八天七夜行程。HTML檔案，含每日行程、記帳、匯率換算、天氣查詢與中日文翻譯小工具。

## 功能

- **行程總覽**：每日路線、時刻表、景點介紹，點擊景點直接開啟Google Maps導航
- **記帳**：多人共用花費紀錄，即時同步（Firebase Firestore），自動依匯率換算台幣總額
- **匯率換算**：即時日圓兌台幣匯率查詢與雙向換算
- **天氣預報**：行程沿線各地點的逐小時天氣查詢
- **中翻日小幫手**：常用旅行短句一鍵翻譯

## 技術架構

純前端靜態網頁，無需建置流程：

- HTML/CSS/原生JavaScript（ES Module）
- [Firebase Firestore](https://firebase.google.com/docs/firestore) — 記帳資料即時同步
- [Open-Meteo API](https://open-meteo.com/) — 天氣預報
- [ExchangeRate API](https://www.exchangerate-api.com/) — 即時匯率
- [MyMemory Translation API](https://mymemory.translated.net/) — 翻譯備援服務

## 本機開啟

可直接用瀏覽器開啟'index.html'，不需要安裝任何套件或啟動伺服器。

## 部署

以GitHub Pages部署，推送到'main'分支後由GitHub Pages自動發布靜態頁面。

## 關於 Firebase 金鑰

'index.html'內含的Firebase用戶端設定是Firebase Web SDK依規範必須公開於前端的識別資訊，非後端密鑰，本身不具備存取控制能力。
