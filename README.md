# ✨ AI 流程圖生成器 (AI Flowchart Generator)

這是一個基於 Google Gemini AI 的自動化流程圖繪製工具。只要輸入文字描述（例如：「資料從 Oracle 抽出，經過 Python 清洗後寫入 SQL Server」），就能自動生成可編輯的流程圖。

## 🚀 快速開始

網頁連結： **[請在此貼上你的 GitHub Pages 網址]**

---

## 🔑 如何申請 Google Gemini API Key (免費)

為了讓 AI 運作，每個人都需要一組自己的 Google API Key。
**請放心，個人使用是免費的，且不需要綁定信用卡。**

### 步驟 1：前往 Google AI Studio
點擊此連結前往申請頁面：[https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

### 步驟 2：登入與建立
1. 使用你的 Google 帳號登入。
2. 點擊藍色的 **「Create API key」** 按鈕。
3. 選擇 **「Create API key in new project」** (在建立新專案中取得金鑰)。

### 步驟 3：複製金鑰
1. 系統會生成一串以 `Alza` 開頭的亂碼，這就是你的 API Key。
2. 點擊 **「Copy」** 複製它。
3. **注意：** 請妥善保存這組 Key，不要貼在公開的網路上。

---

## 🛠️ 如何使用本工具

1. **貼上 Key**：打開網頁，將剛剛複製的 Key 貼入左上角的「Gemini API Key」欄位。
2. **確認模型名稱**：
   - 預設建議使用：`gemini-1.5-flash`
   - 如果你是 Google 開發者計畫成員，可用 `gemini-3-flash-preview` (若無此權限請勿使用，會報錯)。
3. **輸入描述**：在文字框輸入你的業務邏輯。
4. **生成圖表**：點擊 **「⚡ AI 生成圖表」**。

### 🎨 進階功能
- **新增/刪除**：點擊綠色「➕」可新增節點；選中節點按 `Delete` 鍵可刪除。
- **編輯內容**：點擊圖上的節點或線條，左側面板可修改文字。
- **更換圖示**：系統會根據關鍵字（如 Oracle, Python）自動配圖，你也可以點選節點手動上傳圖片。
- **手動連線**：點擊「🔗 連線模式」，依序點擊 A 節點與 B 節點即可連線。

---

## ❓ 常見問題 (Q&A)

**Q: 為什麼按生成後出現 "404 Not Found" 或 "Model not found"?**
A: 這通常是因為模型名稱錯誤。請將左側的「模型名稱」欄位改為標準版：
`gemini-1.5-flash` 或 `gemini-pro`。

**Q: 為什麼出現 "Generative Language API has not been used"?**
A: 代表你的 API Key 專案尚未啟用 AI 功能。
1. [點此前往 Google Cloud Console](https://console.cloud.google.com/apis/library/generativelanguage.googleapis.com)
2. 確認上方選單是你剛剛建立的專案。
3. 點擊藍色的 **「啟用 (ENABLE)」** 按鈕即可。

**Q: 這是免費的嗎？**
A: 是的。Google 提供每分鐘 15 次請求、每天 1,500 次請求的免費額度，對個人使用來說非常足夠。
