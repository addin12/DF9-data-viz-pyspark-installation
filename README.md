# Data Fellowship 9 Session 5: Data Visualization Assignment
Creating a Analytics Dashboard via BI tools (Looker Studio, Power BI, Tableau, Metabase, etc.) using Yellow New York Taxi Trip Records 2019
## Datasets  
- [Kaggle](https://www.kaggle.com/datasets/microize/newyork-yellow-taxi-trip-data-2020-2019?resource=download)  
- [NYC TLC](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
## Tools
- Google Cloud Storage
- Google BigQuery
- Looker Studio (formerly Google Data Studio)
## Steps
### 1. Ingest the data from datasets link into your GCS Bucket

![image](https://user-images.githubusercontent.com/25638454/225272700-c22bb826-d810-4c5b-8853-9a1d4f620c84.png)

### 2. Create your BigQuery dataset table from GCS bucket external table

![image](https://user-images.githubusercontent.com/25638454/225273880-96bb148c-cf7c-4ff6-9727-7d8d9b827b21.png)

### 3. Open [Looker Studio](https://lookerstudio.google.com/u/1/navigation/reporting) to create blank report

![image](https://user-images.githubusercontent.com/25638454/225274293-6c135b7a-e469-4f04-9f03-6403fc27f16f.png)

### 4. Add data connector to our report via BigQuery

![image](https://user-images.githubusercontent.com/25638454/225275157-d5a73a7f-041f-4011-840a-26dab31e1d8f.png)

### 5. Choose our created BigQuery table as this report data source

![image](https://user-images.githubusercontent.com/25638454/225275000-b2f8cb35-f96a-4a42-970e-9c696c5bd7fe.png)

### 6. Then create the dashboard as you want and need

![image](https://user-images.githubusercontent.com/25638454/225275359-232af061-0fba-4817-ba05-c387c99a4b57.png)
## Result
This is the result of a [Dashboard](https://lookerstudio.google.com/reporting/de713711-8297-4fd2-b7f4-cb41c883c73c) I made from Yellow Taxi Trip Records 2019. I made two sub-reports which explain taxi operations and financial reports. I made some scorecards for general insights and time-based trend(monthly and hourly) to know how their business behavior on 2019. 

![image](https://user-images.githubusercontent.com/25638454/225275756-99d080fd-a787-4e7f-b244-fbdc83a8b217.png)
    
# Data Fellowship 9 Session 5: pySpark Installation
PySpark is included in the official releases of Spark available in the Apache Spark website. For Python users, PySpark also provides pip installation from PyPI. This is usually for local usage or as a client to connect to a cluster instead of setting up a cluster itself.

This page includes instructions for installing PySpark by using pip, Conda, downloading manually, and building from the source.
