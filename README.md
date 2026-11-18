# 🛒 Olist E-Commerce Analytics & Logistics Dashboard

An end-to-end data analytics and ETL pipeline project analyzing e-commerce sales performance, payment behavior, customer satisfaction, and logistics delivery trends using the public Olist dataset.

---

## 📌 Project Overview
This project simulates a complete modern Data Stack workflow—from raw data ingestion and cloud warehousing to data transformation and business intelligence visualization. The primary goal is to uncover insights into delivery delays, payment method preferences, and customer satisfaction metrics.

---

## ⚙️ Modern Data Stack & ETL Pipeline Architecture
The project follows a robust, modern ETL workflow:

1. **Data Source (Extract):** 
   - Downloaded raw transactional, customer, and logistics datasets from **Kaggle** (Olist E-Commerce Public Dataset).
2. **Data Staging & Cleaning (Transform):** 
   - Performed initial exploratory data analysis and basic data cleaning in **Google Sheets** to handle missing values and format dates correctly.
3. **Data Pipeline & Ingestion (Load):** 
   - Utilized **Fivetran** to automate data pipelines, moving and syncing the cleaned datasets seamlessly into cloud storage.
4. **Cloud Data Warehouse:** 
   - Stored and structured the centralized relational data tables inside **Snowflake**.
5. **Data Visualization & BI:** 
   - Connected **Power BI** directly to Snowflake to build an interactive executive dashboard.

---

## 📊 Dashboard Components & Key Insights
The final single-page Power BI dashboard features:
* **Executive KPI Cards:** Tracking Total Revenue (`R$15.84M`), Total Orders (`99K`), Average Customer Satisfaction Score (`4.09`), and Active Customers (`96K`).
* **Interactive Slicers:** Dynamic filtering capabilities by `PAYMENT_TYPE` and `ORDER_STATUS`.
* **Monthly Order Volume Trend:** A clean line chart tracking order frequency and seasonal trends month-over-month.
* **Revenue Distribution by Payment Method:** A donut chart highlighting customer payment preferences (Credit Card dominating at ~78%).
* **Delivery Performance vs. Customer Satisfaction:** A comparative analysis showing how on-time deliveries maintain a high rating (~4.2) while delayed deliveries cause satisfaction scores to drop sharply (~2.3).

---

## 🗂️ Folder Structure
```text
📦 Olist-Ecommerce-Analytics-Project
│
├── 📁 Data/
│   ├── 📄 Raw_Data_Kaggle.csv
│   └── 📄 Cleaned_Data_GoogleSheets.csv
│
├── 📁 PowerBI/
│   └── 📊 Olist_Performance_Dashboard.pbix
│
└── 📄 README.md
