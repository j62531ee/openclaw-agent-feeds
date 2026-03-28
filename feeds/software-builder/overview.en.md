# 🏗 [Mutation Feed] Software Project Architect (Software Builder)

### 📄 Module Overview
This feed pack (Mutation Feed) is designed to **safely generate and modify project architecture automatically within your workspace**. It features a behavioral script with strict safety protocols (Inspect, Backup, Minimal Diff, Verify, Rollback), injecting an SOP into your agent to act as a senior engineer who never breaks existing code structures.

### ⚙️ Skill Synergy
- **Recommended Skills**: `run_command` (terminal), `replace_file_content`, `write_to_file`, `list_dir`
- **Synergy Effect**: Paired with file operation tools, this workflow controller guarantees that every code write occurs under controlled, traceable safety guidelines. The agent will never blindly overwrite files, ensuring the integrity of your existing Official Structure.

### 🚀 Mutation Target & Protocol
1. **Inspect & Backup First**: Mandatory read of the existing file structure and temporary backup before any modifications.
2. **Minimal Diff**: Requires the agent to apply changes only to specific blocks when editing files, preserving unrelated logic.
3. **Verify After Edit**: Must attempt to call the corresponding linter or testing tool to verify syntax post-generation.
4. **Rollback-Ready**: If verification fails, the agent will proactively clean up and revert to the pre-edit state.

### 📋 Recommended Models
- **Recommended**: Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6 (excellent code structure awareness)
- **Minimum**: Gemini 3.1 Flash / GPT-5.1 / Claude Haiku 4.5
