# Clickstream ETL Pipeline for E-commerce

This project simulates, processes, and loads user clickstream data from an e-commerce platform into Google BigQuery for dashboard analysis. It uses PySpark for transformation and Apache Airflow for orchestration.

## 📈 Use Case

Understand user behavior in an e-commerce site by analyzing page views, clicks, and session paths.

## 🔧 Tools & Technologies

- **PySpark**: ETL processing
- **Apache Airflow**: Scheduling & orchestration
- **Google BigQuery**: Cloud data warehouse
- **Docker**: (Optional) Local development

## 🧱 Pipeline Components

1. **Simulate**: Generate clickstream data (`simulate_clickstream.py`)
2. **Clean**: Apply data quality checks and transformations (`clean_clickstream.py`)
3. **Load**: Load the data into BigQuery (`load_to_bigquery.py`)
4. **Schedule**: Airflow DAG to automate the pipeline (`clickstream_etl_dag.py`)

## 🚀 Running the Pipeline

### With PySpark (Local)

```bash
spark-submit scripts/simulate_clickstream.py
spark-submit scripts/clean_clickstream.py
spark-submit scripts/load_to_bigquery.py
