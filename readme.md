#  Job-Market-Trends-Analyzer

End-to-end data pipeline that extracts job listings from an external API, processes the data in Databricks, and visualizes key hiring KPIs in Power BI.

---

##  Workflow

1. **Data Collection**: Python script fetches data from job postings API.
2. **ETL & Storage**: Databricks cleans, transforms, and stores data in Delta format.
3. **Dashboard**: Power BI connects to processed data and displays:
   - Total Job Postings
   - Hiring Trends
   - Company & Location Insights

---

##  Project Structure

├── data_pipeline/
│ ├── 01_ingest_jobs.ipynb # API ingest notebook (Bronze)
│ ├── 02_clean_jobs_silver.ipynb # Cleaning + schema fixes (Silver)
│ └── 03_gold.ipynb # Final Gold table prep
│
├── dashboard/
│ └── JobPostingsDashboard.pbix # Power BI report (Top Hiring, Trend, Map)
│
└── README.md


##  Dashboard Preview

> Includes KPIs:
- 📍 Unique Locations
- 📈 Monthly Trends
- 🏢 Top Hiring Companies
- 🌍 Job Distribution Map
- 📅 Average Job Age

---

##  Tech Stack

| Tool         | Purpose                     |
|--------------|------------------------------|
| **Python**   | API ingestion, pre-cleaning  |
| **Databricks** | ETL with PySpark, Delta Lake |
| **Power BI** | BI Dashboard & Data Viz      |

---

##  Author

👤 **Gayatri Ramchandra Vaidya**  