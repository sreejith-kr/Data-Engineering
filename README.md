**Covid Data Analyis**

**Objecive**

Develop a data ingestion pipeline in Azure Data Factory to appl ETL process to find Countries in EU with Highest Corona Virus Hospital Admissions. The dataset is from European Centre for Disease Prevention and Control(ECDC) repository. Make the data available for ML experts to predict the spread of the virus and the potential number of people who may be infected. This information is then used by governments to determine the policies and measures they need to put in place to effectively address the crisis.

**Architecture** : Pls see the Architecture folder for details.


**Data Ingestion**
The Extract part of ETL process is done here. The data is ingested from two sources:

**1. From Azure Blob:**

Ingest ”population by age” for all EU Countries into the Data Lake to support the machine learning models to predict increase in Covid-19 mortality rates.

**2. From http source to Azure Data Lake Data Ingestion**

Ingest data from https://www.ecdc.europa.eu/en/covid-19/data to Azure Data Lake via the Azure Datafactory.


**Transformation**

In this project , the transformation is done in two ways.
1. Data Transformation via the Azure Data factory Data Flow workflow.
2. Data Transformation via Databricks (community edition) after mounting the required storage A/C containers from Azure. This mount points has the files exteracted by the Azure Pipeline.

**Visualization**

The visualization is done using the PowerBi. Multiple charts have been prepared. The details are available in ppt.

**Output Files** : The processed files are available in processed folder.



