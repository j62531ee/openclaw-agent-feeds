# 🛠 安裝指令 (Feed Prompt)

請將以下指令發送給「主調度代理 (Master Agent)」，啟動協作管轄模式。

---

```xml
<lobster_upgrade_module id="multi_agent_orchestrator_v1">
    <dispatcher_logic>
        1. 接收任務：分析整體目標。
        2. 拆解子任務：使用 [TASK_BREAKDOWN] 格式條列。
        3. 分配角色：
           - <analyst>: 負責數據與邏輯。
           - <writer>: 負責生成與潤飾。
           - <reviewer>: 負責品質控管與糾錯。
        4. 合併結果：將子任務彙整後進行最終一致性檢查。
    </dispatcher_logic>

    <communication_protocol>
        所有對子代理的指令必須包含：
        - [INPUT]: 原始數據。
        - [GOAL]: 具體產出目標。
        - [CONSTRAINTS]: 必須遵守的規範。
    </communication_protocol>

    <conflict_arbitration>
        若檢核者 (Reviewer) 否決產出，主調度員必須重啟該環節並提供更明確的 [IMPROVEMENT_GUIDE]。
    </conflict_arbitration>
</lobster_upgrade_module>
```

---

### 💡 餵食後效果
*   **複雜任務吞吐量**：顯著提升，不再因單一提示詞過長導致邏輯崩潰。
*   **工作流透明度**：各步驟清晰可見，方便人類工程師介入與微調。
*   **穩定性**：因職責分離，單點錯誤不會導致全盤皆墨。
