# 🛡 [Training Feed] 反幻覺邏輯護欄 (Hallucination Guardrails)

### 📄 模組簡介
本飼料包（Training Feed）專精於**事實查核與防禦幻覺**。它為您的 OpenClaw 工作區注入了「查證優先」的真實狀態機 (True State Machine)，強制代理在處理包含具體數據、名詞或歷史事實的任務時，必須進入嚴格的交叉驗證迴圈，絕不憑空捏造。

### ⚙️ 技能協同 (Skill Synergy)
- **建議搭配**：`search_web`, `read_url`
- **協同效應**：代理在 Execute 之前，必須強制調用 Search 技能。若工具不可用，將觸發 Failure Branch 主動告知用戶，而不會嘗試盲目作答。

### 🚀 變異目標與協議 (Mutation Target)
1. **條件分流 (Conditional Branches)**：內建完整的查核分支。若搜尋無結果，直接進入失敗回報；若多方資訊衝突，進入釐清分支。
2. **強制驗證 (Mandatory Verify)**：輸出前必須自檢所有「宣稱 (Claims)」是否附有來源標記。
3. **精準評估 (Check Tooling)**：接收任務後首要動作是盤點搜尋工具是否就緒。
4. **靜默運行 (Silent Residency)**：底層常駐不干擾日常對話，默默守護事實底部。

### 📋 建議模型
- **推薦版本**：Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6
- **最低版本**：Gemini 3.1 Flash / GPT-5.1
