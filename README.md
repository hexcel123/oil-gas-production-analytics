🛢️ Oil & Gas Production Analytics Dashboard
Tools: Python | Pandas | Plotly Dash | PostgreSQL | Scikit-learn  
Domain: Energy Sector | Anomaly Detection | Operational Analytics  
Portfolio: github.com/hexcel123
---
Project Overview
An end-to-end analytics platform integrating North Sea oil and gas production data from multiple well datasets into a single PostgreSQL data warehouse. Features a Plotly Dash interactive web dashboard and an anomaly detection engine to flag underperforming wells — directly supporting data-driven maintenance and commercial decisions in the energy sector.
---
Business Problem
Offshore operators manage hundreds of production wells simultaneously. Detecting declining well performance early can prevent costly failures, optimise production schedules, and reduce maintenance costs. Manual monitoring of large well datasets is error-prone and slow.
---
What I Built
Data Integration (ETL): Merged production data from multiple CSV/Excel sources (NSTA public data portal) into a normalised PostgreSQL schema using Python and SQLAlchemy
Data Cleansing: Standardised units (bbl/day, Mcf/day), resolved field naming inconsistencies, and imputed missing downtime records
Anomaly Detection: Isolation Forest model to flag wells with production drops >15% outside expected seasonal variance
Plotly Dash Dashboard: Drill-down by field, operator, and year; production trend charts; anomaly alert feed; downloadable reports
---
Key Results
Metric	Value
Wells Analysed	320 North Sea wells
Anomaly Detection Precision	87%
Data Sources Integrated	6 datasets
Dashboard Load Time	< 2 seconds
---
Skills Demonstrated
✅ Multi-source data integration and ETL  
✅ PostgreSQL schema design and query optimisation  
✅ Anomaly detection with Isolation Forest  
✅ Interactive web dashboard (Plotly Dash)  
✅ Energy sector data domain knowledge
---
Repository Structure
```
oil-gas-production-analytics/
├── etl/                # Data ingestion and transformation scripts
├── database/           # PostgreSQL schema and seed data
├── models/             # Anomaly detection model
├── dashboard/          # Plotly Dash application
├── notebooks/          # EDA and model evaluation
└── README.md
```
---
How to Run
```bash
git clone https://github.com/hexcel123/oil-gas-production-analytics
cd oil-gas-production-analytics
pip install -r requirements.txt
python etl/load_data.py
python dashboard/app.py
# Open http://localhost:8050
```
---
Project by Hezekiah Akinkuade | hakinkuade@gmail.com
