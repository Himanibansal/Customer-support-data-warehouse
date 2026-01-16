# 📊 Customer Support Data Warehouse

A SQL-based data warehouse project built using a **Star Schema data model** and a **Bronze → Silver → Gold** layered architecture to transform raw customer support data into analytics-ready datasets for reporting, KPI tracking, and business insights.

---

## 🚀 Project Overview

Customer support systems generate large volumes of operational data such as tickets, priorities, agents, customers, statuses, and resolution timelines.
This project creates a scalable data warehouse that:

* Ingests raw data from source systems
* Cleans, validates, and standardizes datasets
* Models data using Fact and Dimension tables (Star Schema)
* Enables fast analytical queries and BI reporting

The warehouse follows modern data engineering best practices for performance, reliability, and scalability.

---

## 🏗️ Architecture

```
Source Systems
      ↓
Bronze Layer  → Raw ingestion
      ↓
Silver Layer  → Cleaned and standardized data
      ↓
Gold Layer    → Star Schema (Fact & Dimension tables)
```

---

## ⭐ Star Schema Design

The Gold layer is modeled using a **Star Schema** to optimize query performance and reporting.

### Fact Table

* fact_issues (or fact_tickets)

  * Ticket count
  * Resolution time
  * SLA metrics
  * Reopen count
  * Status duration

### Dimension Tables

* dim_customer
* dim_agent
* dim_issue_type
* dim_priority
* dim_status
* dim_date
* dim_project

Each dimension connects directly to the fact table using surrogate keys.

---

## 🧩 Data Layers

### 🥉 Bronze Layer

* Raw ingestion from source systems
* No transformations applied
* Maintains original data for audit and traceability

### 🥈 Silver Layer

* Data cleaning and validation
* Standardization of formats and data types
* Deduplication and business rule enforcement

### 🥇 Gold Layer

* Star schema implementation
* Fact and dimension tables
* Aggregated KPIs and metrics
* Optimized for analytics and dashboards

---

## 🛠️ Tech Stack

* SQL Server / T-SQL
* Stored Procedures for ETL
* Star Schema Data Modeling
* Git & GitHub
* Data Quality Validation

---

## 📁 Project Structure

```
Customer-support-data-warehouse/
│
├── bronze/
├── silver/
├── gold/
│   ├── fact_tables/
│   └── dimension_tables/
├── scripts/
└── README.md
```

---

## 📈 Key Features

* Star schema optimized for analytics
* Layered data warehouse architecture
* Automated SQL ETL pipelines
* Data quality checks and validation
* Scalable dimensional modeling
* Business-ready reporting datasets

---

## 🎯 Use Cases

* Customer support performance tracking
* SLA compliance monitoring
* Ticket lifecycle analysis
* Agent productivity analysis
* Operational dashboards

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/Customer-support-data-warehouse.git
```

2. Execute Bronze ingestion scripts.

3. Run Silver transformation procedures.

4. Populate Gold fact and dimension tables.

5. Validate results using sample queries.

---

## 👩‍💻 Author

Himani Bansal
Analytics Consultant | SQL | Data Analytics | Data Engineering
