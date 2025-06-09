# Modular ELT Pipeline with Airflow, dbt, and Snowflake

This project demonstrates a modular ELT pipeline using Apache Airflow, dbt, and Snowflake. It automates data staging, transformation, and testing workflows using Cosmos dbt integration and Snowflake’s cloud data platform.

## 📽️ Live Demo
[![YouTube Demo](https://img.shields.io/badge/Watch-Demo-red?logo=youtube)](https://www.youtube.com/your-demo-link)

## 🧩 Architecture

![Architecture Diagram](airflow_dbt_snowflake_architecture.png)

## 🚀 Features

- Orchestrated ELT pipeline with Airflow DAGs
- dbt model execution via Cosmos
- Data transformation and testing on Snowflake
- Debugging and monitoring with Airflow Logs and XCom

## ✅ Prerequisites

- Docker with Astro CLI (`astro dev`)
- Snowflake account with appropriate roles
- Python 3.7+
- dbt-core and dbt-snowflake installed
- Git & VS Code (recommended)

## 🏗️ Stack Used

- Apache Airflow
- dbt-core with dbt-snowflake
- Cosmos dbt integration
- Snowflake
- Astro CLI (local environment)

## 🧪 To Run

1. Clone this repo:
   ```bash
   git clone https://github.com/your-username/modular-elt-airflow-dbt-snowflake.git
   cd modular-elt-airflow-dbt-snowflake
