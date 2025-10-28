# Kaggle 汽車資料集多元線性回歸分析

本專案以 Kaggle「Automobile Dataset」為基礎，依 CRISP-DM 標準流程，實現汽車價格之多元線性回歸預測，涵蓋資料前處理、特徵選擇、建模、評估與應用建議，適用於資料科學、機器學習教學及入門實作。

---

## 專案流程（CRISP-DM）

1. **Business Understanding（商業理解）**  
   明確預測目標：瞭解汽車資料集，協助分析車價影響因子，並以預測價值輔助決策。

2. **Data Understanding（資料理解）**  
   載入資料集，檢視各特徵分布、資料型態與缺值，建立對資料的基本認識。

3. **Data Preparation（資料準備）**  
   完成缺值處理、型態轉換、類別特徵編碼、特徵選擇，確保資料可供回歸建模。

4. **Modeling（建模）**  
   以多元線性回歸模型建構預測流程，利用 SelectKBest 進行特徵篩選，提高模型效能。

5. **Evaluation（評估）**  
   利用 R²、MSE、RMSE 等指標評估模型表現；繪製實際與預測價格圖並標示信賴區間。

6. **Deployment（部署/應用）**  
   說明模型預期應用範疇，舉例於汽車銷售策略、產品定價情境，並建議如何持續優化。

---

## 資料集資訊

- **來源**：[Kaggle Automobile Dataset](https://www.kaggle.com/datasets/toramky/automobile-dataset)
- **檔案**：Automobile_data.csv
- **特徵數量**：約 26 欄（包含車輛技術規格與售價）

---

## 執行說明

1. 請先下載並置於專案根目錄：`Automobile_data.csv`
2. 使用 Jupyter Notebook (.ipynb) 開啟本程式，並依順序執行每個 cell
3. 程式自動執行資料前處理、特徵選擇、建模、模型評估與成果視覺化
4. 詳細中文註解與分段，便於理解每步操作

---

## 成果摘要

- 多元線性回歸模型預測汽車價格，選用 24 個高分特徵。
- 模型評估指標：
     - MSE（均方誤差）: 12,663,837.77
     - RMSE（均方根誤差）: 3,558.63
     - R²（解釋力）: 0.89
- 預測成果視覺化：
<img width="713" height="470" alt="image" src="https://github.com/user-attachments/assets/aed27cf3-3c75-4624-b54e-b9206a5faa4f" />

- 圖中紅色虛線表示理想預測（實際=預測），灰色區塊為95%信賴區間，展示預測信度。
---

## 參考來源

資料集：[Kaggle Automobile Dataset](https://www.kaggle.com/datasets/toramky/automobile-dataset)  
CRISP-DM 流程說明：[資料探勘（國立中山大學推廣中心）](https://lis.nsysu.edu.tw/static/file/1/1001/attach/1/pta_87883_5685077_33615.pdf)
