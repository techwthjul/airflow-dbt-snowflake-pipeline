# 🧬 Modular ELT Pipeline with Airflow, DBT, and Snowflake

This project demonstrates an end-to-end modular ELT (Extract-Load-Transform) pipeline using **Apache Airflow**, **dbt (Data Build Tool)**, and **Snowflake**. It automates data ingestion, transformation, and testing workflows for TPCH datasets using `cosmos` and Airflow DAGs.

## 🚀 Project Highlights

- Built a fully modular ELT pipeline orchestrated with Airflow DAGs and Cosmos
- Integrated dbt models for staging, transformation, and testing in Snowflake
- Debugged access & role issues, ensuring seamless end-to-end CI/CD execution
- Used XCom and logs to trace and resolve DAG failures and data lineage issues

## 🧱 Architecture

```text
Airflow (DAG) 
   │
   ├──> dbt run (stg_tpch_orders, stg_tpch_line_items)
   │
   ├──> dbt run (intermediate models)
   │
   └──> dbt test + dbt run (fact tables)
        ↓
     Snowflake Warehouse
