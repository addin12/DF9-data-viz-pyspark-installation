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

This page includes instructions for installing PySpark by using pip. However you can installing with other methods like using Conda, downloading manually, and building from the source.  
## Using PyPI
PySpark installation using PyPI is as follows:  
![image](https://user-images.githubusercontent.com/25638454/225278149-fc529905-280c-437b-ba38-c214fb5577cb.png)  
If you want to install extra dependencies for a specific component, you can install it as below:  
![image](https://user-images.githubusercontent.com/25638454/225278544-65b0321e-e4ea-473d-b97d-8bd175903a86.png)  
For PySpark with/without a specific Hadoop version, you can install it by using PYSPARK_HADOOP_VERSION environment variables as below:  
![image](https://user-images.githubusercontent.com/25638454/225278788-79adeb0c-44fb-43a1-a6d5-e09e8ecea19a.png)  
The default distribution uses Hadoop 3.3 and Hive 2.3. If users specify different versions of Hadoop, the pip installation automatically downloads a different version and use it in PySpark. Downloading it can take a while depending on the network and the mirror chosen. PYSPARK_RELEASE_MIRROR can be set to manually choose the mirror for faster downloading.  
![image](https://user-images.githubusercontent.com/25638454/225279098-c640fa37-c5b1-430f-aad7-c12962fd00a0.png)  
It is recommended to use -v option in pip to track the installation and download status.  
![image](https://user-images.githubusercontent.com/25638454/225279314-3a73b66b-fde8-4c23-a2bc-b32ba94281bd.png)  
Supported values in PYSPARK_HADOOP_VERSION are:

- without: Spark pre-built with user-provided Apache Hadoop

- 2: Spark pre-built for Apache Hadoop 2.7

- 3: Spark pre-built for Apache Hadoop 3.3 and later (default)

Note that this installation way of PySpark with/without a specific Hadoop version is experimental. It can change or be removed between minor releases.

