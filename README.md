# big-data-analysis-platform-architecture

## On Premise Architecture
![alt text](https://github.com/lavoisierkai/big-data-analysis-platform-architecture-/blob/main/On%20Premise%20Architecture%20.jpg)

You can check below link for original Google Draw:
https://docs.google.com/drawings/d/1ubyRZXlChcelpsZFDKQfWKe3GGBa32qMk93ErVQ5UMU/edit?usp=sharing

### Data model architecture specification for HIVE(HDFS)
![alt text](https://github.com/lavoisierkai/big-data-analysis-platform-architecture-/blob/main/Hive.png)

• ODS: Operational Data Store, the operational data layer, which is structurally consistent with the incremental or full data of the source system. It is equivalent to a data preparation area, and at the same time it is responsible for the recording of basic data and historical changes. Its main function is to introduce basic data into the data warehouse.

• CDM: Common Data Model, the common dimensional model layer, subdivided into DWD and DWS. Its main function is to complete data processing and integration, establish consistent dimensions, construct reusable analysis and statistics-oriented detailed fact tables, and summarize common granularity indicators.

-DWD: Data Warehouse Detail, detailed data layer.

-DWS: Data Warehouse Summary, summarize the data layer.

• ADS：Application Data Service，Application data layer. Used by external applications.


## Cloud Based Architecture

Below is a sample pipline I have designed by using Google Cloud Platform. The function of the pipeline is to collect customer behaviors by using GA,GTM and Google Firebase.
Google pub/sub is a message querying tool to processing real time data, however, it is not necessary if clients only need <style>p{color:Black !important;}</style> features.

![alt text](https://github.com/lavoisierkai/big-data-analysis-platform-architecture-/blob/main/Cloud%20Based%20Architecture.png)
You can check below link for original Google Draw:
https://docs.google.com/drawings/d/1gNx9NtZdTjN_pVhkOZLEEeryTAC1pgRqUOXLwE4rhiU/edit?usp=sharing
