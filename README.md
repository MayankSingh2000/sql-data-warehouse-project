# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 
This project demonstrates a comprhensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed at a portfolio project which highlights industry best practices in data engineering and analytics.

---
## Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:
![image alt](https://github.com/MayankSingh2000/sql-data-warehouse-project/blob/main/docs/data_architecture.png?raw=true)

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.
---

## Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.
---

## Data & Tools Used:
- **Datasets:** Access to the project datasets (CSV files).
- **SQL Server Express** 
- **SQL Server Management Studio (SSMS)** 
- **Git Repository** 
- **DrawIO**
- **Notion**
---

## Project Requirements

### Building the Data Warehouse (Data Engineering)

### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical and informed decision-making.

### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) Provided as csv files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

---

## Data Flow Diagram 
![image alt](https://github.com/MayankSingh2000/sql-data-warehouse-project/blob/main/docs/data_flow_diagram.png?raw=true)

This diagram illustrates a multi-stage data flow pipeline, moving data from Source Systems through a **Bronze, Silver, and Gold Layer architecture**.

The Source Systems (**CRM and ERP**) feed raw data into the Bronze Layer.

The **Bronze Layer** holds the initial, raw, and unvalidated data.

The **Silver Layer** stores clean, transformed, and integrated data, which is ready for consumption.

The final **Gold Layer** contains highly refined, summarized, and optimized data for business intelligence and reporting, structured into fact and dimension tables (i.e., fact_sales, dim_customers, and dim_products).

The flow shows data refinement and transformation at each stage, leading to a dimensional model in the Gold Layer for analytics.
---

## Data Modelling (Star Schema)
![image alt](https://github.com/MayankSingh2000/sql-data-warehouse-project/blob/main/docs/data_modelling.png?raw=true)

This diagram illustrates a Sales Data Mart based on a **Star Schema dimensional model**.

The central table is **gold.fact_sales**, which holds the core measures (like sales_amount, quantity, price etc.) and foreign keys (FK) to the dimension tables, including product_key and customer_key.

**It is connected to two key Dimension Tables:**

- **gold.dim_customers:** Contains detailed attributes about customers (e.g., first_name, country, marital_status etc).

- **gold.dim_products:** Contains detailed attributes about the products sold (e.g., product_name, category, subcategoryetc).

This model is optimized for efficient business intelligence queries and analytical reporting related to sales performance.
---

## BI: Analytics & Reporting (Data Analytics)

### Objective
Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

This insights empower stakeholders with key business metrics, enabling strategic decision-making.

---

## License

This project is licensed under the MIT License.

---

## 📚 Dataset Credits

- Dataset Name: **Data Warehouse and Analytics** 
- Provided By: **Baraa Khatib Salkini(DataWithBaraa)**  
- Purpose: **Educational & Practice Use**  
- Used For: **Data Warehouse and Analytics Project**

All credit for the original dataset goes to the respective provider.

---

## 🙏 Acknowledgements

Special thanks to [@DataWithBaraa](https://github.com/DataWithBaraa) for providing learning resources and datasets.


