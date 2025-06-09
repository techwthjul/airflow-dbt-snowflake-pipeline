# Airflow + DBT + Snowflake Modular ELT Pipeline 🚀

This project implements a **modular ELT (Extract, Load, Transform) pipeline** using **Apache Airflow**, **dbt**, and **Snowflake**, automating data workflows from raw ingestion to transformation and validation.

---

## ✅ Problem We’re Solving

Data teams often face fragmented workflows between orchestration (Airflow) and transformation (dbt), leading to manual effort, poor lineage visibility, and debugging difficulty. This project demonstrates a **unified CI/CD pipeline** with:

- Automated staging and transformation of multiple tables.
- Role-based access and schema control on Snowflake.
- Integrated testing and lineage tracking via Airflow.

---

## 📌 Architecture Overview

![Architecture Diagram](https://github.com/techwthjul/airflow-dbt-snowflake-pipeline/blob/main/architecture.png)

> *Components used: Apache Airflow (DAGs), DBT (modular SQL models), Cosmos (Airflow-dbt integration), Snowflake (Cloud DWH).*

---

## 🛠️ Prerequisites

Before running this project, ensure the following:

- Docker & Docker Compose installed
- Snowflake account with:
  - A database (`dbt_db`)
  - A warehouse (`dbt_wh`)
  - A schema (`dbt_schema`)
  - A role (`dbt-role`) with access
- `astro dev` CLI installed (via Astronomer CLI)
- DBT CLI installed (for local testing)

---

## ⚙️ How It Works

- Airflow DAGs orchestrate the execution of dbt models using [Cosmos](https://astronomer.github.io/astronomer-cosmos/).
- dbt performs transformations on Snowflake data: staging (`stg_tpch_orders`), integration, and fact models.
- dbt tests are triggered and results shown in Airflow UI (XCom and Logs).
- Access control and schema validation are managed in Snowflake connection setup.

---

## 🎬 Live Demo

▶️ [Watch the Full Project Walkthrough on YouTube](https://www.youtube.com/watch?v=your-demo-video-id)

---

## 📂 Project Structure

