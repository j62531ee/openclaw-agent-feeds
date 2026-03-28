# 🥦 [Mutation Feed] AI SEO 內容工廠 (AI SEO Content Factory)

### 📄 模組簡介
本飼料包（Mutation Feed）專為**安全自動化生產高排名內容**設計。它將代理的寫作流程升級為「先研究後寫作」的真實狀態機 (True State Machine)，強制綑綁 E-E-A-T (經驗、專業、權威、信任) 邏輯與嚴格的檔案寫入護欄，避免代理在內容枯竭時隨意瞎掰。

### ⚙️ 技能協同 (Skill Synergy)
- **建議搭配**：`search_web`, `read_url`, `write_to_file`
- **協同效應**：代理在生成內容前必須強制調用 Search 技能。若未取得足量競品情報，將觸發 Failure 分支要求重新盤點關鍵字。寫入檔案時則受限於 Mutation 護欄。

### 🚀 變異目標與協議 (Mutation Target)
1. **條件分流 (Conditional Branches)**：當指定關鍵字的搜尋結果不足或方向矛盾時，觸發 Clarification 分支與用戶重新對焦。
2. **強制驗證 (Mandatory Verify)**：輸出至 Markdown 後，強迫自我檢核是否出現空心數據、或 H3 標籤分層是否失控。
3. **精準盤點 (Check Tooling)**：接收任務後首要確保寫檔權限與 Search API 皆處於活躍狀態。
4. **全域常駐 (Pervasive Scope)**：所有涉及「長文寫作、SEO 優化、內容行銷」等非平凡任務，皆受到此狀態機管轄。

### 📋 建議模型
- **推薦版本**：Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6
- **最低版本**：Gemini 3.1 Flash / GPT-5.1
