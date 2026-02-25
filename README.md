# 🛒 Super Store Analytics Project

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![Python](https://img.shields.io/badge/Python-Analysis-blue?logo=python)
![Git](https://img.shields.io/badge/Git-Version%20Control-orange?logo=git)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

## 📌 Project Overview

This project analyzes sales, profit, discounts, and returns data for a Super Store in the US. The goal is to uncover business insights, identify risk areas (loss-making and high-discount orders), and present findings through interactive dashboards for stakeholders.

The analysis combines **Python** for data wrangling and exploratory analysis with **Power BI** for interactive reporting and visualization.

---

## 📂 Dataset Description

The dataset is provided as an Excel file: **`super_store_us.xlsx`**, containing three sheets:

* **Orders** – Order-level transactional data (sales, profit, discount, region, dates, etc.)
* **Returns** – Information about returned orders
* **Users** – Manager and regional ownership details

Some insights require joining data across these sheets, which is handled in Python.

---

## 🛠️ Tech Stack

* **Python 3.12**

  * pandas
  * numpy
  * matplotlib / seaborn (for exploratory data analysis)
* **Power BI Desktop** (latest version recommended)
* **Git & GitHub** for version control

---

## 🔄 Data Processing & Transformation (Python)

All data preparation and transformations were done using Python, including:

* Loading and inspecting all three sheets
* Joining Orders, Returns, and Users into a unified dataset
* Handling missing values and standardizing column formats
* Creating derived fields, such as:

  * Returned flag
  * Loss-making orders indicator
  * Profit margin
  * Discount levels
  * Time intelligence fields (Year, Month, Start of Month)
* Preparing a clean, analysis-ready dataset for Power BI

The final processed dataset is exported and used directly in Power BI.

---

## 📊 Power BI Dashboard Overview

The Power BI report is organized into **four pages**, each telling a part of the business story:

### 1️⃣ Sales & Profit Overview

* KPI cards: Total Sales, Total Profit, Return Rate, Loss-Making Orders (with PM and vs PM)
* Sales & Profit trend over time
* Sales vs Previous Month comparison
* Sales by Region

**Purpose:** High-level performance snapshot for executives.

---

### 2️⃣ Loss & Profitability Insights

* Loss breakdown by region and category
* Total loss by category
* Top loss-making orders table

**Purpose:** Identify where and why losses occur.

---

### 3️⃣ Discounts, Returns & Customer Impact

* Discount vs Profit scatter plot
* Returns distribution
* Orders with high discounts & returns table
* Sales by customer segment

**Purpose:** Understand the impact of discounting and returns on profitability.

---

### 4️⃣ Geographic Performance & Executive Summary

* KPI cards: Total Sales, Total Profit, Top Region, High-Risk Orders
* Profitability by state (map)
* Regional sales performance
* High-risk orders summary table

**Purpose:** Geographic insights and consolidated executive view.

## Executive Summary

* The Super Store generated $1.92M in total sales and $224K in total profit, demonstrating solid top-line performance with consistent month-over-month growth.
* Approximately 49% of all orders are loss-making, revealing structural profitability challenges beyond overall revenue performance.
* High discount levels are strongly correlated with negative profit margins, making discounting the primary driver of losses.
* Returned orders, while low in volume, consistently show lower profitability and increase financial risk when combined with aggressive discounting.

## Recommendations

* Establish discount governance thresholds to limit margin erosion, especially for historically unprofitable products and regions.
* Proactively monitor and manage high-risk orders by flagging transactions with deep discounts and high return likelihood.
* Optimize the product and regional portfolio by reallocating focus toward consistently profitable categories and markets.
* Enhance decision-making by extending analytics with predictive risk indicators for profitability and returns.

---

## ▶️ How to Run the Project

### 1. Python (Data Preparation)

1. Ensure Python 3.12 is installed
2. Install required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open the Jupyter Notebook(.ipynb) located in the `notebooks/` directory
4. Run all cells
5. The cleaned dataset will be generated for Power BI use

---

### 2. Power BI Dashboard

1. Open **Power BI Desktop**
2. Load the provided `.pbix` file from the `powerbi/` folder
3. If prompted, refresh the data
4. Use slicers (Region, Date, Customer Segment, Discount, Returned) to explore insights interactively

---

## 📁 Repository Structure

```
OluwasegunRaphael_SuperStore/
│
├── data/
│   └── super_store_us.xlsx
│
├── notebooks/
│   └── superstore_analysis.ipynb
│
├── powerbi/
│   └── SuperStore_Report.pbix
│
├── screenshots/
│   └── dashboard_overview.png
│
└── README.md

---

 ## 👤 Author

**Oluwasegun Raphael**  
Data Analyst & Consultant

---
