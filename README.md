# Enterprice_Snowflake_DW_BI_Dashboard


## 📌 Overview

This project simulates a full data pipeline: from generating raw data to loading it into Snowflake, performing SQL-based analytics, and visualizing insights using Power BI. It covers the core lifecycle of data engineering and analytics with hands-on SQL, Python, and Snowflake tools.

---

## 🔧 Tech Stack

* **Python (Pandas, Faker)** – for simulating and generating datasets
* **Snowflake (Snowsql, SQL Workbook)** – for data warehousing
* **Power BI** – for building interactive dashboards and visualizations

---

## 🗃️ Data Modeling

* Implemented a **Snowflake Schema**:

  * Fact Table: `FactOrders`
  * Dimension Tables: `DimCustomer`, `DimProduct`, `DimDate`, `DimStore`, `DimLoyaltyProgram`
* Created and loaded synthetic data using `Faker` and Python scripts

![image](https://github.com/user-attachments/assets/d394dde7-18c9-42fb-88e1-aa2a1d96efb8)



---

## 📥 Data Loading

1. Created file formats and stages in Snowflake (`FILE FORMAT`, `STAGE`)
2. Used `PUT` and `COPY INTO` commands to upload CSV files from local machine to internal stage
3. Loaded data from stage into Snowflake tables using `COPY INTO` with proper formatting

---

## 📊 Key Analytics Performed (SQL)

* Identify **customers inactive** in the last 30 days
* Show **top 3 brands by sales** over the last year
* Get **monthly sales** for 2024
* Count **loyal customers** who purchased 3+ categories in the past 6 months
* Aggregate **sales by region and category**
* Analyze **store performance** after opening
* Calculate **discount/shipping cost impact** on order totals
* Apply **RANK() vs ROW\_NUMBER()** for comparative analysis

---

## 📈 Power BI Dashboard

* Connected Snowflake data to Power BI
* Created KPIs like:

  * Total Order Amount
  * Average Order Value
  * Total Customers
  * Total Discounts and Shipping Costs
* Built Age Distribution visuals using DAX logic

  * Grouped ages into 7 brackets: Minor, 18–24, 25–34, ..., Above 64


## ✅ Learnings & Highlights

* Hands-on with end-to-end ELT using Snowflake and Snowsql
* Practical SQL for business insights
* Power BI integration for real-time storytelling



