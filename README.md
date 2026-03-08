# Sakila Dimensional Modeling

This project implements a robust dimensional model for the Sakila DVD rental database, transforming it from a normalized transactional structure into an optimized Star Schema designed for analytical processing and business intelligence.

## 📌 Project Overview
The Sakila database is a well-known sample schema representing a complex DVD rental business. This project focuses on the de-normalization and structuring of this data into Facts and Dimensions, enabling efficient querying for key business metrics such as revenue trends, inventory management, and customer behavior analysis.

## 🏗 Core Architecture
The system utilizes a **Star Schema** to minimize join complexity and maximize query performance for OLAP (Online Analytical Processing) workloads.

### 1. Fact Tables
* **Rental Fact:** Captures the core business process of DVD rentals, including rental duration, return status, and associated revenue.
* **Payment Fact:** Records transactional financial data linked to specific rentals and customers.

### 2. Dimension Tables
* **Dim_Customer:** Master data for subscriber profiles, including geographical and status information.
* **Dim_Film:** Comprehensive film attributes such as category, language, and rental rates.
* **Dim_Store:** Details about store locations and staff management.
* **Dim_Date:** A specialized time dimension to support temporal analysis across years, quarters, and months.

## 🛠 Technical Deliverables
* **ER Diagrams:** Comprehensive visual maps of the dimensional relationships (available in `ER_Diagram_Sakila_Data.pdf` and `.DM1` formats).
* **Dimensional Model Report:** A technical deep dive into the business requirements, grain identification, and attribute selection for each table (`Sakila_Dimensional_Modeling_Report.pdf`).

## 🚀 Key Features
* **OLTP to OLAP Transition:** Successfully transitions data from a 3rd Normal Form (3NF) transactional database to a high-performance Star Schema.
* **Analytical Readiness:** The schema is specifically structured to support sub-second aggregations and complex filtering in Business Intelligence tools.
* **Schema Integrity:** Enforces referential integrity through strictly defined primary and foreign keys across the dimension-to-fact relationships.

---
*Developed by [Chinmay Kulkarni](https://github.com/ckulkarni13)*
