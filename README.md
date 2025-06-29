# celebal_week-5_assignment

# 🚀 Advanced Data Pipeline & Database Migration

This project addresses key data engineering challenges by implementing robust solutions for data extraction, multi-format export, automated pipeline execution, and flexible database replication strategies.

---

## ✨ Project Objectives & Capabilities

This framework is designed to deliver the following core functionalities:

### 1. Copy Data from Database to CSV, Parquet, and Avro File Formats
We implement functionality to **extract data from a relational database** and export it into various standard file formats:
* **CSV (Comma Separated Values):** For broad compatibility and easy data sharing across different systems.
* **Parquet:** Optimized for efficient analytical queries, leveraging columnar storage, and optimizing performance in data warehousing or big data environments.
* **Avro:** For robust data serialization, compact storage, and effective management of schema evolution in data pipelines.

These diverse formats support a wide range of downstream use cases, including reporting, data warehousing, and distributed data processing.

### 2. Configure Schedule Trigger and Event Triggers to Automate the Pipeline Process
The pipeline is designed for automated execution using a dual-trigger approach:
* **Schedule-Based Triggers:** Configured to run the pipeline at regular, predefined intervals, ensuring timely execution for batch data movements.
* **Event-Based Triggers:** Set up to dynamically initiate pipeline execution in response to specific events, such as the arrival of new files or detected changes within a database.

This automation ensures hands-free, timely, and responsive data movement for both real-time and batch scenarios.

### 3. Copy All Tables from One Database to Another
We provide a comprehensive solution for **full database replication**. This involves dynamically identifying and copying *all* tables along with their complete datasets from a source relational database to a designated destination database. This capability ensures:
* Complete **schema consistency**.
* Full **data consistency** between the source and destination.

This is essential for robust backup strategies, database migration projects, and synchronizing different development or production environments.

### 4. Copy Selective Tables with Selective Columns from One Database to Another
For more controlled data transfer, the project supports **selective data migration**. This functionality allows for:
* Choosing **specific tables** to be copied from the source database.
* Selecting **specific columns** within those chosen tables for transfer.

This approach is highly valuable for supporting compliance requirements, minimizing transferred data volume, and aligning data movement precisely with business-specific needs for targeted data migration.

---

## 🛠️ Technologies 

* **Apache Spark (PySpark):** For scalable data processing.
* **Databricks Platform:** For development, execution, and orchestration.
* **Relational Databases:** As source and destination systems (e.g., via JDBC).
* **File Formats:** CSV, Parquet, Avro.
* **Databricks Workflows/Jobs:** For automation and scheduling.

---

## 📝 Usage & Application

This framework provides fundamental building blocks for various data engineering tasks, from data lake ingestion and reporting to database synchronization and specialized data transfers driven by compliance or performance requirements.

# 📁 Project Structure

Project Root/
├── Data_pipeline_code   # PySpark and ETL pipeline scripts  
├── sample_data       # Input CSV or mock data files  
├── manifest.mf           # Metadata or config file  
└── readme                # Project overview or instructions
