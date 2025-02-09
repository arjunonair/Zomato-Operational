# Comprehensive Data Pipeline for Zomato Restaurants Analytics and Seamless Delivery Solutions

This project implements a comprehensive data pipeline for analyzing Zomato delivery operations and restaurant data in metropolitan areas. The pipeline integrates **Azure Data Factory** for data ingestion, **Azure Databricks** with **PySpark** and **Spark-SQL** for transformation and analytics, and a dashboard solution for visualization.

## Table of Contents
- [Project Overview](#project-overview)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Pipeline Flow](#pipeline-flow)
- [Steps to Reproduce](#steps-to-reproduce)
- [Data Sources](#data-sources)
- [Analytics and Insights](#analytics-and-insights)
- [Visualization and Dashboard](#visualization-and-dashboard)
- [Conclusion](#conclusion)
- [Screenshots](#screenshots)

## Project Overview

The project provides a data pipeline solution for Zomato’s restaurant dataset and delivery operations, focusing on enhancing delivery efficiency in metropolitan areas. This solution leverages **Azure Data Factory** for seamless data ingestion, **Azure Databricks** for advanced data processing, and a visualization dashboard for meaningful insights.

The goal is to deliver:
- **A seamless data pipeline**: From ingestion, transformation, to visualization.
- **Delivery operations insights**: Analysis to optimize delivery time, distance, restaurant efficiency, and service areas.

## Architecture

The architecture of the pipeline includes:
1. **Data Sources**: Multiple datasets, restaurant data and delivery logs.
2. **Data Ingestion with Azure Data Factory**: Ingest data from diverse sources like APIs, cloud storage, and databases into a **NoSQL landing zone** (e.g., Azure Cosmos DB).
3. **Azure Databricks for Data Processing**: Use **PySpark** and **Spark-SQL** for data cleaning, aggregation, and transformation. The data is refined into SQL-based materialized views for analytics.
4. **Dashboard**: A dashboard layer for visualizing key metrics like delivery time, order volume, and heat maps of delivery zones.

## Technologies Used
- **Azure Data Factory**: Data ingestion and orchestration.
- **Azure Databricks**: PySpark and Spark-SQL for processing large datasets.
- **Azure Blob Storage**: For data storage.
- **Azure SQL Database**: For data storage.
- **Cosmos DB**: NoSQL landing zone for ingesting and storing raw data.
- **Python**: Core language for data processing in Databricks.
- **SQL**: For materialized views and advanced querying in Databricks.

## Pipeline Flow

1. **Data Ingestion**:
   - Azure Data Factory ingests data from APIs, cloud storage, and CSV files into the **NoSQL landing zone**.
  
2. **Data Processing in Databricks**:
   - Data is transformed using PySpark for cleaning, filtering, and enrichment.
   - Key metrics and KPIs are calculated using **Spark-SQL**.
   - The cleaned data is stored in SQL-based materialized views for further analysis.
  
3. **Data Analytics**:
   - Delivery operations analytics such as average delivery times, busiest delivery hours, delivery distances, and zone-based delivery performance.
  
4. **Visualization**:
   - The insights are visualized on a **dashboard** showing key metrics and trends such as delivery delays, restaurant performance, and geographic heatmaps.

## Steps to Reproduce

1. Clone this repository.
    ```bash
    git clone https://github.com/arjunonair/Zomato-Operational.git
    ```

2. Set up Azure services:
    - **Azure Data Factory**: Create pipelines to ingest data into Cosmos DB or Blob Storage.
    - **Azure Databricks**: Set up a Databricks cluster with PySpark enabled.

3. Upload the datasets to Azure Blob Storage.

4. Configure Data Factory to read from the Blob and load data into Cosmos DB.

5. In Databricks, execute the notebooks to process data using PySpark.

6. Deploy materialized views using Spark-SQL.

7. Visualize the insights using Databricks dashboard or any BI tool like Power BI.

## Data Sources

The data sources used in this project include:
- **Zomato Restaurant Dataset**: Restaurant information, ratings, cuisine types, and service areas.
- **Delivery Logs**: Data on delivery times, order volumes, and geographic details of delivery zones.

## Analytics and Insights

Key insights generated by this pipeline:
- **Delivery Time Optimization**: Analyze delays and identify the factors contributing to longer delivery times.
- **Geospatial Delivery Patterns**: Use geographic data to optimize delivery zones and reduce delivery times.
- **Restaurant Performance**: Analyze restaurant efficiency based on order volume, delivery speed, and customer satisfaction.

## Visualization and Dashboard

This section contains screenshots and visualizations from the dashboard, providing key metrics and trends:

![Screenshot 2024-10-04 152557](https://github.com/user-attachments/assets/3fe6680d-d2bb-48e0-9ff0-9f9938d47611)

![Screenshot 2024-10-04 152653](https://github.com/user-attachments/assets/7f70f6ca-7a9e-414d-ae03-72d4a44ab41f)


---

## Conclusion

This project delivers an end-to-end data pipeline for analyzing Zomato restaurant data and delivery operations. By leveraging Azure services, we ensure scalability, automation, and valuable insights into the delivery operations in metropolitan areas.

---

