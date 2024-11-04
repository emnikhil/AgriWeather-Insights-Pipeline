# AgriWeather Insights Pipeline

## Project Overview

An end-to-end data pipeline for ingesting, processing, and visualizing weather data, utilizing Apache Airflow, Dataproc, Hive, BigQuery, and Google Data Studio. This pipeline enables seamless extraction, transformation, and analysis of weather data from public APIs to deliver insightful analytics.

## Project Flow Diagram

![AgriWeather Insights Pipeline Flow Diagram](/images/agriWeather-drawio.png)

## Architecture

The pipeline consists of the following main components:

1. **Data Ingestion**: Weather data is ingested from public APIs using Apache Airflow for scheduling and orchestration.
2. **Data Processing**: Google Dataproc, powered by Apache Spark, is used for data cleaning, transformation, and aggregation.
3. **Data Storage**: Processed data is stored in Hive, enabling scalable data storage and easy query access.
4. **Data Fetching and Analysis**: BigQuery is used to fetch the stored data from Hive for further analysis.
5. **Data Visualization**: Insights are visualized in Google Data Studio, allowing for interactive analysis and reporting.

## Technologies Used

- **Apache Airflow**: Manages and schedules workflows for data ingestion and pipeline orchestration.
- **Google Dataproc**: Processes data using Apache Spark for cleaning and transformations.
- **Hive**: Stores processed data in a structured format.
- **BigQuery**: Queries and fetches data from Hive for analysis.
- **Google Data Studio**: Visualizes data and insights for easy interpretation.

## Data Flow

1. **Ingestion**: Apache Airflow ingests raw weather data from APIs.
2. **Processing**: Data is cleaned and transformed in Google Dataproc.
3. **Storage**: Processed data is stored in Hive.
4. **Fetching**: BigQuery is used to query and retrieve data from Hive.
5. **Visualization**: Data Studio visualizes insights from BigQuery.

## Setup Instructions

### Prerequisites
- Google Cloud account with Dataproc and BigQuery enabled.
- Apache Airflow instance configured.
- Hive installed on Google Cloud Dataproc.
- Public weather API access (e.g., OpenWeatherMap, WeatherAPI).

### Steps
1. **Set Up Apache Airflow**:
   - Define DAGs for data ingestion and orchestration.
   - Configure API access and scheduling.

2. **Configure Google Dataproc**:
   - Set up a Dataproc cluster with Hive and Spark installed.
   - Define Spark jobs for data cleaning and transformation.

3. **Create Hive Tables**:
   - Set up necessary tables in Hive to store processed weather data.

4. **Enable BigQuery to Access Hive Data**:
   - Configure BigQuery to fetch data from Hive for seamless access.

5. **Connect Google Data Studio**:
   - Link Data Studio to BigQuery and design visualizations for weather insights.

## Usage

1. **Start the Pipeline**:
   - Trigger the DAG in Apache Airflow to start the data ingestion process.

2. **View Data in Google Data Studio**:
   - Open Data Studio to analyze and interpret insights from the weather data.

### Steps to Set Up

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/emnikhil/AgriWeather-Insights-Pipeline.git
   cd AgriWeather-Insights-Pipeline