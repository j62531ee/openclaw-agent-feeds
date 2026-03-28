# 🧪 [Mutation Feed] 自主研究引擎 (Autonomous Research Engine)

### 📄 模組簡介
本飼料包（Mutation Feed）專為需要**深度資料挖掘**與**資訊驗證寫出**的任務設計。它能將您的 OpenClaw 工作區裝載「迭代驗證與安全報告生成」的 SOP 流程控制器。

### ⚙️ 技能協同 (Skill Synergy)
- **建議搭配**：`search_web`, `read_url`, `write_to_file`, `list_dir`
- **協同效應**：透過強制調用搜尋工具進行初步與後續交叉驗證，並在資料確鑿後，遵循寫檔安全協議產生研究報告，絕不干擾專案核心代碼。

### 🚀 變異目標與協議 (Mutation Protocol)
1. **安全報告寫入 (Inspect & Backup First)**：確保產出的研究報告僅限於指定資料夾，若需更新必須先進入備份防呆確認。
2. **三階段驗證法**：強制執行 檢索 -> 交叉比對 -> 衝突解決 的狀態機迴圈。
3. **資訊預警 (Rollback-Ready)**：當資訊不足以支撐結論且無法查證時，強制觸發回溯與中斷邏輯，終止寫入並通知用戶。

### 📋 建議模型
- **推薦版本**：Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6
- **最低版本**：Gemini 3.1 Flash / GPT-5.1
