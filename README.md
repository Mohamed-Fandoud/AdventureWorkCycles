# 🚲 AdventureWorks Bikes Dashboard Project Summary

---

## 💡 Project Overview
This Power BI dashboard analyzes sales, customer behavior, product trends, and inventory movement using the **AdventureWorksDW2022** dataset. It spans data from **December 2020 to January 2025** and focuses on the performance of bike products across different territories, customers, and time periods. The dashboard is powered by data sourced from **Microsoft SQL Server**, queried using T-SQL, and modeled using a **star schema** in Power BI.

---

## 🧩 Data Model Overview
<img width="980" height="692" alt="Image" src="https://github.com/user-attachments/assets/dcbff994-072b-4bab-80fa-2e5616581a4c" />
The data model follows a **star schema** design to ensure efficient querying and report performance.

### 🔹 Fact Tables
- `FactInternetSales`: Contains all sales transaction data, including order quantities, amounts, dates, and customer/product keys.
- `FactProductInventory`: Tracks product inventory movements, balances, and cost over time.
- `FactTarget`: Imported from Excel; contains monthly sales targets.

### 🔹 Dimension Tables
- `DimDate`: Calendar table connected to all time-based analysis.
- `DimCustomer`: Provides enriched customer data including demographics, income, education, and segmentation.
- `DimGeography`: Linked to customers, offering detailed city and country-level data.
- `DimSalesTerritory`: Defines broader sales regions and groupings.
- `DimProduct`: Merged with category and subcategory tables to offer full product hierarchy.

Relationships are primarily one-to-many from dimensions to fact tables, with special handling for targets (linked by month and year).

---

## 📊 Dashboard Pages Description

### 🏠 Landing Page
<img width="1301" height="727" alt="Image" src="https://github.com/user-attachments/assets/6e767196-ec82-4ec6-8575-3ca19b442d67" />
Introduces the dashboard and dataset, outlines the time range and content, and provides navigation buttons to key report sections.

### 📈 Overview Page
<img width="1298" height="718" alt="Image" src="https://github.com/user-attachments/assets/36274d4c-c3b3-4226-a2d7-b7bf3fc140cf" />
Presents KPIs such as total revenue, profit, orders, and customers. Includes trend visuals, product category breakdowns, and top-performing countries.

### 🌍 Map Analysis
<img width="1306" height="731" alt="Image" src="https://github.com/user-attachments/assets/04941443-24c7-4baa-a90e-96ad9bc37535" />
Interactive map visuals showing geographic distribution of sales by country and city. Allows for comparison and exploration of regional trends.

### 👥 Customer Analysis
<img width="1302" height="727" alt="Image" src="https://github.com/user-attachments/assets/e947976a-33d5-4d5d-8c8f-b52517f5be17" />
Displays customer segmentation (VIP, Frequent, Potential, etc.), income brackets, and behavioral insights. Highlights top customers and their contributions.

### 🚴‍♂️ Product Analysis
<img width="1300" height="725" alt="Image" src="https://github.com/user-attachments/assets/e5be1e0d-1707-4152-888b-4959b1fdd362" />
Analyzes product-level sales and profitability. Includes best-seller lists, product category comparisons, and trends over time.

### 📦 Inventory Analysis
<img width="1302" height="732" alt="Image" src="https://github.com/user-attachments/assets/9a02467a-e384-47e4-890a-f7e72c6a69ee" />
Tracks inventory balances, last movement dates, and product-level stock levels. Includes a time series of total stock value.

### 🔄 Year-over-Year Comparison
<img width="1302" height="733" alt="Image" src="https://github.com/user-attachments/assets/4db70f39-5043-4e23-b2d5-9a80610d9594" />
Compares sales, orders, and customers between selected years. Includes YoY growth %, breakdown by product and region, and top/bottom growth contributors.

### ❓ Q&A Page
<img width="1301" height="717" alt="Image" src="https://github.com/user-attachments/assets/b16f1470-d4f9-4d24-92ae-e1aaffd74505" />
Allows users to ask natural language questions to explore data freely. Powered by Power BI's Q&A visual.

---

## 🛠 Tools & Technologies
- **Microsoft SQL Server**: Data extraction using T-SQL.
- **Power BI Desktop**: Data modeling, DAX measures, visual design, and interactivity.
- **Excel**: Monthly targets imported and related via calendar dimensions.

---
