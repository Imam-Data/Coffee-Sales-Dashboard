# Coffee Shop Sales Analysis Dashboard

## Project Overview
**Role:** Data Analyst  
**Tools:** Microsoft Excel (Pivot Tables, XLOOKUP, Dashboarding)  
**Dataset:** Retail Sales Data (2019 - 2022)

This project analyzes sales transaction data for a coffee shop chain operating in the United States, Ireland, and the United Kingdom. The goal was to transform raw data into an **interactive dashboard** that helps stakeholders track sales performance, identify customer purchasing behaviors, and optimize product inventory.

---

## 📊 Dashboard Preview
![Dashboard Overview](01_Dashboard_Overview.png)
*(Click the image to view the full resolution)*

---

## Business Problem
The company wanted to answer key business questions to improve profitability:
1.  **Sales Trends:** How has the sales performance changed over the years (2019-2022)?
2.  **Product Analysis:** Which coffee type (Arabica, Robusta, etc.) generates the most revenue vs. profit?
3.  **Customer Segmentation:** Who are the top customers and where are they located?
4.  **Seasonality:** Are there specific months with sales spikes that require better inventory planning?

---

## Process & Methodology
To build this dashboard, I performed the following End-to-End Data Analysis process:

### 1. Data Gathering & Cleaning (See: `02_Data_Cleaning_Process.png`)
* Imported 3 separate datasets: **Orders**, **Customers**, and **Products**.
* Checked for missing values (NULLs) and data consistency using Filters.
* Ensured correct data types for Dates and Currency.

### 2. Data Transformation (Excel Formulas)
Merged the datasets into a single "Master Sheet" using complex formulas to enable analysis:
* `XLOOKUP`: To retrieve **Customer Name** and **Country** from the Customer table based on Customer ID.
* `INDEX-MATCH` / `XLOOKUP`: To fetch **Product Price** and **Profit Margin** from the Product table.
* `IF` Functions: Created logical columns for loyalty program segmentation.
* `YEAR` & `MONTH`: Extracted date parts for time-series analysis.

### 3. Data Analysis & Modeling (See: `03_Data_Modeling_Analysis.png`)
Created aggregated Pivot Tables to calculate key metrics:
* **Total Sales & Profit** (KPIs).
* **Sales by Country** (Geographic analysis).
* **Top 5 Customers** (Customer ranking).
* **Sales Trends** (Time-series grouping).

### 4. Visualization & Dashboarding
* Designed a clean, user-friendly interface using a consistent color palette.
* Built **Interactive Charts** (Line, Bar, Donut) connected to Pivot Tables.
* Integrated **Slicers** (Roast Type, Size, Loyalty Card) and **Timeline** to allow users to filter data dynamically.

---

## Key Findings & Insights
Based on the analysis, here are the major findings:

* **🇺🇸 Market Dominance:** The **United States** is the largest market, contributing to over 70% of total revenue, followed by Ireland.
* **Seasonal Spikes:** Sales consistently peak in **Q4 (October - December)**, likely driven by year-end holidays and winter season demand.
* **Product Preferences:** **Arabica** and **Liberica** are the best-selling coffee types. However, **Robusta** offers competitive profit margins despite lower volume.
* **Customer Loyalty:** Top 5 customers contribute significantly to revenue; most high-value customers are enrolled in the Loyalty Card program.

---

## Recommendations
1.  **Inventory Management:** Increase stock levels for **Arabica** coffee starting in September to prepare for the Q4 demand surge.
2.  **Marketing Strategy:** Launch a targeted "US Exclusive" campaign to further penetrate the most profitable market.
3.  **Upselling:** Offer bundle promotions for **Robusta** coffee to increase its sales volume, leveraging its healthy profit margin.

---

## File Structure
* `Coffee_Sales_Dashboard_Analysis.xlsx`: The complete Excel file containing Raw Data, Processing, and Dashboard.
* `01_Dashboard_Overview.png`: Screenshot of the final dashboard.
* `02_Data_Cleaning_Process.png`: Screenshot of the data cleaning/formula process.
* `03_Data_Modeling_Analysis.png`: Screenshot of the Pivot Table/Calculation sheet.

---
*Created by [Nama Kamu]*
