# Google 書籤自動分類 AI（Chrome Extension MVP）

## 專案簡介
這是一個 Chrome 擴充功能，能掃描未分類（根層）書籤，透過 AI 自動建議分類，並在你確認後才套用變更。

## 目前功能
- 掃描根層（unfiled/root-level）書籤
- 支援 OpenRouter 或 Gemini API 分類
- 分類結果可先審核再套用
- 可限制分類目標為你指定的既有資料夾
- 若分類結果不符合目標資料夾，會移到備援資料夾（預設 `AI Filtered`）
- 分類粒度可選 `Broad` 或 `Detailed`
- 支援「套用後復原（Undo latest apply）」

## 如何使用
1. 開啟 Chrome，進入 `chrome://extensions`
2. 開啟右上角 `Developer mode`
3. 點選 `Load unpacked`
4. 選擇本專案資料夾：
   - `C:\Users\User\Desktop\Google Drive\Google 書籤自動分類 AI`
5. 進入擴充功能 `API Settings`：
   - 選擇 provider
   - 輸入 API Key
   - 設定 model、granularity、fallback folder
   - 儲存設定
6. 回到擴充功能 Popup 介面：
   - 選擇 destination root
   - （可選）勾選限制可用的目標資料夾
   - 執行掃描與 AI 分類
   - 審核結果後套用
   - 若需要可執行 Undo



