# NYC 311 Data Pipeline & Complaint Trend Analysis

## Overview

This project analyzes NYC 311 service request data and demonstrates the evolution from an initial exploratory analysis into a scalable Python workflow.

What began as a large raw dataset analysis was expanded into a refreshable pipeline capable of pulling live data, validating records, and powering downstream reporting.

The project focuses on real-world analytics challenges including large data volumes, API ingestion, data cleaning, feature engineering, and trend analysis.

---

## Business Objective

Use NYC 311 complaint data to identify changes in service demand, complaint categories, and borough-level patterns that may help inform operational planning and resource allocation.

---

## Key Skills Demonstrated

- Python data analysis with pandas
- Large dataset processing using chunking
- API-based live data ingestion
- Data cleaning and transformation
- Deduplication and validation checks
- Feature engineering / category mapping
- Time-series trend analysis
- Year-over-year growth analysis
- Data storytelling with Jupyter notebooks
- Iterative workflow improvement

---

## Tools Used

- Python
- pandas
- Matplotlib
- Jupyter Notebook
- NYC Open Data API
- GitHub

---

## Project Structure

01_initial_analysis.ipynb
02_data_pipeline.ipynb
03_pipeline_analysis.ipynb
README.md

1. Initial Analysis Notebook

Exploratory analysis of approximately 7 million records focused on 2024–2025 data.

Includes:

Chunked CSV processing
Complaint grouping logic
Borough comparisons
Trend charts
Year-over-year category analysis
2. Data Pipeline Notebook

Built to improve scalability and refreshability.

Includes:

Live API data ingestion
Monthly batch extraction
Retry / backoff handling
Validation checks
Deduplication
Export of refreshed master dataset
3. Pipeline Analysis Notebook

Uses pipeline-generated data for updated reporting and extended trend analysis.

Includes:

2024–Present monthly trends
Updated complaint category analysis
Dynamic year-over-year comparisons
Partial-year handling for current data
Key Analytical Findings
Transportation complaints remained one of the largest demand categories.
Noise complaints showed strong year-over-year growth.
Housing-related complaints remained consistently high, especially heat/hot water requests.
Complaint activity demonstrated seasonal patterns across categories.
Borough-level demand patterns varied significantly.

## Real-World Challenges Solved

### Large Dataset Constraints
Initial raw data size required chunked processing to manage memory efficiently.

### Static Reporting Limitations
A one-time analysis workflow was upgraded into a reusable refreshable pipeline.

### API Reliability
Rate limiting was addressed through throttling, retries, and backoff logic.

### Data Quality
Duplicate detection, null checks, and date-range validation were performed before analysis.

## Key Analytical Findings

- Transportation complaints remained one of the largest demand categories.
- Noise complaints showed strong year-over-year growth.
- Housing-related complaints remained consistently high, especially heat/hot water requests.
- Complaint activity demonstrated seasonal patterns across categories.
- Borough-level demand patterns varied significantly.

## Why This Project Matters

This project demonstrates the ability to move beyond static dashboards and work through the full analytics lifecycle:

**Raw Data → Cleaning → Scalable Ingestion → Validation → Insight Generation**

## How to Run

1. Clone the repository  
2. Open notebooks in Jupyter  
3. Update local file paths if needed  
4. Run notebooks in numerical order  

## Future Enhancements

- Power BI dashboard integration  
- Automated scheduled refresh  
- Geographic mapping of complaints  
- Predictive trend modeling  
- SQL-based storage layer  

## Contact

**Nicholas Villiard**  
LinkedIn: [Add Your LinkedIn URL]  
GitHub: [Add Your GitHub Profile URL]
