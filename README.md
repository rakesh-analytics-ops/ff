

# Automation Solver
# Automated Data Cleaning Pipeline for Analytics, BI & ML Workflows
Overview

This repository contains a reusable, automated data cleaning pipeline that I use as the first step in all my analytics, BI, and machine learning projects.

The goal is simple: ensure every dataset entering the system is clean, standardized, and reliable before it is used for dashboards, SQL reporting, or predictive modeling.

⚙️ Key Features

Automatic file detection from a raw data folder

Duplicate record removal

Business-friendly missing value handling

Column name and whitespace standardization

Date and numeric format validation

Timestamped, BI-ready output generation

Execution logging for traceability

🏗 Project Structure
automation-solver/
│
├── data_raw/        # Drop new weekly files here
├── data_cleaned/   # Cleaned output auto-generated here
├── logs/           # Pipeline execution logs
│
├── cleaner.py      # Core cleaning engine
├── watcher.py     # Auto-run file detector
├── config.py      # Folder & path settings
├── requirements.txt
└── README.md
🚀 Setup & Usage
1. Install Dependencies
pip install -r requirements.txt
2. Start the Automation Service
python watcher.py
3. Run the Pipeline

Place any CSV file into the data_raw folder.
A cleaned, timestamped file will automatically be generated in the data_cleaned folder.

💼 Practical Use Case

This pipeline is designed to simulate real-world data ingestion workflows commonly used in analytics and data engineering teams. It enables downstream systems such as:

Power BI dashboards

SQL-based reporting

ML feature pipelines

To operate on consistent, high-quality data.

🔮 Roadmap

Data quality summary report (row counts, null %, duplicates removed)

Email or Slack alerts on pipeline failure

Cloud ingestion (Google Drive / AWS S3)

Scheduled execution (Cron / Windows Task Scheduler)

👤 Author

Rakesh Mahakur

Data Analyst | BI | Python Automation

GitHub: https://github.com/rakesh-analytics-ops
