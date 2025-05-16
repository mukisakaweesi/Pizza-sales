# 🍕 Pizza Sales Analysis Dashboard

### 🔍 Project Description

This project explores and analyzes a year's worth of pizza sales data using **SQL** for analysis and **Power BI** for visualization. The goal is to uncover trends in revenue, order frequency, product performance, and customer preferences. The final dashboard delivers clear insights into sales performance by category, size, time, and day of the week — empowering business decision-makers in the food and beverage space.

---

## 📚 Table of Contents
1. [Project Overview](#1-project-overview)  
2. [Data Sources](#2-data-sources)  
3. [Tools Used](#3-tools-used)  
4. [Data Cleaning and Preparation](#4-data-cleaning-and-preparation)  
5. [Exploratory Data Analysis (EDA)](#5-exploratory-data-analysis-eda)  
6. [Data Analysis](#6-data-analysis)  
7. [Results & Findings](#7-results--findings)  
8. [Recommendations](#8-recommendations)  
9. [Limitations](#9-limitations)  
10. [References](#10-references)

---

## 1. Project Overview

The purpose of this project is to analyze sales performance for a pizza restaurant, with the aim of identifying best-selling products, busiest sales periods, and customer purchasing behavior. The insights are visualized in a Power BI dashboard to help managers make data-driven decisions to boost revenue and streamline operations.

---

## 2. Data Sources

- **Dataset**: `pizza_sales.csv`  
- Data covers all pizza orders from **January to December 2015**
- Key columns: `order_id`, `order_date`, `pizza_name`, `pizza_size`, `pizza_category`, `quantity`, `total_price`

---

## 3. Tools Used

- **MySQL** – Data querying and analysis  
- **Power BI Desktop** – Interactive data visualization  
- **Microsoft Excel** – Data formatting and CSV structure validation  

---

## 4. Data Cleaning and Preparation

- Removed duplicate rows and ensured data types were consistent (e.g., date fields, numeric totals)  
- Standardized pizza category and size naming conventions  
- Checked for and handled null or invalid entries (e.g., missing prices or sizes)  
- Created new fields for:
  - Month and day name for trend analysis
  - Revenue metrics
  - Aggregated quantities and totals by category and size

---

## 5. Exploratory Data Analysis (EDA)

Using **MySQL**, the following metrics were computed:

- **Total Revenue**  
```sql
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;
```
## 6. Data Analysis
Using SQL and Power BI:

Calculated KPIs: total revenue ($817.9K), total orders (21K), total pizzas sold (50K), average order value ($38.31), and average pizzas per order (2.32)

Tracked daily and monthly order trends to identify peak sales periods

Analyzed percentage of sales by pizza category and size

Identified top 5 and bottom 5 performers based on:

Revenue

Quantity sold

Number of orders

Evaluated performance by pizza size and category using bar and pie charts

Visualized key metrics using card visuals, line charts, and clustered columns

---
## 7. Results & Findings
Revenue: Total revenue generated was $817.9K

Order Volume: 21K orders processed in 2015, totaling 50K pizzas

Top Sales Days: Highest orders occurred on Fridays, Saturdays, and Sundays

Top Months: Peak sales occurred between January and July

Category Performance:

Classic category had the highest contribution to revenue

Chicken and Veggie categories closely followed

Size Performance:

Large (L) pizzas made up 45.9% of total sales

Medium (M) and Small (S) sizes followed at 30.5% and 21.8% respectively

---

## 8. Recommendations
Stock & promote large-sized pizzas more aggressively due to higher demand

Focus marketing efforts on the weekend, particularly Friday–Sunday

Optimize menu based on the top 5 best sellers and consider phasing out the lowest performers

Run seasonal promos from January to July to boost already strong months

Consider offering combo deals or discounts to increase average order value above $38

---
## 9. Limitations
Data only includes one year (2015); long-term trends unavailable

No customer-level data for deeper behavioral segmentation (e.g., repeat buyers)

External factors such as weather, holidays, or marketing campaigns were not accounted for

Pizza customization or toppings data not available
---

##10. References
Power BI Documentation

MySQL Documentation
---

Pizza Sales Dashboard Inspiration – SQLBI
