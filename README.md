# Seasonal Agriculture Performance Analysis

A data analytics project analyzing how agricultural performance varies across seasons, using a farm-level dataset covering seasons, states, crops, and irrigation methods across India. Completed as the major project for the VOIS AICTE Internship (Data Visualization track).

## Problem Statement

Agricultural performance is influenced by seasonal variations in environmental conditions, farming practices, resource availability, and market conditions. Raw agricultural data does not clearly explain how performance changes across seasons. This project analyzes seasonal agricultural data to identify meaningful patterns, trends, relationships, and variations in performance across seasons.

## Dataset

- **Records:** 4,000 farm-level entries
- **Features:** 28 columns
- **Seasons covered:** Kharif, Rabi, Zaid
- **Coverage:** 8 Indian states, 8 crops, 4 irrigation methods
- **Variables:** environmental conditions (rainfall, temperature, humidity, soil), farming inputs (fertilizer, pesticide, water use), and economic outcomes (yield, cost, revenue, profit)

## Tools & Technologies

- Python (Google Colab / Jupyter Notebook)
- Pandas, NumPy — data cleaning and analysis
- Matplotlib, Seaborn — data visualization
- IQR method — outlier detection

## Project Workflow

1. **Data Loading & Cleaning** — handled missing values (median imputation by season) and verified no duplicate records
2. **Feature/Variable Review** — categorized all 28 columns into identifier, environmental, input, and outcome variables
3. **Outlier Detection** — investigated and justified retaining natural crop-scale outliers
4. **Univariate Analysis** — distribution of categorical and numeric variables
5. **Bivariate Analysis** — seasonal comparison of yield, cost, revenue, and profit
6. **Multivariate Analysis** — correlation heatmap, profit by crop and season, irrigation method impact
7. **Additional Student-Designed Analyses:**
   - Regional consistency of seasonal patterns
   - Disease/pest risk vs. profitability
   - Water-use efficiency across seasons
8. **Key Insights** — 9 documented insights, each with observation, evidence, interpretation, and limitation
9. **Recommendations & Conclusion** — evidence-based, data-supported recommendations

## Key Findings

- **Kharif** is the strongest-performing season across all metrics and all 8 states (Yield 5.63 t/ha, Profit ₹178,915).
- **Zaid** is the only season with a negative average profit (-₹24,805), despite having the highest average cost.
- **Irrigation method** strongly affects seasonal profit — Drip irrigation stays profitable in every season, while Flood and Rainfed irrigation turn unprofitable in Zaid.
- **Zaid** uses the most water (6,419.89 m³) but has the lowest water efficiency (4.41 t/1000m³) of all three seasons.
- **Disease/pest risk does not explain** Zaid's weaker performance — Kharif has the highest pest risk (54.47%) yet remains the most profitable season.
- **Chilli and Sugarcane** are the most consistently profitable crops across all seasons.

## Recommendations

1. Prioritize Drip irrigation in Zaid season.
2. Target water-efficiency improvements at Zaid-season farms.
3. Give closer attention to Zaid-season farming in Gujarat and Andhra Pradesh.
4. Consider Chilli and Sugarcane where crop choice is flexible.
5. Do not prioritize pest/disease control as the primary fix for Zaid's weaker performance.

## Limitations

- Zaid season has a smaller sample size (594 records) compared to Kharif (1,779) and Rabi (1,627).
- The dataset covers a single time period, with no year-over-year data to confirm consistency.
- All relationships identified are associative, not causal.

## Author

**Aakriti Sharma**
