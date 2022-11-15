Data Lake Project:
------------------
This README file descripe the project motivation and the approach to achieve the results

Background and motivation:
-------------------------
A music streaming startup is growing (Users and Song Database). They would like to move to Data Lake to make the best use of Data Lake capabilities by establish several data analysis over the available data and customers usage.
As they consolidate all usage within JSON file formats (Logs of user activities - Metadata with songs in the app). They are in a need for a Data Engineer skills to help them read those files and re-shape in a dimensional tables within shared S3.
This need to be achieved by creating ETLs to read the JSON files and Transform the data for splitting into fact/dimensional tables. Following that, it needs to extract this data through files and store in S3 directory back for processing by analyitical team.

How to achieve that:
--------------------
Simply, by follow below steps:

1. Build ETL pipeline to get data from S3
2. Load data from S3 and process the data to analytical tables using Spark
3. Once tables structured and created (fact/dimensional), we extract them back into S3 bucket
4. Will use a cluster within AWS to support the Spark processes
