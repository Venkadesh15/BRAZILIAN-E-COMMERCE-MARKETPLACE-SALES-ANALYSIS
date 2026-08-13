## Brazilian E-Commerce Marketplace Sales Analysis

## 📊 Data Analytics Mini Project

This project focuses on **Brazilian E-Commerce Marketplace Sales Analysis** using **Microsoft Excel and Power BI**.

The main objective is to perform an end-to-end data analytics workflow, including **data cleaning, transformation, analysis, data modeling, and interactive visualization** using Brazilian e-commerce marketplace data.

---

## 🛠️ Tools & Technologies Used

* Microsoft Excel
* Power Query
* Power BI
* DAX
* Pivot Tables
* Pivot Charts
* VLOOKUP
* DATEDIF
* Nested IF
* Data Modeling
* Data Visualization

---

## 🎯 Project Objectives

* Data Cleaning
* Data Transformation
* Data Pre-Processing
* Data Analysis
* Data Modeling
* Data Visualization
* Interactive Dashboard Development
* Deriving business insights from e-commerce data

---

## 🔄 Project Workflow

The project was completed in three major stages:

1. **ETL Using Excel**
2. **Data Pre-Processing & Analysis Using Excel**
3. **Data Visualization & Reporting Using Power BI**

---

# 1. 🔄 ETL Using Excel

The Brazilian e-commerce CSV datasets were imported into Excel using:

**Data → From Text/CSV**

Power Query Editor was then used to transform and prepare the datasets before loading them into Excel tables.

### 📁 Datasets Used

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

---

# 2. 🧹 Data Pre-Processing Using Excel

## Data Standardization

Data types and formats were standardized across the datasets.

Examples include:

* Customer-related columns → Text format
* ZIP code → Number format
* Latitude & Longitude → Number format
* Price & Freight values → Accounting format
* Shipping limit date → Date format

## Duplicate Removal

Duplicate records were checked and removed where applicable from:

* Product Category Translation
* Order Payments
* Order Details
* Geolocation datasets

## Irrelevant Data Removal

Columns that were not required for analysis were removed, including:

* `payment_sequential`
* `order_item_id`
* `customer_unique_id`
* Review comment columns
* Product dimension and description columns

## Missing & Inconsistent Value Handling

Missing and inconsistent values were handled using Excel tools such as **Find & Replace** and data-cleaning techniques.

Examples:

* Standardizing `boleto` as **Bank Slip**
* Handling unknown product category values
* Handling blank or missing order dates without modifying valid existing dates

---

# 3. 🔗 Combining Data Using VLOOKUP

**VLOOKUP** was used to retrieve and combine related information across worksheets.

The following information was retrieved where required:

* `customer_id`
* `payment_type`
* `customer_zip_code_prefix`
* `sales_city`
* `sales_state`
* `product_category_name`
* `order_status`
* `product_load`

Related IDs such as:

* `order_id`
* `customer_id`
* `product_id`

were used to connect information between datasets.

---

# 4. 🧮 Calculated Fields in Excel

Several calculated fields were created to support analysis.

### Final Price

The final price was calculated as:

**Final Price = Price + Shipping Cost**

### Delivery Time

Delivery time was calculated using the **DATEDIF** function based on relevant order and delivery dates.

### Product Weight

Product weight was converted from **grams to kilograms**.

### Product Load

A `product_load` category was created based on product weight using a **Nested IF** formula.

This helped categorize products based on their weight for further analysis.

---

# 5. 📊 Excel Data Analysis

Pivot Tables and Pivot Charts were created to analyze sales, payments, delivery costs, and geographical performance.

## 📈 Visualizations Created

* **Column Chart** → Total Revenue by Product Category
* **Area Chart** → Total Revenue by State
* **Bar Chart** → Order Payment Type Distribution
* **Pie Chart** → Revenue by Payment Method
* **Area Chart** → Delivery Cost by State and Product Load

These visualizations helped identify patterns and trends in Brazilian e-commerce sales.

---

# 6. 📈 Power BI Data Visualization

The cleaned and prepared Excel data was imported into **Power BI**.

Power Query was used to:

* Select required tables
* Transform data
* Verify data types
* Prepare data for visualization
* Ensure consistency between datasets

---

# 7. 🔗 Power BI Data Modeling

A relational data model was created in Power BI to connect the different datasets.

## One-to-Many Relationships

The following relationships were created:

