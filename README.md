# Spotify Data Pipeline and Data Analysis

<img width="854" alt="Data Pipeline" src="https://github.com/sabarishsubramaniam2000/Spotify-Data-Pipeline-And-Analysis/assets/84472301/2ece16cb-c403-470d-85ad-890cf1032414">

This project showcases a full end-to-end data pipeline built on AWS to store, transform, and analyze Spotify data, culminating in an interactive Tableau dashboard. It follows a structured workflow, leveraging AWS's robust suite of data tools to process, query, and visualize insights.

## Workflow Overview

- **Data Storage**
  Raw Spotify data is uploaded to an Amazon S3 bucket, serving as the initial staging area.

- **Data Transformation**
  AWS Glue ETL jobs handle data cleaning, enrichment, and restructuring. The processed data is saved to a separate S3 bucket acting as the data warehouse.

- **Data Cataloging**
  An AWS Glue Crawler scans the transformed data and updates the AWS Glue Data Catalog, generating a searchable database and table.

- **Data Querying**
  AWS Athena runs SQL queries directly on the S3-stored data, enabling flexible and efficient exploration.

- **Data Visualization**
  Tableau connects to Athena to build rich, interactive visualizations that reveal insights and trends from the Spotify dataset.

## Tableau Dashboard

<img width="880" alt="Spotify Tableau Dashboard" src="https://github.com/sabarishsubramaniam2000/Spotify-Data-Pipeline-And-Analysis/assets/84472301/2b3ba5db-8ec5-48e9-8144-12b3b5bad222">

<img width="885" height="530" alt="Screenshot 2025-07-12 at 5 16 33 PM" src="https://github.com/user-attachments/assets/582c841e-5b53-4f22-8a35-d7cb4999075f" />


- The dashboard delivers a clear summary of Spotify data insights, highlighting key patterns in artist popularity and music genre trends.  
- It showcases the **top 10 artists**, featuring their popularity scores and follower counts.  
- It also ranks the **top 15 music genres** by popularity, offering a view into audience preferences on the platform.  
- The dashboard compares the distribution of **explicit vs. non-explicit songs** and examines how artist popularity relates to their follower numbers.  
- Additionally, it spotlights the **top 10 genres** with the largest song counts, giving an overview of the variety within each category.  
Overall, the dashboard offers a well-rounded look at Spotify’s music trends and listener behaviors.

## Dataset
The dataset used in this project is publicly available on Kaggle: [Spotify Dataset 2023](https://www.kaggle.com/datasets/tonygordonjr/spotify-dataset-2023).
