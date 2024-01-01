# Tokyo-Olympics-fabric-end-to-end

## Introduction
In an age where data is as vital as the events themselves, the Azure Data Engineering End-2-End Tokyo Olympics 2020 Project represents a transformative approach to managing and extracting value from data at scale. This project harnesses the full spectrum of Azure services to create a cohesive and powerful data pipeline, turning raw data into actionable insights that drive strategic decision-making and enhance the Olympic experience for participants and viewers alike.

## Workflow Overview

![Azure Data Engineering Project Workflow](https://github.com/azeemite1/Tokyo-Olympics-fabric-end-to-end/blob/main/Azure%20Data%20Engineering%20Project%20Workflow.jpg "Azure Data Engineering Project Workflow")


## Data Source
The process begins with the data source. For this project, the data is sourced from <a href = "https://github.com/azeemite1/Tokyo-Olympics-fabric-end-to-end/tree/main/data"> GitHub</a>, which suggests that the raw data for the Tokyo Olympics 2020 is stored in a repository on GitHub, making it accessible and version-controlled. This data can include various datasets such as athlete profiles, event schedules, results, and more.

## Data Ingestion
The next step involves ingesting the data into the Azure platform. Azure Data Factory is used for this purpose. It is a cloud-based data integration service that allows you to create data-driven workflows for orchestrating and automating data movement and data transformation. Data Factory enables the extraction of data from various sources, in this case, <a href = "https://github.com/azeemite1/Tokyo-Olympics-fabric-end-to-end/tree/main/data"> GitHub</a>, and then loads the data into a centralized storage using pipeline for further processing.

![Pipeline](https://github.com/azeemite1/Tokyo-Olympics-fabric-end-to-end/blob/main/pipeline.png "Pipeline")

### Raw Data Storage
Once ingested, the data is stored in Azure Data Lake Storage Gen2. This is an enterprise-wide hyper-scale repository for big data analytics workloads. It combines the capabilities of Azure Data Lake Storage Gen1 with Azure Blob Storage, providing a platform that is optimized for analytics. The data is stored in its raw form, making it available for processing and analysis.

![Azue Data Lake Gen 2 Storage Container](https://github.com/azeemite1/Tokyo-Olympics-fabric-end-to-end/blob/main/strorage%20container.png "Azure Data Lake Storage")

![Azue Data Lake Gen 2 Eaw Storage Container](https://github.com/azeemite1/Tokyo-Olympics-fabric-end-to-end/blob/main/raw.png "Raw Storage")

Data Transformation
Azure Databricks is used to transform the raw data. It is an analytics platform optimized for the Microsoft Azure cloud services platform. Databricks offers a collaborative environment with a workspace for data scientists, data engineers, and business analysts to work together. Data transformation involves cleaning, aggregating, and preparing the data for analysis. This step is crucial to ensure that the data is in the right format and quality to derive meaningful insights.

Transformed Data Storage
The transformed data is then stored again in Azure Data Lake Storage Gen2, but this time, it is stored in a processed form that is optimized for querying and analysis. This separation of raw and transformed data storage allows for more organized data management and governance.

Analytics
Azure Synapse Analytics, previously known as Azure SQL Data Warehouse, is used to perform analytics on the processed data. It is an analytics service that brings together enterprise data warehousing and Big Data analytics. It offers a unified experience to ingest, prepare, manage, and serve data for immediate BI and machine learning needs.

Visualisation/Dashboard
Finally, the insights derived from the analytics are visualized using Microsoft Power BI. This is a suite of business analytics tools that deliver insights throughout your organization. It enables connecting to hundreds of data sources, simplifying data prep, and driving ad hoc analysis. Power BI provides a platform to create reports and dashboards that are interactive, and can be shared with others.