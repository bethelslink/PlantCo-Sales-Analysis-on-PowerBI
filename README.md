# Plant Co. Sales and Profitability Analysis

## Table of Contents

1. [Introduction](#introduction)
2. [Data](#data)
    * [Understanding the Data](#understanding-the-data)
    * [Data Cleaning](#data-cleaning)
    * [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
        * [Sales Trend Analysis](#sales-trend-analysis)
        * [Most and Least Profitable Products](#most-and-least-profitable-products)
        * [Regional Sales Distribution](#regional-sales-distribution)
3. [Dashboard Overview](#dashboard-overview)
    * [How Each Visualization Was Created](#how-each-visualization-was-created)
4. [Key Metrics](#key-metrics)
5. [Key Insights](#key-insights)
6. [Recommendations](#recommendations)
7. [Conclusion](#conclusion)
8. [File Links](#file-links)

## Introduction

This report presents the analysis of Plant Co.'s sales and profitability performance for the year 2023. The primary focus is on sales trends, profitability, and regional performance, aimed at providing data-driven insights to enhance business strategy.

Plant Co. is engaged in the sale and distribution of plant-related products, including indoor, landscape, and outdoor plants. The company operates in multiple countries, supplying a diverse range of plant products to various markets.

## Data

### Understanding the Data

The dataset comprises three tables:

* **Plant FACT (Main Sales Data)**
    * Product ID – Unique identifier for each product.
    * Sales USD – Total sales in USD.
    * Quantity – Number of units sold.
    * Price USD – Price per unit in USD.
    * COGS USD – Cost of Goods Sold (COGS) in USD.
    * Date Time – Transaction date.
    * Account ID – Links to the Accounts table.
* **Accounts (Customer/Location Data)**
    * Country Code, Country Name – Country details.
    * Account – Customer or business name.
    * Master ID, Account ID – Identifiers for accounts.
    * Latitude, Longitude – Geographical location.
    * Postal Code, Street Name, Street Number – Address details.
* **Plant Hierarchy (Product Classification)**
    * Product Family, Product Family ID – High-level product category.
    * Product Group, Product Group ID – Sub-category of products.
    * Product Name, Product Name ID – Specific product names.
    * Product Size – Size classification (Small, Medium, Large).
    * Product Type – Type of product (Landscape, Outdoor, etc.).

### Data Cleaning

Steps taken to clean the data:

* Checked for missing values, incorrect data types, duplicates, and inconsistencies.
* **Missing Values:** 796 missing Account IDs were removed from the Accounts dataset.
* **Duplicates:** No duplicate rows found.
* Ensured Date Time in Plant FACT is in the correct datetime format.
* Standardized column names (e.g., corrected Product Type naming inconsistencies).

### Exploratory Data Analysis (EDA)

#### Sales Trend Analysis

The sales trend over time showed fluctuations, with noticeable spikes, indicating seasonal demand or promotional events.

#### Most and Least Profitable Products

* **Top 10 Most Profitable Products:** The most profitable product (Product ID 2940) generated $43,880 in profit, with others ranging from $34,269 to $43,880.
* **Top 10 Least Profitable Products:** The least profitable product (Product ID 2401) had only $803 in profit, with several products generating below $1,500.

#### Regional Sales Distribution

Top 3 countries by sales:

1. China – $9,986,710
2. Brazil – $2,259,971
3. Philippines – $2,065,942

The United States ranked 8th with $1,129,565 in sales.

## Dashboard Overview

![Dashboard Overview](project%20dash.png)

[Interact with Dashboard ](https://github.com/bethelslink/PlantCo-Sales-Analysis-on-PowerBI/blob/main/Performance%20Report.pbix)


The dashboard provides an analysis of Plant Co.'s quantity performance in 2023, comparing Year-to-Date (YTD) vs. Prior Year-to-Date (PYTD) sales trends. It includes country-wise performance, monthly trends, product type segmentation, and profitability insights.

### How Each Visualization Was Created

1. **KPI Cards (Top Summary)**
    * Metrics: YTD Quantity (555.66K), YTD vs PYTD Difference (17.05K), PYTD Quantity (538.61K), Gross Profit Percentage (39.62%).
    * Calculations: YTD Quantity = Sum of quantity for the current year; PYTD Quantity = Sum of quantity for the same period last year; GP% = ((Sales USD - COGS USD) / Sales USD) * 100.

2. **Bottom 10 Countries (Left Heatmap)**
    * Shows the lowest YTD vs PYTD performance.
    * Built using grouped data by country, sorted by bottom 10 values, with a heatmap gradient.

3. **Waterfall Chart (Quantity YTD vs PYTD by Month)**
    * Displays monthly quantity changes.
    * Positive (green) represents increases, negative (red) represents decreases.

4. **Column & Line Chart (Quantity YTD & PYTD by Month)**
    * Stacked bars for Indoor, Landscape, Outdoor product types.
    * A red line represents PYTD Quantity.

5. **Scatter Plot (Account Profitability Segmentation)**
    * Each dot represents an account.
    * X-axis: Value YTD; Y-axis: GP%; Dot size: Sales USD.

## Key Metrics

* YTD Quantity Sold: 555.66K
* YTD vs. PYTD Difference: 17.05K
* PYTD Quantity Sold: 538.61K
* Gross Profit Percentage (GP%): 39.62%

## Key Insights

1. **Overall Growth in Sales Volume:** Sales increased by 17.05K units compared to the previous year, with a stable GP% of 39.62%.
2. **Declining Market Performance in Certain Regions:** China (-9.76K), Sweden (-6.71K), and Japan (-3.74K) saw significant declines.
3. **Seasonal Sales Variations:** Peak months: April (52.26K), May (49.71K), and December (48.63K). Lowest month: September (37.2K).
4. **Product Type Contribution to Sales:** Indoor plants contributed the most to total sales.

## Recommendations

1. **Expand High-Performing Products:** Increase production and marketing for the most profitable products.
2. **Address Regional Declines:** Implement targeted promotional campaigns in underperforming regions.
3. **Optimize Inventory Management:** Prepare for peak seasons based on sales trends.
4. **Improve Low-Profit Products:** Assess pricing and cost structures for low-margin products.

## Conclusion

Plant Co. experienced overall sales growth in 2023, with a stable gross profit percentage. However, regional market declines and low-profit products require strategic interventions to maximize future profitability.

## File Links

[RAW Dataset (Excel File)](https://github.com/bethelslink/PlantCo-Sales-Analysis-on-PowerBI/blob/main/Plant_DTS.xlsx)
[Interact with Power BI ](https://github.com/bethelslink/PlantCo-Sales-Analysis-on-PowerBI/blob/main/Performance%20Report.pbix)


