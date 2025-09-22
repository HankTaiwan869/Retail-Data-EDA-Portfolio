[Scroll down for English version.]

# 零售促銷：促銷折扣對銷售成效的EDA作品集

## 簡介
本作品集探討促銷折扣對每週銷售額的影響，使用的是一份真實的去識別化零售資料集，聚焦於探討**哪些降價策略能帶來可衡量的銷售提升，以及其效果在何時最為明顯**，協助零售決策，辨識出對不同商店類型最有效的促銷方式，以及適合的檢驗時間窗口。

## 資料集
資料集來源為 Amazon 提供的去識別化零售資料，包含 3 個資料表，總計超過 40 萬筆資料與 16 個變數。內容涵蓋 5 種降價活動(Markdown 1-5)、每週銷售額、商店類型（A、B、C），以及其他影響因素。降價活動的數值代表每週於五個（去識別化後的）促銷類別上實際施行的折扣量。

## 主要發現  
### 哪些促銷方式最有效？
- 對於 A、B 類型商店，**降價活動 3 與 5** 對銷售有明顯影響，其中 **降價活動 5 的投資報酬率（ROI）最高**。  
- 對於 C 類型商店，僅有 **降價活動 1** 對銷售有明顯影響，其餘不顯著。  
### 應該在什麼時間窗口觀察促銷效果？
- A、B 類型商店：促銷效果在 **4–5 週移動平均(forward moving average)**下最為明顯。  
- C 類型商店：**降價活動 1** 的效果在 **5–6 週移動平均**下最強。  

## 商業建議
### 對 A、B 類型商店
- 將預算從 **降價活動 1 與 4** 轉移至 **降價活動 3 與 5**。  
- 特別建議加大對 **降價活動 5** 的投入（ROI 高且underutilized）。  
- 使用 **4–5 週移動平均**來評估降價活動 3 與 5 的效果。  
### 對 C 類型商店
- 將預算從 **降價活動 3 與 4** 轉移至 **降價活動 1 與 5**。  
- 使用 **5–6 週移動平均**來評估降價活動 1 的效果。  

資料來源: https://www.kaggle.com/datasets/manjeetsingh/retaildataset/data

-----------------------------------------------------------------


# Exploring the Impact of Promotional Discounts on Sales Performance

## Overview
This project explores the effectiveness of promotional discounts on weekly sales using a real-world anonymized retail dataset. The analysis aims to support retail decision-making by identifying which markdown types are most effective for each store type, and over what time windows their impact is most apparent.

## Dataset
The dataset is a real Amazon anonymized retail datasets contains 3 tables, totalling more than 400,000 rows and 16 unique variables. It includes 5 markdown volumes, weekly sales, store types (A, B, C), and other factors. Markdown volumes represent promotional discounts applied each week across five (anonymized) categories.

## Key Findings
### Which Markdown Events work (the best)?
- For Store Types A and B, Markdown events 3 and 5 have significant effects on sales while the others don't. Markdown 5 has the highest ROI (Return on Investment) among all promotion types.
- For Store Type C, only Markdown 1 has statistically significant effects on sales while the others don't.
### When should we measure the effects of the promotional events?
- For Store Type A, B, Promotional effects are strongest when measured using 4 or 5 week rolling averages.
- For Store Type C, the effects of Markdown 1 is strongest when measured using 5-6 week rolling averages.

## Business Recommendation
### For Store Type A and B, 
- Reallocate budget *away from* Markdown 1 and 4 *to* **Markdown 3 and 5**.
- Invest especially more in **Markdown 5** (higher ROI and underutilized).
- Measure the effects of Markdown 3 and 5 using **4-5** forward rolling averages of weekly sales.
### For Store Type C, 
- Reallocate budget *away from* Markdown 3 and 4 *to* **Markdown 1 and 5**.
- Measure the effects of Markdown 1 using **5-6** forward rolling averages of weekly sales.

Data source: https://www.kaggle.com/datasets/manjeetsingh/retaildataset/data
