# Brazilian E-Commerce Marketplace Sales Analysis

## 📊 Data Analytics Mini Project

This project focuses on **Brazilian E-Commerce Marketplace Sales Analysis** using **Excel and Power BI**.

The main objective of the project is to perform **data cleaning, transformation, analysis, and visualization** on Brazilian e-commerce data.

---

## 🛠️ Tools Used

* Microsoft Excel
* Power Query
* Power BI
* DAX
* Pivot Tables
* Pivot Charts
* VLOOKUP

---

## 🎯 Project Objective

* Data Cleaning
* Data Transformation
* Data Analysis
* Data Visualization
* Data Modeling
* Interactive Dashboard Development

---

# 📁 Project Workflow

The project was completed in three major stages:

1. **ETL Using Excel**
2. **Data Pre-Processing Using Excel**
3. **Data Visualization and Reporting Using Power BI**

---

# 1. 🔄 ETL Using Excel

The Brazilian e-commerce CSV datasets were imported into Excel using **Data → From Text/CSV** and transformed using **Power Query Editor**.

### Datasets Imported

The project worked with the following Olist datasets:

* Olist Customers
* Olist Geolocation
* Olist Order Items
* Olist Order Payments
* Olist Order Reviews
* Olist Orders
* Olist Products
* Olist Sellers
* Olist Product Category Translation

## The datasets were transformed and loaded into Excel tables.

# 2. 🧹 Data Pre-Processing Using Excel

## Data Standardization

The following data formats were standardized:

* Customer columns → Text format
* ZIP code → Number format
* Latitude and longitude → Number format
* Price and freight values → Accounting format
* Shipping limit date → Date format

## Duplicate Removal

Duplicate records were checked and removed from:

* Product Category Translation
* Order Payments
* Order Details
* Geolocation datasets

## Irrelevant Data Removal

Irrelevant columns were removed from the datasets, including:

* `payment_sequential`
* `order_item_id`
* `customer_unique_id`
* Review comment columns
* Product dimension and description columns

## Missing Value Handling

Missing and inconsistent values were handled using Excel tools such as **Find and Replace**.

Examples included:

* Standardizing `boleto` to bank slip
* Handling unknown product category values
* Handling blank/missing order dates without changing existing dates

---

# 3. 🔗 Combining Data Using VLOOKUP

VLOOKUP was used to combine information from different worksheets.

The project retrieved:

* `customer_id`
* `payment_type`
* `customer_zip_code_prefix`
* `sales_city`
* `sales_state`
* `product_category_name`
* `order_status`
* `product_load`

using related IDs such as `order_id`, `customer_id`, and `product_id`.

---

# 4. 🧮 Calculated Fields in Excel

Several calculated fields were created:

### Final Price

`final_price` was calculated by adding:

**Price + Shipping Cost**

### Delivery Time

`time_delivery` was calculated using the **DATEDIF** function.

### Product Weight

Product weight was converted from **grams to kilograms**.

### Product Load

A `product_load` category was created based on product weight using a **Nested IF formula**.

---

# 5. 📊 Excel Data Analysis

Pivot Tables and Pivot Charts were created for sales analysis.

### Visualizations Created

* Column Chart → Total Revenue by Product Category
* Area Chart → Total Revenue by State
* Bar Chart → Order Payment Type Distribution
* Pie Chart → Revenue by Payment Method
* Area Chart → Delivery Cost by State and Product Load

---

# 6. 📈 Power BI Data Visualization

The cleaned Excel dataset was imported into Power BI.

Power Query was used to:

* Select required tables
* Transform data
* Verify data types
* Prepare data for visualization

---

# 7. 🔗 Power BI Data Modeling

Relationships were created between the different tables.

### One-to-Many Relationships

* `customers_location` → `sales_details`
* `sellers_location` → `sales_details`
* `products_details` → `sales_details`
* `orders_delivery` → `order_payments`
* `orders_delivery` → `order_reviews`
* `customers_location` → `orders_delivery`

### Many-to-Many Relationship

* `geography` ↔ `sales_details` using `zip_code`

The overall Power BI model contains the connected tables required for sales analysis.

---

# 8. 📊 Power BI Report & Visualizations

The Power BI report was designed to analyze Brazilian e-commerce sales.

## KPI Cards

The following DAX-based cards were created:

* **Total Sales**
* **Total Orders**
* **Total Customers**
* **Average Order Value**

## Charts

The report includes:

* Sales by Product Category
* Sales by Month
* Sales by Payment Type
* Sales by Location
* Yearly Sales Trend
* Sales by Payment Type using Donut Chart
* Sales by Payment Type using Bar Chart
* Sales by Geographical Location using Map

---

# 9. 🎛️ Interactive Slicers & Filters

Interactive slicers were created for:

* **State**
* **Payment Type**
* **Product Category**
* **Order Status**

These slicers allow users to interactively filter and analyze the sales data.

---

# 10. 📌 Interactive Dashboards

Two interactive Power BI dashboards were developed:

### 🛒 Brazilian E-Commerce Sales Dashboard

Provides an interactive view of sales performance using KPI cards, charts, geographical analysis, and slicers.

### 📦 Brazilian E-Commerce Order Dashboard

Provides an interactive view of order-related information and order analysis.

---

# 🔍 Key Skills Demonstrated

* Excel Data Cleaning
* Excel Data Transformation
* Power Query
* VLOOKUP
* DATEDIF
* Nested IF
* Pivot Tables
* Pivot Charts
* Power BI
* DAX Measures
* Data Modeling
* One-to-Many Relationships
* Many-to-Many Relationships
* Data Visualization
* Interactive Dashboards
* Slicers and Filters

---

# 📂 Project Structure

```text
Brazilian-E-Commerce-Marketplace-Sales-Analysis/
│
├── README.md
├── Brazilian E-Commerce Marketplace Sales Analysis.xlsx
├── Brazilian E-Commerce Marketplace Sales Analysis.pbix
│
└── screenshots/
    ├── excel-analysis.png
    ├── power-bi-data-model.png
    ├── sales-dashboard.png
    └── order-dashboard.png
```

> Add the Excel, Power BI, and screenshot files to the repository if they are available.

---

# 🎓 Project Outcome

This mini project demonstrates an end-to-end **data analytics workflow**, starting from raw Brazilian e-commerce datasets, followed by data cleaning and transformation in Excel, data modeling in Power BI, and finally interactive visualization and dashboard development.

The project was completed using **Excel and Power BI**, with the objective of applying practical data analytics techniques to e-commerce data.

---

## 👤 Project Information

**Project:** Brazilian E-Commerce Marketplace Sales Analysis
**Type:** Data Analytics Mini Project
**Tools:** Excel & Power BI
**Focus:** Data Cleaning, Transformation, Analysis & Visualization
**Submission Date:** 12/08/2026
