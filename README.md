# SQL Sales & Customer Analytics

![SQL](https://img.shields.io/badge/SQL-Analysis-blue?style=for-the-badge)
![Data Analytics](https://img.shields.io/badge/Data-Analytics-0f766e?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> An end-to-end SQL analytics project focused on exploring sales, customer, product, and order data to uncover meaningful business insights using advanced SQL techniques.

---

## Contents

- [1. What is this project for?](#1-what-is-this-project-for)
- [2. Why did I choose this project?](#2-why-did-i-choose-this-project)
- [3. What did I learn?](#3-what-did-i-learn)
- [4. Project Structure & Architecture](#4-project-structure--architecture)
- [5. Tech Stack](#5-tech-stack)
- [6. Visuals](#6-visuals)
- [7. How to Explore the Project](#7-how-to-explore-the-project)

---

## 1. What is this project for?

This project is designed to demonstrate how **SQL can be used as a business analytics tool**, not just as a way to retrieve data.

The analysis works across core business entities such as:

- **Customers** — customer details and segmentation
- **Orders** — transaction and order-date information
- **Products** — product, category, and pricing information
- **Sales** — quantities, revenue, and product-level sales activity

The main objective is to move from **raw transactional data → analysis → insights → business understanding**.

### Key analytical questions

| Area | Questions explored |
|---|---|
| Sales | What are the overall sales and revenue trends? |
| Customers | Which customers are the most valuable? |
| Products | Which products and categories perform best? |
| Orders | How frequently do customers purchase? |
| Trends | How do sales change over time? |
| Segments | How does performance differ across customer groups? |

---

## 2. Why did I choose this project?

I chose this project because I wanted to build a SQL project that reflects the type of analysis a **Data Analyst performs in a real business environment**.

Rather than focusing only on SQL syntax, I wanted to practice answering questions such as:

> **What happened? Why did it happen? Which customers or products matter most? What can the business learn from the data?**

This project also gave me the opportunity to work with several SQL concepts together instead of learning them in isolation. That includes joins, aggregations, CTEs, subqueries, conditional logic, and window functions.

The project is therefore a practical exercise in connecting **technical SQL skills with business-oriented thinking**.

---

## 3. What did I learn?

### SQL skills

- Writing analytical queries using `SELECT`, `WHERE`, `GROUP BY`, `HAVING`, and `ORDER BY`
- Combining multiple relational tables using `INNER JOIN` and `LEFT JOIN`
- Performing calculations with aggregate functions such as `SUM`, `AVG`, `COUNT`, `MIN`, and `MAX`
- Building reusable query logic with **CTEs (Common Table Expressions)**
- Using **subqueries** for nested analysis
- Creating business rules with `CASE WHEN`
- Applying **window functions** such as:
  - `ROW_NUMBER()`
  - `RANK()`
  - `DENSE_RANK()`
  - `LAG()`
  - `LEAD()`

### Analytical skills

- Translating a business question into a SQL query
- Comparing customer and product performance
- Identifying trends and outliers
- Segmenting customers based on behavior or value
- Interpreting query results instead of stopping at the output
- Turning quantitative findings into business insights

### Key takeaway

> **The biggest lesson from this project was that good SQL analysis is not only about writing complex queries; it is about using those queries to answer the right business questions.**

---

## 4. Project Structure & Architecture

### Project flow

```text
                 RAW DATA
                    │
                    ▼
       ┌─────────────────────────┐
       │ Customers / Orders      │
       │ Products / Sales        │
       └────────────┬────────────┘
                    │
                    ▼
             SQL Data Layer
                    │
        ┌───────────┼───────────┐
        ▼           ▼           ▼
      JOINs     Aggregations  CTEs
        │           │           │
        └───────────┼───────────┘
                    ▼
          Window Functions
                    │
                    ▼
            Business Analysis
                    │
          ┌─────────┼─────────┐
          ▼         ▼         ▼
       Sales     Customer   Product
       Trends    Insights   Performance
          │         │         │
          └─────────┼─────────┘
                    ▼
             Final Insights
```

### Logical data model

```text
Customers
    │
    │ customer_id
    ▼
Orders
    │
    │ order_id
    ▼
Sales
    │
    │ product_id
    ▼
Products
```

The relationships allow the analysis to connect **who purchased**, **what they purchased**, **when they purchased it**, and **how much was generated**.

### Recommended repository structure

```text
Sales-Customer-Analytics/
│
├── datasets/
│   └── raw and reference datasets
│
├── sql/
│   ├── 01_data_exploration.sql
│   ├── 02_sales_analysis.sql
│   ├── 03_customer_analysis.sql
│   ├── 04_product_analysis.sql
│   └── 05_advanced_analysis.sql
│
├── visuals/
│   └── screenshots and analysis visuals
│
├── README.md
└── LICENSE
```

> Update the folder/file names above to match the exact files you keep in the repository.

---

## 5. Tech Stack

| Technology | Purpose |
|---|---|
| **SQL** | Data exploration, transformation, aggregation, and analysis |
| **Relational Database** | Storage and querying of customers, orders, products, and sales data |
| **Git** | Version control |
| **GitHub** | Project hosting and portfolio presentation |
| **VS Code** | SQL development and project management |

### SQL concepts used

`JOINs` · `GROUP BY` · `HAVING` · `CASE WHEN` · `CTEs` · `Subqueries` · `Aggregate Functions` · `Window Functions` · `Ranking` · `Time-based Analysis`

---

## 6. Visuals

### Project Preview

Add your best SQL result screenshots, database/schema diagram, or dashboard visuals here.

```text
📷 Visual 1 — Database / Schema
📷 Visual 2 — Sales Analysis Output
📷 Visual 3 — Customer Analysis Output
📷 Visual 4 — Product Performance Output
```

Example Markdown format:

```md
![Database Schema](visuals/database-schema.png)

![Sales Analysis](visuals/sales-analysis.png)

![Customer Analysis](visuals/customer-analysis.png)
```

### Suggested visuals to include

1. **Database schema** — shows relationships among Customers, Orders, Sales, and Products.
2. **Sales trend** — monthly/periodic revenue trend.
3. **Customer analysis** — high-value or repeat-customer analysis.
4. **Product performance** — top products/categories by sales or revenue.
5. **Optional Power BI dashboard** — if you later extend the project into visualization.

---

## 7. How to Explore the Project

### 1. Clone the repository

```bash
git clone https://github.com/AmanJha-1337/Sales-Customer-Analytics.git
cd Sales-Customer-Analytics
```

### 2. Load the dataset

Import the project dataset into your SQL environment and confirm the table relationships.

### 3. Run the analysis

Start with the basic exploration queries, then move through sales, customer, product, and advanced analysis.

### 4. Interpret the results

For every query, focus on three questions:

- **What does the query calculate?**
- **Why is the metric useful?**
- **What business conclusion can be drawn from the result?**

---

## Project Objective

The goal of this project is to demonstrate that I can go beyond writing SQL syntax and use SQL to perform **structured, business-focused data analysis**.

> **Explore → Analyze → Interpret → Communicate**

---

## Author

**Aman Jha**  
Data Analytics | SQL | Python | Excel | Power BI

[GitHub](https://github.com/AmanJha-1337)
