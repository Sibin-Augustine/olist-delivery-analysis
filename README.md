# 🚚 Olist E-Commerce Delivery Performance Analysis

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.5+-green.svg)

## 📌 Overview

Comprehensive analysis of ~100,000 orders from Olist, Brazil's largest e-commerce platform, 
to identify factors affecting delivery performance and provide actionable business insights.

## 🎯 Business Questions Answered

1. What percentage of orders are delivered early, on-time, or late?
2. Which geographic regions face the biggest delivery challenges?
3. Do product categories affect delivery time?
4. Does higher freight value guarantee faster delivery?
5. How does delivery performance impact customer reviews?

## 📊 Key Findings

- **92%** of orders delivered early or on-time
- **Northern states** experience delivery times **3x longer** than Southeast
- **1-star reviews** have a **35% late delivery rate** vs only **3%** for 5-star
- Freight value and delivery time are not linearly dependent, however for longer delivery time (>60 days) average freight values is approximately 20-40 BRL
- **GO → GO** is the fastest route (5 days); **CE → AM** is the slowest (100+ days)

## 🖼️ Visualizations

### Overall Delivery Performance

<img width="328" height="317" alt="image" src="https://github.com/user-attachments/assets/0490c8ef-2331-4351-84ef-da081841da32" />



### Route Analysis Heatmap

<img width="661" height="342" alt="image" src="https://github.com/user-attachments/assets/f7e0b9ca-3c8e-4395-b57c-942a3c185137" />


### Freight value vs Delivery time 

<img width="490" height="292" alt="image" src="https://github.com/user-attachments/assets/95d7bb68-fc94-42e6-abc7-e5b0d719d082" />


### Review Score vs Delivery Performance

<img width="491" height="291" alt="image" src="https://github.com/user-attachments/assets/5ce023fd-fbda-4a84-916a-c47a31ef98c8" />


## 🛠️ Tools & Technologies

- **Python 3.9+**
- **Pandas** - Data manipulation
- **Matplotlib & Seaborn** - Visualization
- **Jupyter Notebook** - Analysis environment

## 💡 Recommendations

1. **Regional Warehouses**: Establish fulfillment centers in Northern regions.
2. **Better Delivery Estimates**: Adjust estimated dates for remote destinations.
3. **Category-specific SLAs**: Set realistic delivery times for bulky items.
4. **Freight Subsidy**: Consider partial subsidies for high-cost regions.
5. **Priority Handling**: Flag orders to remote regions for expedited processing.
