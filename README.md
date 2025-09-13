# 🚀 AcidOnSpark-ETL

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Docker](https://img.shields.io/badge/Docker-Ready-blue?logo=docker)
![Spark](https://img.shields.io/badge/Apache%20Spark-ETL-orange?logo=apachespark)
![Airflow](https://img.shields.io/badge/Apache%20Airflow-Orchestration-brightgreen?logo=apacheairflow)
![License](https://img.shields.io/badge/License-MIT-green)

A **modern ETL pipeline** that combines the power of **Spark, Airflow, MinIO, Delta Lake, Hive, Presto, and Superset** into a fully containerized data ecosystem.  
Built for **scalable, fault-tolerant, and analytics-ready workflows**.  

📖 Learn more here:  
👉 [Doing ACID on Spark (Medium)]

---

## ⚡️ Features

- End-to-End ETL pipeline – from ingestion to visualization  
- Fully containerized using Docker  
- Horizontally scalable with Spark & Presto  
- ACID-compliant storage with Delta Lake  
- SQL-ready via Hive Metastore + Presto  
- Interactive dashboards with Superset  

---

## 🛠️ Tech Stack

🐍 Python 3 · 🐳 Docker · 🔥 Apache Spark · 🌬 Airflow · 📦 MinIO  
🗂 Delta Lake · 🐝 Hive · 🐬 MariaDB · ⚡ Presto · 📊 Superset  

---

## 🔧 How It Works

All components are containerized and can be started with simple `make` commands:

```bash
# 🔥 Spark
make spark        # Launch Spark master + one worker
make scale-spark  # Scale Spark workers horizontally

# 🌬 Airflow
make airflow      # Launch Airflow for workflow orchestration

# 📦 MinIO
make minio        # Start S3-compatible storage for data lake & Hive tables

# 🗂 Hive + 🐬 MariaDB
make hive         # Launch Hive Metastore + MariaDB as metastore DB

# ⚡ Presto
make presto-cluster  # Launch Presto coordinator + worker(s)
make presto-cli      # Open interactive Presto SQL CLI

# 📊 Superset
make superset     # Launch Superset for dashboards & BI
