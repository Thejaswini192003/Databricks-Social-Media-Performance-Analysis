# Databricks Social Media Performance Analysis

## Project Overview
This project leverages Databricks to analyze social media performance across multiple platforms including LinkedIn, Instagram, Medium, and YouTube. The goal is to provide actionable insights on engagement, virality, and growth trends using Spark, PySpark, and Delta Lake.

Presentation video: https://www.linkedin.com/posts/thejaswinisv_kaggle-dataanalytics-socialmediainsights-share-7427749353647239168-NFBF?utm_source=share&utm_medium=member_desktop&rcm=ACoAADZiPxkBSxkrHMtWvfQ1PMt7p-KJ6XjfxII

Key objectives include:
- Aggregating social media performance metrics into a centralized Delta Lake table.
- Performing data cleaning, transformation, and enrichment using PySpark.
- Conducting correlation and statistical analysis to understand engagement patterns.
- Generating dashboards and reports for stakeholders to monitor performance trends.

## Technologies Used
- Databricks – Cloud-based data engineering and analytics platform
- Apache Spark & PySpark – Distributed data processing and transformations
- Delta Lake – Reliable data storage with ACID transactions
- Python – Data cleaning, transformation, and visualization
- Matplotlib / Seaborn / Plotly – Data visualization
- SQL – Querying and aggregating data within Spark SQL
- ML - logistic regression, decision tree, gradient boosting.

## Dataset
download the dataset from kaggle: https://www.kaggle.com/datasets/svthejaswini/social-media-performance-and-engagement-data
The project uses a consolidated social media dataset with the following key columns:  
- `platform` – Social media platform name (LinkedIn, Instagram, Medium, YouTube)  
- `views` – Total content views  
- `engagement_rate` – Engagement rate percentage  
- `is_viral` – Binary flag indicating viral content  
- `followers_count` – Number of followers/subscribers  
- `content_type` – Type of content (post, video, article, etc.)  
- `publish_date` – Date of content publishing  

The data is sourced from internal exports and public APIs, aggregated into Delta tables for consistency.

## Architecture
The project follows a Lakehouse architecture using Databricks:

1. **Raw Layer (Bronze)** – Raw social media data ingested from CSV/JSON sources  
2. **Cleaned Layer (Silver)** – Data cleaned, formatted, and enriched with computed metrics  
3. **Analytics Layer (Gold)** – Aggregated, transformed, and ready for reporting or visualization  

## Installation
1. Clone this repository
2. Open the project in Databricks workspace
3. Install required Python libraries:
pip install pyspark delta-spark matplotlib seaborn plotly pandas
4. Configure Databricks cluster with appropriate Spark and Python versions
