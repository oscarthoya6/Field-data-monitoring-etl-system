# Overview

This project is a Python-based ETL (Extract, Transform, Load) pipeline designed to automate the flow of field data collected through KoboToolbox into Google Sheets for real-time monitoring and reporting.

It is built to support field operations teams by improving data visibility, quality tracking, and timely decision-making through automated data workflows.

# Problem Statement

Field data collected via mobile or web tools often remains fragmented, delayed, or unvalidated before analysis. This project solves that by:

- Automating data extraction from KoboToolbox
- Cleaning and standardizing incoming datasets
- Delivering structured outputs to Google Sheets for live monitoring

# System Architecture
KoboToolbox (Data Collection Platform)
        ↓
Python ETL Script (API Extraction)
        ↓
Data Cleaning & Transformation (pandas)
        ↓
Validation & Quality Checks
        ↓
Google Sheets (Monitoring Dashboard)

# Key Features
-Automated extraction of field data from KoboToolbox API
-Data cleaning and transformation using pandas
-Structured output to Google Sheets for reporting
-Basic data quality checks (missing values, duplicates, formatting)
-Modular ETL pipeline design for scalability
-Logging for process tracking and debugging

# Tech Stack
Python 
Pandas
KoboToolbox API
Google Sheets API
gspread / Google OAuth
dotenv (environment variables)

# ETL Workflow
1. Extract

Pulls raw submissions from KoboToolbox via API.

2. Transform
Cleans missing or inconsistent values
Standardizes dates and identifiers
Removes duplicates
Generates basic KPIs (optional)
3. Load

Pushes processed data into Google Sheets for live monitoring.

# Live Monitoring Dashboard

The pipeline outputs cleaned field data into a live Google Sheet:

https://docs.google.com/spreadsheets/d/1WWn-Ah5YzLmSmJMT1ObtBoLT-vRYQ7aOZrAYJCPNEtw/edit?usp=sharing

This acts as the real-time monitoring dashboard for field data collection.

# Output Use Case

The final Google Sheet acts as a live dashboard for field data, enabling:

Center-level tracking
Field officer performance monitoring
Data completeness checks
Daily submission summaries

