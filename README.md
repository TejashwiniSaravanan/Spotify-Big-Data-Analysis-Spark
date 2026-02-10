Spotify Big Data Analysis Spark
Analyzing 600k+ Spotify tracks using the Spark DataFrame API for ISM 6362: Big Data and Cloud-Based Tools at Seattle Pacific Univeristy

Spotify Big Data Analysis: Spark DataFrame API
Project Overview
This project involves a comprehensive exploratory data analysis (EDA) of the "Spotify Dataset 1921-2020," which contains over 600,000 tracks. Using the Spark DataFrame API, the analysis uncovers temporal music trends and audio characteristic patterns across a century of data.

Problem Statement
Analyzing datasets with hundreds of thousands of rows requires scalable tools. The goal was to efficiently process this large-scale dataset to identify how music features like popularity, danceability, and energy have evolved, while managing data quality issues like null values and inconsistent formatting.

Tools & Technologies
Language: Python (PySpark)

Engine: Apache Spark 3.3.0

Platform: Google Colab (Cloud-based environment)

Libraries: pyspark.sql, findspark

Approach / Architecture
Environment Setup: Initialized a SparkSession and configured the Java/Spark environment in the cloud.

Data Ingestion: Loaded the tracks.csv file, inferring the schema to ensure correct data types.

Data Cleaning: Selected relevant audio features, cast numeric columns to Double types, and calculated null counts for data validation.

Transformation & Aggregation: Grouped data by year to calculate moving averages of audio metrics and filtered tracks based on high-performance criteria (popularity > 80).

Storage: Exported the final processed yearly trends into both CSV and Parquet formats for optimized storage.

Key Results
Temporal Trends: Observed a steady increase in danceability from 2012 (0.59) to 2021 (0.67).

Popularity Insights: Identified that modern tracks (2019–2021) maintain significantly higher popularity scores compared to historical recordings.

High-Performers: Filtered a subset of 417 tracks released since 2000 that met the "Viral" criteria (High popularity + High danceability).

Course Context
This project was developed as part of the course ISM 6362 – Big Data and Cloud-Based Tools at Seattle Pacific University.
