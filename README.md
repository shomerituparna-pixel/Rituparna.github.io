# Automated Data Quality Validation Framework
A python framework that scans any dataset, detects data quality issues and denerates a complete data quality report with scoring and recommendations.

## Project Overview
Organisations these days rely heavily on accurate and high-quality data to make decisions. However, most datasets contain issues such as missing values, inconsistencies, wrong formats, duplicates, and outliers — all of which affect reporting and model performance.
This project provides an automated Python-based data quality validation framework that performs:
1. Schema validation
2. Missing value & completeness checks
3. Duplicate detection
4. Outlier detection
5. Data type consistency checks
6. Business rule validation
7. Correlation anomaly detection
8. Automated HTML + PDF Data Quality Report
9. Data Quality Score (0–100)
    
The system works on any CSV dataset and generates a ready-to-share report for stakeholders.

### Tech Stack
- Python
- Pandas, NumPy
- Scikit-Learn
- Plotly / Matplotlib
- Jinja2 (HTML rendering)
- ReportLab (PDF reporting)

### Core Features Implemented
1. Completeness Checks
- Missing values
- NULL % by column
- Blank string detection
2. Uniqueness Checks
- Duplicate rows
- Duplicate keys
- Duplicate proportion
3. Data Type Validation
- Type mismatches
- Unexpected column types
4. Outlier Detection
- IQR method
- Z-score detection
5. Business Rule Validation
- Custom rules per dataset
- Pass/Fail summary
6. Data Quality Score
- Completeness – 25%
- Uniqueness – 25%
- Consistency – 20%
- Valid Formats – 15%
- Business Rules – 15%

### Reports Generated
1. HTML Interactive Report
Contains:
- Missing value heatmaps
- Duplicate patterns
- Outlier plots
- Business rule summary
- Data Quality Score gauge
2. PDF Executive Report
- Summary table
- Key issues
- Recommendations
- Quality Score

### How to Run
1. Add your CSV file to the /data folder
2. Open the notebook:
notebooks/data_quality_analysis.ipynb
3. Run all cells — it generates:
- dq_report.html
- dq_report.pdf

#### Future Enhancements
- API endpoint to upload files
- Slack/Email alerting
- Data Quality Database store
- Rule-based anomaly detection

