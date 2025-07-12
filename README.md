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

https://public.tableau.com/app/profile/sabarish.subramaniam3258/viz/SpotifyDataAnalysis_17158893218970/SpotifyDataAnalysisDashboard

<img width="880" alt="Spotify Tableau Dashboard" src="https://github.com/sabarishsubramaniam2000/Spotify-Data-Pipeline-And-Analysis/assets/84472301/2b3ba5db-8ec5-48e9-8144-12b3b5bad222">

- The dashboard presents a concise overview of Spotify data insights, encompassing key aspects of artist popularity and music genre trends. It features the top 10 artists, showcasing their popularity metrics and followers. 
- Additionally, it ranks the top 15 genres by their popularity on Spotify, providing insight into listener preferences. 
- The dashboard also compares the prevalence of explicit and non-explicit songs and explores the relationship between artist popularity and follower count. 
- Lastly, it highlights the top 10 genres with the highest number of songs available, offering a glimpse into the breadth of musical content within each genre. 
- Overall, the dashboard provides a comprehensive snapshot of music consumption patterns and trends on Spotify.

## Dataset

The dataset used for this project can be found on Kaggle: [Spotify Dataset 2023](https://www.kaggle.com/datasets/tonygordonjr/spotify-dataset-2023).
