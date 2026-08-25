# 🚚 Olist E-Commerce Delivery Performance Analysis

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.5+-green.svg)
![Status](https://img.shields.io/badge/status-completed-brightgreen)

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YTpcOW0EoMT7Xg_1ikVNoFrvmuDJepFX#scrollTo=kIgjBWqU_p-5)

Analyzed 100K+ Brazilian e-commerce orders to uncover why 8% arrive late — and how to fix it with 5 data-backed recommendations.

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Problem Statement](#-problem-statement)
- [Dataset](#-dataset)
- [Methodology](#-methodology)
- [Key Findings](#-key-findings)
- [Visualizations](#-visualizations)
- [Recommendations](#-recommendations)
- [Business Impact](#-business-impact)
- [Skills Demonstrated](#-skills-demonstrated)
- [Tools & Technologies](#-tools-&-technologies)

## 📌 Overview

Comprehensive analysis of ~100,000 orders from Olist, Brazil's largest e-commerce platform, 
to identify factors affecting delivery performance and provide actionable business insights.

## 🎯 Business Questions

1. What percentage of orders are delivered early, on-time, or late?
2. Which geographic regions face the biggest delivery challenges?
3. Do product categories affect delivery time?
4. Does higher freight value guarantee faster delivery?
5. How does delivery performance impact customer reviews?

## 🔬 Methodology
1. **Data Cleaning**: Handled X missing values, removed Y outliers...
2. **Feature Engineering**: Created delivery_days, delivery_status, route columns
3. **EDA**: Univariate → Bivariate → Multivariate analysis
4. **Statistical Testing**: Chi-square for categorical, correlation for numeric
5. **Visualization Strategy**: Chose X because Y

## 📊 Key Findings

- **92%** of orders delivered early or on-time
- **Northern states** average **21 days** delivery vs. **7 days in Southeas**t (3x slower), affecting ~8% of orders but generating 35% of complaints
- **1-star reviews** have a **35% late delivery rate** vs only **3%** for 5-star
- Freight value and delivery time are not linearly dependent, however for longer delivery time (>60 days) average freight values is approximately 20-40 BRL
- **GO → GO** is the fastest route (5 days); **CE → AM** is the slowest (100+ days)

## 🖼️ Visualizations

### Overall Delivery Performance

<img width="328" height="317" alt="image" src="https://github.com/user-attachments/assets/0490c8ef-2331-4351-84ef-da081841da32" />

> **🗺️ Insight**: 92% early delivery rate looks great — but it's actually a red flag for inflated ETAs. Recalibrating delivery estimates could improve conversion rates without harming actual performance

---

### Route Analysis Heatmap

<img width="661" height="342" alt="image" src="https://github.com/user-attachments/assets/f7e0b9ca-3c8e-4395-b57c-942a3c185137" />

> **🗺️ Insight:** Delivery times vary dramatically by route, ranging from 5 days (GO→GO) to 20+ days for cross-country shipments. Same-state deliveries (diagonal cells) consistently show the fastest times (6–11 days), while shipments to Northern/Northeastern states (AM, PA, CE) take 2–3x longer regardless of origin. This confirms that geographic distance and infrastructure gaps — not seller performance — are the primary bottleneck.

---

### Freight value vs Delivery time 

<img width="491" height="290" alt="image" src="https://github.com/user-attachments/assets/1e31bd15-1585-44c3-870e-36fc585ab5db" />

> **💰 Insight:** The distribution forms a triangular pattern — within 20 days, freight values span the entire range (0–60 BRL), but beyond 40 days, low-cost freight (<15 BRL) virtually disappears.

---

### Review Score vs Delivery Performance

<img width="491" height="291" alt="image" src="https://github.com/user-attachments/assets/5ce023fd-fbda-4a84-916a-c47a31ef98c8" />

> **⭐ Insight:** There's a clear inverse relationship between delivery time and customer satisfaction. Median delivery time drops from ~14 days for 1-star reviews to ~10 days for 5-star reviews, and the spread of outliers shrinks dramatically as scores improve. Notably, 1-star reviews show extreme variance (some deliveries taking 55+ days), while 5-star reviews are tightly clustered under 25 days.

---

## 💡 Recommendations

1. **Regional Warehouses**: Establish fulfillment centers in Northern regions.
2. **Better Delivery Estimates**: Adjust estimated dates for remote destinations.
3. **Category-specific SLAs**: Set realistic delivery times for bulky items.
4. **Freight Subsidy**: Consider partial subsidies for high-cost regions.
5. **Priority Handling**: Flag orders to remote regions for expedited processing.

## 💰 Estimated Business Impact
- Implementing Northern warehouse → **~40% delivery time reduction**
- Better SLA estimates → potential **15% increase in 5-star reviews**
- Freight optimization → **R$ X savings per order** on remote routes


## 🎯 Skills Demonstrated
- **Data Wrangling**: Merged 9 relational tables (orders, customers, reviews...)
- **EDA**: Univariate, bivariate, geospatial analysis
- **Statistical Analysis**: Correlation, hypothesis testing
- **Data Visualization**: Matplotlib, Seaborn, heatmaps, scatter plots
- **Business Acumen**: Translated data patterns into actionable recommendations
- **Storytelling**: Structured findings for non-technical stakeholders

## 🛠️ Tools & Technologies

- **Python 3.9+**
- **Pandas** - Data manipulation
- **Matplotlib & Seaborn** - Visualization
- **Jupyter Notebook** - Analysis environment
