# Nyc-Data-engineer
### Introduction
This project showcases the complete process of developing a Data Engineering and Analytics solution for addressing a real-world business challenge from start to finish
### Architecture 
![data_architecture](https://github.com/sahamsiddiqui/Nyc-Data-engineer/assets/52113462/f21cbb0d-2b2e-44dc-b255-f562f6865a58)

### Dataset

Parquet data, containing individual trip information from raw trip data from yellow cabs in NYC, is used.For location data, a CSV file containing Borough and zone information is augmented with pickup and drop-off location coordinates and other geometric data from a zipfile format on the same webpage. The geospatial data file in the zip includes the shapefile .shp
Find more about the data here-https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

### Technology Stack - 
The project is constructed using GCP and leverages their Cloud Storage for raw data storage, Compute Engine for VM machine instances, Mage.ai ETL tool, BigQuery data warehouse, and Looker for dashboard creation.

Language - python for data Engineering task; SQL for Analysis in BigQuery

### Project Overview:
Data Engineering Use Case:
- Raw data is extracted from the source system and stored in the Staging Area, a GCP object storage.
- The data pipeline, built on Mage, extracts data from the staging area to initiate the transformation process.
- The extracted data is cleaned and transformed using the Kimball star approach in the data pipeline.
- Transformed data is then uploaded to BigQuery.

Data Analysis Use Case:
- Analyzing NYC trip data using SQL and BigQuery.
-  Utilizing Looker dashboards for insights.


Checkout detailed description of the project on this [medium Blog](https://medium.com/@sahamsiddiqui/navigating-data-engineering-from-raw-data-to-business-insights-part-1-d4e4969004d8)
