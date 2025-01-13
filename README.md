# Nigeria-Agricultural-Export-Analysis

## Problem Statement
  This project examines the sales performance, cost analysis, geographic distribution, and performance comparison of Nigeria's agricultural exports
  
## Table of Content
* [Tools](#tools)
* [Data Cleaning and Preparation](#data-cleaning-and-preparation)
* [Exploratory Data Analysis](#exploratory-data-analysis)
* [Modelling](#modelling)
* [Data Analysis](#data-analysis)
* [Visualization](#visualization)
* [Analysis Report and insight](#analysis-report-and-insight)

## Tools
* Execel
* PowerBi

## Data Cleaning and Preparation
Completed the Data cleaning and transformation in excel by removing duplicates and inconsistent data
![image](https://github.com/user-attachments/assets/b3725245-c932-45f7-bd70-4ef706e0eb2c)

## Exploratory Data Analysis
* What are the top-selling products?
* Which company has the highest sales revenue?
* How do sales vary across different export countries? You should look at
* Which destination ports receive the highest volume of exports?
* What are the transportation modes commonly used for export?

## Modelling
After the dataset was cleaned and transformed, it was loaded into Microsoft Power BI Desktop for modeling.
![export 5](https://github.com/user-attachments/assets/efade14e-053f-4381-8707-6f5a5e573043)

## Data Analysis
Measures created for analysis 
``` DAX
2023 COGS = CALCULATE(
    '_measures'[Sum of COGS], 'Import Country'[start of year] = 2023)

2023 profit = CALCULATE(
    '_measures'[sum of profit],'Import Country'[start of year] = 2023)

Revenue by year 2023 = CALCULATE([Total revenue],
'Import Country'[start of year] = 2023)

Sum of COGS = SUM('Product'[COGS])

sum of profit = SUM('Product'[Profit per unit] )

Sum of unit = SUM('Product'[Units Sold] )

Total revenue = SUM('Product'[Export Value])

unit sold 2023 = CALCULATE(
    '_measures'[Sum of unit], 'Import Country'[start of year] = 2023)
```

## Visualization
visualization of data potraying cost analysis, different export company and state performance and timeline analysis
![export 4](https://github.com/user-attachments/assets/092e98e2-c2e9-495d-bcb0-4ccafbaa1925)
![export 1](https://github.com/user-attachments/assets/49e01e0c-3ed2-453f-a304-37fe4063be12)
[Dashboard Report](https://app.powerbi.com/view?r=eyJrIjoiMmNiZjgyNjctYTc4YS00OWIzLWE2MDEtYzM2ZDJiYTRjZWRlIiwidCI6IjI2MTRhZTljLTQ2MmUtNDMyMi05MGE4LWRkMmNkYzYyM2ZjNiJ9)

## Analysis Report and insight

Port Analysis
 * Top Port: Lagos leads in sales volume (of 28,474 units), revenue (with 54.29 % of total revenue), and profitability, followed by Warri (with 17.37 % of revenue, 9,856 units sold and over N100k profit)  and Calabar (12.53 % revenue, 8,351 units sold and over N80k profit).
 * Key Products: Cashew and Cocoa dominate sales and revenue.
 * Recommendations: Optimize Lagos port operations, focus on high-value products, and diversify the product portfolio.
  
Company Analysis
 * Top Performers: Nigeria Agro Export Company, Prime Agro Exports Nigeria Limited, and Solid Agro Nigeria Limited excel in revenue, profit, and unit sales.
 * Key Products: Cashew and Rubber are the most exported.
  
Product Analysis
 * Top Products: Cocoa (with N2.38bn in revenue)and Rubber(with N2.12bn in revenue) lead in revenue, while Sesame dominates sales volume with over 70k units sold.
 * COGS: Cashew has the highest production costs (of over N2bn), indicating room for cost optimization.
  
Import Country Analysis
 * Top Markets: Italy, Denmark, and France rank highest in export value of N1.96bn, N1.83bn and 1.81bn respectively
 * Preferred Port: Lagos is the main hub for exports.

Timeline Analysis
 * Trends: Revenue and unit sales fluctuate, with profit showing mixed results; COGS has generally risen.
  
