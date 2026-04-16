# 2007 YRBS 數據分析專案：青少年飲酒行為與體重之統計推論
# (Project: Statistical Inference on Adolescent Alcohol Use and Body Weight)

---

### 👥 團隊資訊 (Group Information)
* **組別 (Group Number)**：Group 16
* **組員名單 (Members)**：
    * 113370240 鍾肇紘
    * 111370231 吳子漢
    * 11337026 盧軒堃

---

### 📊 使用數據 (Dataset)
* **數據集名稱**：2007 年青少年危險行為調查 (Youth Risk Behavior Surveillance System, YRBS)
* **來源**：美國疾病管制與預防中心 (CDC)

---

### 🔍 選定變數 (Selected Variables)
1. **生理性別 (Sex)**：原始編碼為 1 (Female) 與 2 (Male)。
2. **飲酒狀態 (Alcohol Usage)**：將原始 `CurrentAlcoholUse` 變數重編碼為二元變數 `alcohol_binary` (0: 不喝酒, 1: 有喝酒)。
3. **體重 (Weight)**：受訪者不穿鞋的體重數據 (單位：kg)。

---

### 📍 基準值設定 (Benchmark Values)
* **比例分析基準 ($p_0$)**：**0.35** (檢定青少年飲酒比例是否為 35%)。
* **平均數分析基準 ($\mu_0$)**：**68.0 kg** (檢定青少年平均體重是否為 68.0 kg)。

---

### ❓ 研究問題 (Project Questions)
1. **比例推論**：2007 年高中生飲酒的盛行率（Success Rate）是否顯著不同於基準值 **0.35**？
2. **平均數推論**：高中生之平均體重是否顯著不同於基準值 **68.0 kg**？
3. **延伸探索**：生理性別與飲酒行為對於青少年體重是否存在顯著的交互影響？

---

### 💡 最終結論 (Final Conclusion)
* **飲酒比例分析**：經單一樣本 Z 檢定，樣本飲酒比例（45.17%）顯著高於基準值 35% ($p < 0.05$)。
* **體重平均數分析**：經單一樣本 T 檢定，樣本平均體重（68.55 kg）顯著高於基準值 68.0 kg ($p < 0.05$)。
* **分組與交互觀察**：延伸探索發現「生理性別」具備調節效應。在男性組別中，飲酒者平均體重顯著高於非飲酒者；然而在女性組別中，飲酒行為與體重之間並無統計上的顯著差異。

---

## 📂 資料夾結構 (Folder Structure)
* `notebooks/`: 包含數據清洗、EDA 與推論分析的 Jupyter Notebook。
* `outputs/`: 包含高品質視覺化圖表 (.png) 與統計摘要表 (.csv)。
* `references/`: 包含中英文變數定義表與重編碼規則說明文件。
