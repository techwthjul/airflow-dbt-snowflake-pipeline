# 🌐 Airflow + DBT + Snowflake ELT Pipeline

This project demonstrates a complete modular ELT (Extract, Load, Transform) data pipeline using Apache Airflow, dbt, and Snowflake. The pipeline automates raw data staging, transformation, and testing using dbt models orchestrated by Airflow DAGs.

---

## 🧩 What Problem Are We Solving?

Modern data teams face challenges in orchestrating scalable and testable data pipelines that ensure data quality and modular transformations. This project solves that by combining:
- **Airflow** for scheduling and DAG orchestration
- **DBT** for modular SQL-based transformations and testing
- **Snowflake** as the cloud data warehouse

---

## 📺 Live Demo (YouTube)

📹 [Watch the demo](https://www.youtube.com/watch?v=0OOGlrK5_HM)  
<table>
  <tr>
    <td>
      <a href="https://www.youtube.com/watch?v=0OOGlrK5_HM" target="_blank">
        <img src="https://img.youtube.com/vi/0OOGlrK5_HM/0.jpg" width="100%">
        <br><strong>ELT Pipeline using Airflow, DBT, Snowflake and Cosmos</strong>
      </a>
    </td>
</table>


---

## 🧱 Tech Stack

- Apache Airflow (Astro CLI)
- DBT (Data Build Tool)
- Snowflake Cloud Data Platform
- Cosmos (DBT-Airflow integration)
- Python
- SQL 
- Docker (via Astro CLI)

---

## 🧭 Architecture Diagram

![Architecture Diagram](https://github.com/techwthjul/airflow-dbt-snowflake-pipeline/blob/main/ChatGPT%20Image%20Jun%209%2C%202025%2C%2012_17_16%20PM.png?raw=true)

---

## ⚙️ Prerequisites

- ✅ Snowflake account & credentials with correct roles
- ✅ [Astro CLI](https://docs.astronomer.io/astro/cli/install-cli) installed
- ✅ Docker Desktop running
- ✅ Git installed

---

## 🚀 Getting Started

1. **Clone the repo**
   ```bash
   git clone https://github.com/techwthjul/airflow-dbt-snowflake-pipeline.git
   cd airflow-dbt-snowflake-pipeline