* `customers_location` → `sales_details`
* `sellers_location` → `sales_details`
* `products_details` → `sales_details`
* `orders_delivery` → `order_payments`
* `orders_delivery` → `order_reviews`
* `customers_location` → `orders_delivery`

These relationships allow information from dimension tables to filter and analyze related sales and order data.

## Many-to-Many Relationship

A many-to-many relationship was created between:

* `geography`
* `sales_details`

using the `zip_code` field.

The overall Power BI data model connects customer, seller, product, order, payment, review, and geographical information for comprehensive e-commerce analysis.

---

# 8. 📊 Power BI Report & Visualizations

The Power BI report was designed to provide an interactive overview of Brazilian e-commerce sales and order performance.

## 📌 KPI Cards

The following DAX-based KPIs were created:

* **Total Sales**
* **Total Orders**
* **Total Customers**
* **Average Order Value**

## 📈 Charts & Visualizations

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

Interactive slicers were added to make the Power BI report dynamic.

### Slicers Used

* State
* Payment Type
* Product Category
* Order Status

Users can select different values to dynamically filter the charts and KPI cards.

---

# 10. 📌 Interactive Dashboards

Two interactive Power BI dashboards were developed.

## 🛒 Brazilian E-Commerce Sales Dashboard

Provides an interactive overview of:

* Sales performance
* Revenue
* Orders
* Customers
* Product categories
* Payment methods
* Monthly and yearly trends
* Geographical sales performance

## 📦 Brazilian E-Commerce Order Dashboard

Provides an interactive view of:

* Order performance
* Order status
* Delivery information
* Payment methods
* Customer and order analysis
* Order-related KPIs

---

# 🔍 Key Skills Demonstrated

### Excel

* Data Cleaning
* Data Transformation
* VLOOKUP
* DATEDIF
* Nested IF
* Pivot Tables
* Pivot Charts
* Data Formatting
* Data Analysis

### Power BI

* Power Query
* DAX Measures
* Data Modeling
* One-to-Many Relationships
* Many-to-Many Relationships
* KPI Cards
* Charts
* Maps
* Slicers
* Filters
* Interactive Dashboards

### Data Analytics

* ETL
* Data Pre-Processing
* Exploratory Data Analysis
* Data Visualization
* Business-oriented Reporting

---

# 📂 Project Structure

```text
Brazilian-E-Commerce-Marketplace-Sales-Analysis/
│
├── README.md
│
├── Brazilian E-Commerce Marketplace Sales Analysis.xlsx
├── Brazilian E-Commerce Marketplace Sales Analysis.pbix
│
└── screenshots/
    ├── excel-analysis.png
    ├── power-bi-data-model.png
    ├── sales-dashboard.png
    └── order-dashboard.png
```

> **Note:** The Excel and Power BI files are large files. If they exceed GitHub's standard file-size limit, they should be stored using **Git LFS** or an external cloud-storage link rather than committing them directly to a normal Git repository.

---

# 🎓 Project Outcome

This mini project demonstrates an **end-to-end data analytics workflow**, starting from raw Brazilian e-commerce datasets and progressing through:

**Raw Data → ETL → Data Cleaning → Data Transformation → Data Analysis → Data Modeling → Visualization → Interactive Dashboard**

The project provided practical experience in using **Excel and Power BI** to transform raw e-commerce data into meaningful analytical reports and interactive dashboards.

---

# 👤 Project Information

| Details             | Information                                             |
| ------------------- | ------------------------------------------------------- |
| **Project**         | Brazilian E-Commerce Marketplace Sales Analysis         |
| **Project Type**    | Data Analytics Mini Project                             |
| **Domain**          | E-Commerce                                              |
| **Tools**           | Microsoft Excel & Power BI                              |
| **Focus**           | Data Cleaning, Transformation, Analysis & Visualization |
| **Data Source**     | Olist Brazilian E-Commerce Dataset                      |
| **Submission Date** | 12/08/2026                                              |

---

## ⭐ Project Highlights

* Worked with multiple Brazilian e-commerce datasets
* Performed data cleaning and transformation using Excel and Power Query
* Used VLOOKUP to combine related information
* Created calculated fields using Excel formulas
* Built Pivot Tables and Pivot Charts
* Developed a relational data model in Power BI
* Created DAX-based KPI measures
* Developed interactive dashboards
* Used slicers, filters, charts, maps, and KPI cards
* Applied practical data analytics techniques to a real-world e-commerce dataset
