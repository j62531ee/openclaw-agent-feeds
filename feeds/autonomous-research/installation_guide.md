# 🛠 安裝指令 (Feed Prompt)

請直接將以下指令發送給負責資料研究的代理，啟動「深度研究模式」。

---

```xml
<lobster_upgrade_module id="autonomous_research_v1">
    <research_loop>
        1. 初始檢索 (Initial Search)：針對目標問題進行廣泛搜索。
        2. 資訊過濾 (Filtering)：排除過期或明顯偏頗的資料。
        3. 交叉比對 (Cross-Referencing)：從至少兩個獨立來源驗證關鍵數據。
        4. 迭代優化 (Iteration)：若發現資訊衝突，則針對衝突點發起二閃搜尋 (Secondary Search)。
    </research_loop>

    <verification_tags>
        - [VERIFIED_SRC]: 已通過交叉驗證的資訊。
        - [SINGLE_SRC]: 僅有單一來源的資訊（需標註不確定性）。
        - [CONFLICT_REPORT]: 資訊不一致時的詳細說明。
    </verification_tags>

    <citation_requirement>
        所有關鍵主張必須附帶原始網址或出處名稱。
    </citation_requirement>
</lobster_upgrade_module>
```

---

### 💡 餵食後效果
*   **數據精準度**：大幅減少 AI 因記憶錯亂產生的「幻覺」數據。
*   **報告深度**：從表格化的數據轉變為具備論點支持的深度報告。
*   **搜尋效率**：減少亂無章法的隨機檢索，集中於有價值的資訊點。
