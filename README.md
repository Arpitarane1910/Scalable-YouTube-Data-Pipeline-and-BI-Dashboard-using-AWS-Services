# 📊 YouTube Trending Data Pipeline & Dashboard

This project is focused on securely ingesting, transforming, and visualizing YouTube trending data to uncover insights across video categories and regional performance. The architecture leverages AWS cloud services to ensure scalability, performance, and interactivity at every stage of the data lifecycle.

---

## 🎯 Project Goals

- **Data Ingestion**: Develop a robust pipeline to ingest trending video data from multiple regional sources.
- **ETL Pipeline**: Transform raw CSV/JSON data into clean, structured formats using scalable AWS services.
- **Centralized Data Lake**: Store all ingested and transformed data in a secure, centralized Amazon S3 data lake.
- **Scalability**: Design the pipeline to handle increasing volumes of data efficiently over time.
- **Cloud Integration**: Utilize AWS infrastructure to process and manage data beyond local system limitations.
- **Reporting & Visualization**: Build an interactive dashboard to track trends, engagement metrics, and category-level performance.

---

## ☁️ AWS Services Utilized

| Service         | Purpose                                                                 |
|----------------|-------------------------------------------------------------------------|
| **Amazon S3**   | Object storage for raw and processed data with high durability         |
| **AWS IAM**     | Role-based access control to manage secure usage of AWS resources      |
| **AWS Glue**    | Serverless ETL for data cataloging, cleaning, and transformation       |
| **AWS Lambda**  | Serverless compute to trigger Glue jobs automatically on data arrival  |
| **Amazon Athena** | Run SQL queries directly on S3-stored data without needing ETL        |
| **Amazon QuickSight** | Create and share interactive dashboards for analytics and insights |

---

## 📁 Dataset Used

**Source**: [YouTube Trending Videos Dataset – Kaggle](https://www.kaggle.com/datasets/datasnaek/youtube-new)

This dataset provides daily snapshots of the top trending YouTube videos in multiple countries. Each region has a separate CSV file, containing up to 200 trending videos per day. Key features include:

- **Fields Included**:
  - Video title, channel title, publish time
  - Views, likes, dislikes, and comment counts
  - Video description and tags
  - `category_id` (referenced via regional JSON files)

The dataset enables region-based comparative analysis, category trends, and audience engagement metrics at scale.

---


## 📈 Architecture
![image](https://github.com/user-attachments/assets/cd25912e-f806-4ab9-8ea7-94c55c7e2085)

