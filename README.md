Big Data E-Commerce Analytics Project 

Overview

This project demonstrates a complete end-to-end big data analytics pipeline for an e-commerce platform. It integrates multiple big data technologies to handle data generation, storage, processing, analytics, and visualization.

The project focuses on analyzing customer behavior, transaction patterns, and product performance using both batch processing and integrated analytics techniques.

Technologies Used:

    Python – Data generation, processing, and visualization

    MongoDB – Document-oriented storage for users, products, and transactions

    Apache HBase (Dockerized) – Time-series and high-write data storage (user sessions, product metrics)

    Apache Spark – Batch processing, Spark SQL analytics, and integrated analytics

    Matplotlib / Pandas – Static data visualizations

How to Reproduce Key Results

1. Data Generation

Generate the synthetic e-commerce dataset by running:

    python dataset_generator.py
    python generate_transactions.py


This step creates JSON files for users, products, categories, and transactions.

2. MongoDB

Import the generated JSON files into MongoDB using MongoDB Compass.

Collections used:

    users

    products

    categories

    transactions

MongoDB is used to store transactional and catalog data due to its flexible document model.

3. Spark Analytics

    Start the Spark shell:

    pyspark


Run the Spark applications located in the spark/ directory:

batch_processing.py 
   – Batch processing, data cleaning, cohort analysis, and Spark SQL analytics

integrated_analytics.py 
   – Integrated analytics including Customer Lifetime Value (CLV) estimation

4. Visualizations

Run the scripts in the visualization/ directory to generate static plots:

    Sales performance over time

    Top products by total revenue

    Customer distribution by country

    Customer Lifetime Value (CLV) distribution

Generated images are saved in the report/images/ directory and embedded in the final report.

Results

The project produces the following analytical outcomes:

    Cohort analysis of user purchasing behavior based on registration period

    Customer Lifetime Value (CLV) estimation using integrated user and transaction data

    Sales trends analysis over time

    Product performance insights, including top-selling products

    Geographical customer distribution by country