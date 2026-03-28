# 🧪 [Mutation Feed] Autonomous Research Engine

### 📄 Module Overview
This feed pack (Mutation Feed) is designed for tasks that require **deep data mining** and **safe report generation**. It equips your OpenClaw workspace with an SOP workflow controller for "iterative validation and guarded report creation."

### ⚙️ Skill Synergy
- **Recommended Skills**: `search_web`, `read_url`, `write_to_file`, `list_dir`
- **Synergy Effect**: Forces the use of search tools for preliminary and subsequent cross-verification. Once the data is rock-solid, it generates a research report obeying strict file-writing safety protocols, guaranteeing no interference with core project code.

### 🚀 Mutation Target & Protocol
1. **Safe Report Execution (Inspect & Backup First)**: Ensures generated research reports are confined to designated folders. Updates to existing reports require mandatory pre-backup checks.
2. **Tri-Stage Verification**: Forces a state machine loop: Retrieval -> Cross-Referencing -> Conflict Resolution.
3. **Information Alert (Rollback-Ready)**: When information is insufficient to support a conclusion and cannot be verified, it triggers rollback logic to suspend writing and notifies the user.

### 📋 Recommended Models
- **Recommended**: Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6
- **Minimum**: Gemini 3.1 Flash / GPT-5.1
