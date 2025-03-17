# Plant Co. Sales and Profitability Performance with PowerBI

## Table of Contents
1. [Introduction](#introduction)
2. [Data Content](#data-content)
3. [Data Cleaning Process](#data-cleaning-process)
4. [Dashboard Overview](#dashboard-overview)
5. [Insights & Recommendations](#insights--recommendations)
6. [Conclusion](#conclusion)
7. [Project Files](#project-files)

## Introduction
This project analyzes Plant Co.'s sales and profitability performance using Power BI. The objective is to uncover insights into quantity performance, profitability segmentation, and trends over time to drive strategic decision-making.

## Data Content
The dataset includes:
- **Sales Data**: Transaction-level data for various products.
- **Profitability Metrics**: Gross profit percentages, revenue, and cost details.
- **Time Component**: Monthly breakdown of sales performance.
- **Geographical Distribution**: Sales across different countries.

## Data Cleaning Process
To ensure data accuracy and usability, the following cleaning steps were performed:
1. **Handling Missing Values**: Null values in key fields like sales quantity and revenue were replaced with appropriate estimates or removed.
2. **Standardizing Data Types**: Ensuring numerical fields like revenue and profit percentages were correctly formatted.
3. **Removing Duplicates**: Duplicate records were identified and removed.
4. **Fixing Inconsistencies**: Product names and country names were standardized for consistency.

## Dashboard Overview
The Power BI dashboard presents an interactive view of key performance metrics:

![Dashboard Overview](project%20dash.png)

[Interact with Power BI ](https://github.com/bethelslink/PlantCo-Sales-Analysis-on-PowerBI/blob/main/Performance%20Report.pbix)
### Key Visuals:
- **Top 10 and Bottom 10 Countries**: A bar chart showing performance variations.
- **Year-to-Date (YTD) vs. Prior Year-to-Date (PYTD)**: Comparison of sales performance over time.
- **Product Type Segmentation**: Breakdown of sales by different product categories.
- **Account Profitability Segmentation**: Scatter plot of Gross Profit % vs. Quantity.

## Insights & Recommendations
### Insights:
1. **Overall Growth**: YTD sales have increased by **17.05K units** compared to PYTD, indicating positive performance.
2. **Country Performance**:
   - **China and Sweden** show significant declines.
   - **France and Greece** are leading in growth.
3. **Product Trends**:
   - **Indoor and Landscape products** contribute most to sales.
   - **Outdoor products** show fluctuating demand.
4. **Profitability Segmentation**:
   - A cluster of low-GP% accounts with high sales suggests potential pricing inefficiencies.

### Recommendations:
- **Optimize Pricing Strategy**: Investigate accounts with high quantity but low GP% and adjust pricing accordingly.
- **Market Expansion in High-Performing Countries**: Leverage growth in France and Greece to expand market share.
- **Revamp Sales Strategy in Declining Markets**: Implement targeted marketing efforts in China and Sweden.
- **Focus on High-Margin Products**: Shift marketing and production efforts toward more profitable product categories.

## Conclusion
The dashboard provides valuable insights into Plant Co.’s sales trends, country performance, and profitability segmentation. Implementing the recommendations can improve revenue and operational efficiency.

## Project Files
[RAW Dataset (Excel File)](https://github.com/bethelslink/PlantCo-Sales-Analysis-on-PowerBI/blob/main/Plant_DTS.xls)
[Interact with Power BI ](https://github.com/bethelslink/PlantCo-Sales-Analysis-on-PowerBI/blob/main/Performance%20Report.pbix)


