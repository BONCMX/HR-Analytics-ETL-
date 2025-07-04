# 📊HR-Analytics-ETL-
#  ETL Data HR Analysis Project – Enrollee Profiling & Workforce Readiness

## 🚀 Project Overview

This project demonstrates a comprehensive **ETL (Extract – Transform – Load)** pipeline applied to a simulated workforce analytics dataset. The goal is to **collect, clean, and prepare** data for future analysis related to **employment prediction, training assessment**, and **urban development factors**.

Designed to mirror real-world enterprise pipelines, this project showcases key competencies required for **Data Analyst / BI Analyst / DA Engineer** roles — with a focus on clean code, modular processing, and insight readiness.

---

## 🗂️ Data Sources

The project integrates **diverse data formats** (Google Sheets, Excel, CSV, SQL, HTML) from multiple simulated business domains:

| Table Name              | Description                                             | Format      |
|-------------------------|---------------------------------------------------------|-------------|
| `enrollies_data`        | Basic demographic info (ID, name, gender, city)         | Google Sheet |
| `education`             | University info, education level, major discipline      | Excel       |
| `work_experience`       | Experience years, company type/size, last job info      | CSV         |
| `training_hours`        | Training time per user (from SQL)                       | MySQL       |
| `city_development_index`| Urban development index per city (public HTML table)    | HTML        |
| `employment`            | Target label – whether a candidate is employed or not   | SQL         |

---

## 🔄 ETL Pipeline

### ✅ Step 1: **Extract**

- Connected to:
  - Google Sheets via direct URL
  - Excel + CSV files from local sources
  - MySQL database using `SQLAlchemy`
  - Public HTML table using `pandas.read_html()`

> 📌 Demonstrates versatility across real-world data sources.

---

### 🧹 Step 2: **Transform**

Each dataset underwent robust **data wrangling and inspection**, including:

- ✅ Missing value imputation (using mode & custom logic)
- ✅ Categorical encoding (object → category)
- ✅ Outlier removal using **IQR method** for numeric fields
- ✅ Type optimization for memory efficiency
- ✅ Feature consistency checks (e.g., ID format, value alignment)

✔️ Over 6 datasets and ~19,000 rows cleaned to **production-grade standard**.

---

### 🛢 Step 3: **Load**

All cleaned DataFrames were loaded into a local `SQLite` database:

- Naming conventions followed **dim_** (dimension) and **fact_** (fact) schemas
- Stored as tables using SQLAlchemy engine for query-ready format

> 🔗 `data_warehouse.db` ready for downstream analytics (BI, modeling, clustering)

---

## 🔍 Key Highlights

- 🔄 Fully modular ETL pipeline: ready for automation
- 🔬 Outlier detection logic using **non-parametric IQR filter**
- 📉 Real-world challenges handled: mixed formats, public web tables, missing labels
- 🧠 Designed for advanced analytics: employment prediction, city-level segmentation

---

## 🛠 Tech Stack

| Tool / Library | Purpose                        |
|----------------|--------------------------------|
| Python         | Core scripting language        |
| Pandas         | Data wrangling and EDA         |
| SQLAlchemy     | Database connectivity           |
| MySQL / SQLite | Relational database support    |
| Matplotlib     | Visual inspection (optional)   |

---

## 💼 Career Relevance

This project reflects real job deliverables of:

- 📊 **Data Analysts**: EDA, data cleaning, and transformation
- 🧠 **ML Practitioners**: Clean target-ready datasets
- 🧱 **BI Developers**: Warehouse-ready structured schema
- ⚙️ **Data Engineers**: Multisource ETL architecture

---

## 🧠 Final Thoughts

> “In a world where data is abundant, the ability to **clean and prepare it with purpose** becomes your sharpest competitive edge.”

This project reflects not just technical skill, but a deep understanding of how to prepare data **for impact**. Ready for production. Ready for insight. Ready for the real world.

---

## 📬 Contact

**Name**: Anh Lộc đẹp trai vô địch khắp mọi vũ trụ  
**Email**: [your_email@example.com]  
**LinkedIn**: [Your LinkedIn Profile](#)  

---

