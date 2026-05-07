# NYC 311 Data Pipeline & Complaint Analysis (2024–2025)

## Overview
This project analyzes NYC 311 service request data and demonstrates the evolution from an initial exploratory analysis into a scalable Python data pipeline.

The pipeline ingests live data from the NYC Open Data API, processes millions of records efficiently, and produces a validated dataset for downstream analysis.

The automated workflow generates a refreshed dataset exceeding 8 million records and enables analysis of complaint trends across time, categories, and boroughs.

---

## Key Highlights
- Processes **8M+ records** using chunked data handling
- Live API ingestion with retry and backoff logic
- End-to-end pipeline from raw data to validated dataset
- Feature engineering for simplified complaint categorization

---

## Business Objective
Use NYC 311 complaint data to identify changes in service demand, complaint categories, and borough-level patterns to help inform operational planning and resource allocation.

---

## Data Source
This project uses the NYC Open Data 311 Service Requests dataset.

Primary Source:  
https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2020-to-Present/erm2-nwe9

- Initial analysis used a downloaded CSV extract  
- The pipeline version uses live API ingestion from the same source  

---

## Pipeline Architecture

- **Batch Data Extraction**  
  Monthly API queries were used to manage large data volumes and avoid truncation limits.

- **Chunked Processing**  
  Data was processed in 100,000-row chunks to improve memory efficiency and handle large datasets.

- **Data Cleaning & Standardization**  
  Column names were normalized and date fields were parsed into usable formats.

- **Data Validation**  
  Duplicate checks, null analysis, and date range verification were performed to ensure data quality.

- **Feature Engineering**  
  A `complaint_group` column was created to categorize complaint types into broader analytical groups.

- **Data Consolidation**  
  Processed chunks were combined into a unified dataset.

- **Final Output**  
  A validated dataset was exported for downstream analysis and reporting.

---

## Pipeline Output
- Rows Processed: 8,264,071  
- Duplicate Records: 0  
- Coverage Period: Jan 2024 – Apr 2026  
- Output Dataset: Validated master dataset for downstream analysis  

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

---

## Tools Used
- Python  
- pandas  
- Matplotlib  
- Jupyter Notebook  
- NYC Open Data API  
- GitHub  
- AI-assisted development (ChatGPT) for debugging and optimization  

---

## Project Structure

01_initial_analysis.ipynb
02_data_pipeline.ipynb
03_pipeline_analysis.ipynb
README.md


---

## Notebooks Overview

### 1. Initial Analysis Notebook
Exploratory analysis of approximately 7 million records focused on 2024–2025 complaint data.

Includes:
- Chunked CSV processing for large dataset handling  
- Complaint grouping and category mapping  
- Borough-level comparisons  
- Monthly trend visualizations  
- Year-over-year category analysis  

---

### 2. Data Pipeline Notebook
Built to improve scalability and support automated data refreshes.

Includes:
- Live API data ingestion  
- Monthly batch extraction  
- Retry and backoff handling for API reliability  
- Data validation checks  
- Deduplication of records  
- Export of refreshed master dataset  

---

### 3. Pipeline Analysis Notebook
Uses pipeline-generated data for updated reporting and extended trend analysis.

Includes:
- 2024–Present monthly trend analysis  
- Updated complaint category analysis  
- Dynamic year-over-year comparisons  
- Partial-year handling for current data  

---

## Real-World Challenges Solved

- **Large Dataset Constraints**  
  Managed memory limitations using chunked processing for millions of records.

- **Static Reporting Limitations**  
  Transformed a one-time analysis into a reusable, refreshable pipeline.

- **API Reliability**  
  Addressed rate limiting using throttling, retries, and backoff logic.

- **Data Quality**  
  Ensured reliability through duplicate detection, null checks, and validation steps.

---

## Key Analytical Findings

- Transportation complaints remained one of the largest demand categories  
- Noise complaints showed strong year-over-year growth  
- Housing-related complaints remained consistently high, especially heat/hot water requests  
- Complaint activity demonstrated seasonal patterns across categories  
- Borough-level demand patterns varied significantly  

---

## Why This Project Matters
This project demonstrates the ability to move beyond static analysis and work through the full analytics lifecycle:

**Raw Data → Scalable Ingestion → Cleaning → Validation → Insight Generation**

---

## How to Run

1. Clone the repository  
2. Open notebooks in Jupyter  
3. Update local file paths if needed  
4. Run notebooks in numerical order  

---

## Future Enhancements
- Power BI dashboard integration  
- Automated scheduled refresh  
- Geographic mapping of complaints  
- Predictive trend modeling  
- SQL-based storage layer  

---

## Contact
**Nicholas Villiard**  
LinkedIn: https://www.linkedin.com/in/nicholas-villiard/  
GitHub: https://github.com/nicholasvilliard  