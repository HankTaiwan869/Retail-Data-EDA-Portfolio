# Retail-Data-EDA-Portfolio

# Exploring the Impact of Promotional Discounts on Sales Performance

## Overview
This project explores the effectiveness of promotional discounts on weekly sales using a real-world anonymized retail dataset.

## Goal
The analysis aims to support retail decision-making by identifying which markdown types are most effective for each store type, and over what time windows their impact is most apparent.

## Dataset
The dataset is a real Amazon anonimyzed retail datasets contains 3 tables, totalling more than 400,000 rows and 16 unique variables. It includes 5 markdown volumes, weekly sales, store types (A, B, C), and other factors. Markdown volumes represent promotional discounts applied each week across five (anonymized) categories.

## Key Questions
- Do promotions correlate with higher weekly sales?
- Is the store type a major factor in sales and promotion effects?
- Over what time window (in weeks) should sales be measured to best capture the effects of promotions?

## Key Findings
### Store Types patterns?
- Store types A and B demonstrate similar sales patterns while Type C is unique.
- Store Type also strongly affects the effectiveness of promotional strategies.
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
