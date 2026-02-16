# Databricks Social Media Performance Analysis

## Project Overview

This project leverages Databricks Lakehouse architecture to analyze social media performance across multiple platforms including LinkedIn, Instagram, Medium, and YouTube.

The objective is to centralize engagement metrics into Delta Lake tables and generate actionable insights on engagement trends, virality, and growth patterns using Spark, PySpark, and Machine Learning.

 Presentation Video:  
https://www.linkedin.com/posts/thejaswinisv_kaggle-dataanalytics-socialmediainsights-share-7427749353647239168-NFBF?utm_source=share&utm_medium=member_desktop&rcm=ACoAADZiPxkBSxkrHMtWvfQ1PMt7p-KJ6XjfxII

---

## Key Objectives

- Aggregate social media performance data into centralized Delta tables  
- Perform data cleaning, transformation, and enrichment using PySpark  
- Conduct statistical and correlation analysis to understand engagement patterns  
- Build ML models to predict viral content  
- Generate dashboards and analytical reports for stakeholders  

---

## Technologies Used

- Databricks  
- Apache Spark  
- PySpark  
- Delta Lake  
- Python  
- Spark SQL  
- Matplotlib  
- Seaborn  
- Plotly  
- Machine Learning (Logistic Regression, Decision Tree, Gradient Boosting)

---

## Dataset

Download from Kaggle:  
https://www.kaggle.com/datasets/svthejaswini/social-media-performance-and-engagement-data

### Key Columns

- `platform` – Social media platform (LinkedIn, Instagram, Medium, YouTube)  
- `views` – Total content views  
- `engagement_rate` – Engagement rate percentage  
- `is_viral` – Binary flag indicating viral content  
- `followers_count` – Number of followers/subscribers  
- `content_type` – Type of content (post, video, article, etc.)  
- `publish_date` – Date of publishing  

Data is aggregated into Delta tables for consistency and reliability.

---

## Architecture (Lakehouse – Medallion Model)

### Bronze Layer – Raw Data
- Ingest raw CSV/JSON files
- Store as Delta tables
- Apply schema inference

### Silver Layer – Cleaned & Enriched
- Handle null values
- Perform type casting
- Create derived metrics
- Feature engineering

### Gold Layer – Analytics Ready
- Aggregated KPIs
- Platform-level performance metrics
- ML-ready dataset for virality prediction

---

## Machine Learning

Models Used:
- Logistic Regression
- Decision Tree
- Gradient Boosting

Evaluation Metrics:
- Accuracy
- Precision
- Recall
- ROC-AUC

---

## Insights Generated

- Platform-wise engagement comparison  
- Correlation between followers and virality  
- High-performing content types  
- Engagement trend analysis over time  
- Viral prediction probability scores  

---

## Installation

1. Clone this repository  
2. Open the project in Databricks Workspace  
3. Configure a Spark cluster  
4. Install required libraries

   
5. Upload dataset to DBFS or mount cloud storage  
6. Execute Bronze → Silver → Gold pipeline  

---

## Project Highlights

- End-to-end Lakehouse implementation  
- Distributed data processing using Spark  
- Delta Lake with ACID transactions  
- ML-based virality prediction  
- Production-style data engineering workflow  

---

## Author

**Thejaswini S.V**  
Data Analyst | Data Science Enthusiast | Lakehouse & ML Projects  
