# 🥦 [Mutation Feed] AI SEO 內容工廠 (AI SEO Content Factory)

### 📄 模組簡介
本飼料包（Mutation Feed）專為**安全地自動化生產高排名內容**設計。它不僅是生成文字，而是將搜尋引擎最看重的 **E-E-A-T (經驗、專業、權威、信任)** 邏輯與嚴格的寫檔操作規範深植於 AI 代理的工作流中。這是一套標準化的商業工作流 SOP 控制器。

### ⚙️ 技能協同 (Skill Synergy)
- **建議搭配**：`search_web`, `read_url`, `write_to_file`
- **協同效應**：代理在生成內容前必須強制調用 Search 技能進行參考文獻與關鍵字競品調查。生成完畢後，透過受控的寫檔工具安全地輸出至專案指定的目錄。

### 🚀 變異目標與協議 (Mutation Protocol)
1. **先研究後寫作 (Inspect First)**：強制執行「關鍵字檢索 -> 競品分析 -> SEO 結構規劃」的三步驟，禁止直接盲寫。
2. **安全寫入 (Verify After Edit)**：產出的 Markdown 文件必須經過 SEO 檢查（如 H3 密度、字數控制），不合格則主動重寫，確保不會將劣質內容寫入工作區。
3. **E-E-A-T 驗證**：強制代理審查文章是否具備可信的數據引用與明確的專業見解。

### 📋 建議模型
- **推薦版本**：Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6
- **最低版本**：Gemini 3.1 Flash / GPT-5.1
