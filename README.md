# 2007 YRBS 數據分析專案：青少年飲酒行為與體重之統計推論
# (Project: Statistical Inference on Adolescent Alcohol Use and Body Weight)

---

### 👥 團隊資訊 (Group Information)
* **組別 (Group Number)**: Group 16 / 第 16 組
* **組員名單 (Members)**: 
    * 113370240 鍾肇紘
    * 111370231 吳子漢
    * 11337026 盧軒堃

---

### 📊 使用數據 (Dataset)
* **數據集名稱 (Dataset Name)**: 2007 Youth Risk Behavior Surveillance System (YRBSS) / 2007 年青少年危險行為調查
* **來源 (Source)**: Centers for Disease Control and Prevention (CDC) / 美國疾病管制與預防中心

---

### 🔍 選定變數 (Selected Variables)
1. **生理性別 (Biological Sex)**: Original codes: 1 (Female) and 2 (Male) / 原始編碼：1 (女性) 與 2 (男性)。
2. **飲酒狀態 (Alcohol Usage Status)**: Recoded `CurrentAlcoholUse` into a binary variable `alcohol_binary` (0: No Use, 1: Any Use) / 將原始飲酒天數重編碼為二元變數 `alcohol_binary` (0: 不喝酒, 1: 有喝酒)。
3. **體重 (Weight)**: Respondent's weight without shoes in kilograms (kg) / 受訪者不穿鞋之體重數據 (單位：kg)。

---

### 📍 基準值設定 (Benchmark Values)
* **比例分析基準 (Proportion Benchmark $p_0$)**: **0.35**
* **平均數分析基準 (Mean Benchmark $\mu_0$)**: **68.0 kg**

---

### ❓ 研究問題 (Project Questions)
1. **比例推論 (Proportion Inference)**: Is the drinking prevalence among high school students in 2007 significantly different from the benchmark of **0.35**? / 2007 年高中生飲酒的盛行率是否顯著不同於基準值 **0.35**？
2. **平均數推論 (Mean Inference)**: Is the average weight of high school students significantly different from the benchmark of **68.0 kg**? / 高中生之平均體重是否顯著不同於基準值 **68.0 kg**？
3. **延伸探索 (Extended Exploration)**: Does biological sex moderate the relationship between alcohol consumption and body weight? / 生理性別與飲酒行為對於青少年體重是否存在交互影響？

---

### 💡 最終結論 (Final Conclusion)
* **飲酒比例 (Alcohol Proportion)**: Based on the one-sample Z-test, the sample proportion (45.17%) is significantly higher than the benchmark of 35% ($p < 0.05$) / 經單一樣本 Z 檢定，樣本飲酒比例 (45.17%) 顯著高於基準值 35% ($p < 0.05$)。
* **體重平均數 (Weight Mean)**: Based on the one-sample T-test, the sample mean weight (68.55 kg) is significantly higher than the benchmark of 68.0 kg ($p < 0.05$) / 經單一樣本 T 檢定，樣本平均體重 (68.55 kg) 顯著高於基準值 68.0 kg ($p < 0.05$)。
* **交互觀察 (Interaction Observations)**: Biological sex acts as a key moderator. A significant difference in weight between drinkers and non-drinkers was found in males, while no statistically significant difference was observed in females / 生理性別具備調節效應。在男性組別中，飲酒者體重顯著高於非飲酒者；然而在女性組別中，飲酒行為與體重之間並無統計上的顯著差異。

---

## 📂 資料夾結構 (Folder Structure)
* `notebooks/`: Jupyter Notebooks for data cleaning, EDA, and inference / 包含數據清洗、EDA 與推論分析之程式稿。
* `outputs/`: High-resolution figures (.png) and statistical summary tables (.csv) / 包含視覺化圖表與統計摘要表。
* `references/`: Variable definitions and recoding rules in both English and Chinese / 包含中英文變數定義表與重編碼規則說明。
