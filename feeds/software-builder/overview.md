# 🏗 [Mutation Feed] 軟體專案架構代理 (Software Builder)

### 📄 模組簡介
本飼料包（Mutation Feed）專為**安全地在工作區自動生成與改變專案架構**設計。具備在安全協議下修改現有 OpenClaw 專案與檔案權限的行為腳本，將一段嚴格的（Inspect, Backup, Minimal Diff, Verify, Rollback）SOP 注入到您的代理中，使其成為一位不會破壞現有程式碼架構的資深工程師。

### ⚙️ 技能協同 (Skill Synergy)
- **建議搭配**：`run_command` (terminal), `replace_file_content`, `write_to_file`, `list_dir`
- **協同效應**：配合檔案操作工具，這套流程控制器能保證每一次的代碼寫入都在受控、可回溯的安全規範下進行，代理不會盲目覆寫檔案，確保現有 Official Structure 的完整性。

### 🚀 變異目標與協議 (Mutation Protocol)
1. **先審視與備份 (Inspect & Backup First)**：所有修改前，強制讀取現有檔案架構並暫存備份。
2. **最小化差異 (Minimal Diff)**：在編輯檔案時，要求代理僅針對特定區塊進行變更，不破壞無關邏輯。
3. **修改後驗證 (Verify After Edit)**：代碼產出後必須試著呼叫對應的 linter 或測試工具驗證語法。
4. **隨時準備復原 (Rollback-Ready)**：若驗證失敗，代理將主動清理並還原至編輯前的狀態。

### 📋 建議模型
- **推薦版本**：Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6 (擁有優異的程式碼結構意識)
- **最低版本**：Gemini 3.1 Flash / GPT-5.1 / Claude Haiku 4.5
