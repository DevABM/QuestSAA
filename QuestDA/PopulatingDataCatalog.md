## Populating the data catalog. 
In this practice lab, you will
- use AWS Glue to create database in the data catalog. 
- Use an AWS Glue crawler to create a table in the data catalog. 
- Use Amazon Athena to query data in the table. 
- Run the inventory management application to ingest new inventory data with added columns. 
- Run the crawler again and perform an Athena query to check the new table. 

A data lake built on AWS uses Amazon Simple Storage Service Amazon S3 as its primary storage resource. Amazon S3 provides an optimal foundation for a data lake because of its virtually unlimited scalability and 99.99999999999% (11 9s) of data durability.

AWS Glue is fully managed, extract, transform and reload ETL service that can categorize your data, clean it, enrich it and move it reliably between various data stores and data streams. AWS Glue is serverless, so there is no infrastructure to set up or manage. With AWS Glue access and analyze data through one unified interface without loading it into multiple data silos. 
- AWS Glue consists of a central meta data repository known as the AWS Glue Data Catalog. 
- Each AWS account has one AWS Glue Data Catalog by AWS region. 
- The Data Catalog contains table definitions, job definitions, schemas, and other control information to help you manage your AWS Blue environment. 
- A database in the Data Catalog is a container that holds tables. You use database to organize your tables into separate categories. 
- When you define a table in the Data Catalog, you add it to your database. 
- A table can be in only one database. The table is the metadata definition that represents your data, including its schema. 
- A table in the data catalog consists of names of columns, data type definitions, the partition information and other metadata about your base dataset. 
- The actual data reminds in its original data store. 
- The tables in the data catalog do not contain data. 
You can use a crawler to populate the data catalog with the metadata tables definitions. A crawler is a program that connects to your data store. So it's a target.  Prioritized list of classifiers to determine the schema of your data and then creates meta data tables in the data catalog. 
- An AWS Glue connection is a data catalog object that stores for a particular data store, login credentials, URI strings, virtual private cloud information and more. 
- When you add a crawler to the data catalog for an Amazon S3 data store, you can specify an S3 path in your account or another account. 
- All folders and files contained in the path are crawled. A classifier reads the data in the data store. If you recognize the format of the data, it generates a schema. AWS Glue provides a set of built-in classifiers, but you can also create custom classifiers. 