# 🍬 Candy ETL Project

## 📌 Project Overview

The **Candy ETL Project** is a full-stack data pipeline and business intelligence project built using a dataset extracted from **Kaggle**. The aim was to perform end-to-end **data cleaning**, **exploratory data analysis (EDA)**, and **visualization** to gain insights into candy sales and shipping performance across various regions.

---

## ⚙️ Tools & Technologies Used

- 🐍 **Python**: Data cleaning and preprocessing (Pandas, NumPy)
- 🔍 **Google BigQuery**: Exploratory Data Analysis (SQL queries)
- 📊 **Business Intelligence Tool**: Data visualization and dashboard creation (e.g., Looker Studio / Tableau / Power BI)
- 🗂️ **Kaggle**: Dataset source

---

## 🧹 Data Cleaning (Python)

Performed in Python using **Pandas**, including:

- Handling missing values
- Standardizing date formats (`Order_Date`, `Correct_shipdate`)
- Creating new columns such as `Orders_delay` and `Shipping_years`
- Converting data types (e.g., `Sales`, `Gross_Profit` to float64)
- Renaming columns for clarity

---

## 🔍 Exploratory Data Analysis (BigQuery)

EDA was done using **Google BigQuery**, focusing on:

- Sales trends across different regions and factories
- Shipping delays by `Ship_Mode`
- Factory-wise gross profit and unit economics
- Identifying top-selling products and peak order months



## 📈 Business Intelligence Dashboard

The cleaned and transformed data was visualized using a BI tool to uncover:

- 🔝 Top-performing factories
- 🛳️ Shipping mode efficiency
- 📦 Product-wise revenue breakdown
- 🗺️ Regional sales distribution (map visuals using `Latitude` & `Longitude`)

---

## 📁 Dataset Features
---

| **Column Name**        | **Data Type**         | **Description**                                  |
|------------------------|-----------------------|--------------------------------------------------|
| `Row_ID`               | `int64`               | Unique row identifier                            |
| `Order_ID`             | `object`              | Sales order ID                                   |
| `Order_Date`           | `datetime64[ns]`      | Date when the order was placed                   |
| `Ship_Mode`            | `object`              | Shipping mode used                               |
| `Customer_ID`          | `object`              | Unique customer identifier                       |
| `Country_Region`       | `object`              | Country or region of the customer                |
| `City`                 | `object`              | Customer's city                                  |
| `State_Province`       | `object`              | Customer's state or province                     |
| `Postal_Code`          | `object`              | Postal code                                      |
| `Division`             | `object`              | Division (likely product or location category)   |
| `Region`               | `object`              | Sales region                                     |
| `Product_ID`           | `object`              | Unique product identifier                        |
| `Product_Name`         | `object`              | Name of the product                              |
| `Sales`                | `float64`             | Sales amount                                     |
| `Units`                | `float64`             | Number of units sold                             |
| `Gross_Profit`         | `float64`             | Gross profit generated                           |
| `Cost`                 | `float64`             | Cost of the sale                                 |
| `Factory`              | `object`              | Factory that produced the product                |
| `Unit_Price`           | `float64`             | Price per unit                                   |
| `Unit_Cost`            | `float64`             | Cost per unit                                    |
| `Latitude`             | `float64`             | Latitude of the location                         |
| `Longitude`            | `float64`             | Longitude of the location                        |
| `Correct_shipdate`     | `datetime64[ns]`      | Cleaned/verified shipping date                   |
| `Orders_delay`         | `object`              | Delay status of the order                        |
| `Shipping_years`       | `int64`               | Year in which the order was shipped              |

---

## ✅ Outcomes

- Built an automated ETL pipeline
- Leveraged BigQuery for fast and scalable EDA
- Delivered a live dashboard providing business-critical insights

## 📎 Resources

- Dataset: [Kaggle Link (if public)](your-link-here)
- BI Dashboard: [View Live (if public)](your-link-here)
