# 🥦 [Mutation Feed] AI SEO Content Factory

### 📄 Module Overview
This feed pack (Mutation Feed) is designed for **safely automating the production of high-ranking content**. Rather than just generating text, it embeds the critical SEO logic of **E-E-A-T (Experience, Expertise, Authoritativeness, Trustworthiness)** and strict file operation guardrails deep into the AI agent's workflow. This is a standardized business workflow SOP controller.

### ⚙️ Skill Synergy
- **Recommended Skills**: `search_web`, `read_url`, `write_to_file`
- **Synergy Effect**: Before generating content, the agent is forced to call Search skills to investigate references and analyze competitors. Once generated, the output is safely written to the specified project directory via controlled file-writing tools.

### 🚀 Mutation Target & Protocol
1. **Research Before Writing (Inspect First)**: Enforces a three-step process of "Keyword Search -> Competitor Analysis -> SEO Structure Planning", strictly prohibiting blind writing.
2. **Safe Writing (Verify After Edit)**: The generated Markdown file must pass an SEO self-check (e.g., heading density, word count). If it fails, the agent must proactively rewrite it to prevent low-quality content from entering the workspace.
3. **E-E-A-T Validation**: Forces the agent to audit whether the article contains credible data citations and clear professional insights.

### 📋 Recommended Models
- **Recommended**: Gemini 3.0 Pro / GPT-5.3 / Claude Sonnet 4.6
- **Minimum**: Gemini 3.1 Flash / GPT-5.1
