---
id: 515
name: 'BigQuery Fundamentals for Oracle Professionals'
type: Course
url: https://www.cloudskillsboost.google/course_templates/515
date_published: 2023-04-06
topics:

---

# [BigQuery Fundamentals for Oracle Professionals](https://www.cloudskillsboost.google/course_templates/515)

**Description:**

This course covers BigQuery fundamentals for professionals who are familiar with SQL-based cloud data warehouses in Oracle and want to begin working in BigQuery. Through interactive lecture content and hands-on labs, you learn how to provision resources, create and share data assets, ingest data, and optimize query performance in BigQuery. Drawing upon your knowledge of Oracle, you also learn about similarities and differences between Oracle and BigQuery to help you get started with data warehouses in BigQuery.

After this course, you can continue your BigQuery journey by completing the skill badge quest titled Build and Optimize Data Warehouses with BigQuery.

**Objectives:**

* Describe BigQuery’s architecture, resource provisioning, and data definition model.
* Create, secure, and share BigQuery data assets using best practices.
* Implement common patterns and best practices for designing schemas and ingesting data in BigQuery.
* Use best practices to optimize query performance and control costs in BigQuery.
* Compare and contrast the differences and commonalities between Oracle and BigQuery.

## BigQuery Architecture and Resource Provisioning

This introductory module summarizes the key details of BigQuery architecture and resource provisioning including how BigQuery utilizes slots to execute SQL queries and workload management in BigQuery. Drawing upon your knowledge of Oracle, this module also provides a high-level overview of the similarities and differences between Oracle and BigQuery architecture and resource provisioning to help you get started with BigQuery.

### Link - [BigQuery Architecture and Resource Provisioning](https://www.cloudskillsboost.google/course_templates/515/documents/375019)

* [BigQuery Architecture and Resource Provisioning](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-BQORA-I/M1/index.html)

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/515/quizzes/375020)

#### Quiz 1.

> [!important]
> **Which two statements about BigQuery resources are true? (Choose two.)**
>
> * [ ] BigQuery uses row-based storage.
> * [ ] BigQuery is optimized for high-read data.
> * [ ] Data on BigQuery is physically stored on the compute cluster.
> * [ ] The number of slots allotted to a query is independent of query complexity.
> * [ ] A BigQuery slot is a combination of CPU, memory, and networking resources.

#### Quiz 2.

> [!important]
> **What is one of the main reasons BigQuery can scale effectively to store and query large datasets?**
>
> * [ ] Storage and compute are handled separately and automatically scale to match consumption.
> * [ ] BigQuery relies on user-generated cached indexes to improve the performance of your queries.
> * [ ] BigQuery data is always stored in Cloud Storage buckets.
> * [ ] Users can manually launch and customize as many virtual machines as they need to process and store larger BigQuery datasets.

#### Quiz 3.

> [!important]
> **You have an application that uses Oracle as the backend database. The application currently takes snapshots of the Oracle tables every 1,000 entries and keeps the snapshots for 72 hours. You need to convert the backend database of the application to BigQuery and want to use the most efficient method to meet the same data retention level. What should you do?**
>
> * [ ] Back up the data to Oracle's Automatic Storage Management (ASM) and import it directly to BigQuery.
> * [ ] Use a Google Cloud Transfer Appliance to back up the BigQuery resource to another BigQuery resource.
> * [ ] Use BigQuery's time travel window.
> * [ ] Take snapshots of the BigQuery instance every 24 hours.

### Lab - [Monitoring BigQuery Workloads](https://www.cloudskillsboost.google/course_templates/515/labs/375021)

This lab teaches you to perform SQL executions and monitor their slot utilization.

* [ ] [Monitoring BigQuery Workloads](../labs/Monitoring-BigQuery-Workloads.md)

## BigQuery Data Definition Model

This module summarizes the key details of BigQuery's resource hierarchy and data definition model, including how to create datasets and tables in BigQuery. Drawing upon your knowledge of Oracle, this module also provides a high-level overview of the similarities and differences between the Oracle and BigQuery resource hierarchies and primary data types to help you start working with data in BigQuery.

### Link - [BigQuery Data Definition Model](https://www.cloudskillsboost.google/course_templates/515/documents/375022)

* [BigQuery Data Definition Model](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-BQORA-I/M2/index.html)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/515/quizzes/375023)

#### Quiz 1.

> [!important]
> **You work on Project A. You need to run a query on BigQuery datasets stored in Project B, which is another project in your organization. Where will the query charges be billed?**
>
> * [ ] To your user in Project A
> * [ ] To Project A
> * [ ] To Project B
> * [ ] To the owner of the dataset in Project B

#### Quiz 2.

> [!important]
> **In Oracle, tables are organized into schemas within a database. How does this compare with the data resource hierarchy in BigQuery?**
>
> * [ ] In BigQuery, tables are stored within schemas.
> * [ ] In BigQuery, datasets are stored within schemas.
> * [ ] In BigQuery, datasets are stored within tables.
> * [ ] In BigQuery, tables are stored within datasets.

#### Quiz 3.

> [!important]
> **What is the column limit per table in BigQuery?**
>
> * [ ] 10,000
> * [ ] Unlimited
> * [ ] 1,000
> * [ ] 5,000

## BigQuery and Google Cloud IAM

This module summarizes the key details of the Google Cloud Identity and Access Management (IAM) model, including how roles and permissions are applied to datasets and tables in BigQuery. Drawing upon your knowledge of Oracle, this module also provides a high-level overview of the similarities and differences in roles and permissions between Oracle and BigQuery to help you start securing and sharing your data in BigQuery.

### Link - [BigQuery and Google Cloud IAM](https://www.cloudskillsboost.google/course_templates/515/documents/375024)

* [BigQuery and Google Cloud IAM](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-BQORA-I/M3/index.html)

### Quiz - [Module 3 Quiz](https://www.cloudskillsboost.google/course_templates/515/quizzes/375025)

#### Quiz 1.

> [!important]
> **Your application uses Oracle as the backend database. You have a database-level account to perform the backend tasks for the application including creating tables and views, performing queries, and deleting tables. You want to migrate the backend database of your application to BigQuery and provision an account to perform the same tasks by using Google best practices. What should you do?**
>
> * [ ] Add a label to the BigQuery user with the keyword "superuser."
> * [ ] In Google Cloud's Identify and Access Management (IAM), create a service account for the application; in BigQuery, assign it the role of BigQuery data editor on the specific datasets.
> * [ ] Use the CREATE USER command at the database level.
> * [ ] In Google Cloud's Identify and Access Management (IAM), create a new user for the application, and assign it the role of BigQuery admin at the project level.

#### Quiz 2.

> [!important]
> **You want to follow Google-recommended practices to limit the rows of all tables in your dataset for a specific access group in your organization. What should you do?**
>
> * [ ] Copy the source tables within the dataset, manually delete rows in the copies, and share the resulting data tables with the group.
> * [ ] Create separate data tables within the original dataset and permission authorized views on top of the source data tables in the same dataset.
> * [ ] Handle the permissioning for data table row access at the Google Cloud project level.
> * [ ] Create a separate dataset as an authorized dataset based on the original source dataset.

### Lab - [Securing and Sharing BigQuery Datasets and Tables](https://www.cloudskillsboost.google/course_templates/515/labs/375026)

Lab description.

* [ ] [Securing and Sharing BigQuery Datasets and Tables](../labs/Securing-and-Sharing-BigQuery-Datasets-and-Tables.md)

## BigQuery Data Ingestion

This module summarizes the primary options and best practices for ingesting data into BigQuery, including batch data loading, streaming ingestion, and queries to external data sources. Drawing upon your knowledge of Oracle, this module also provides a high-level overview of the similarities and differences in data ingestion options between Oracle and BigQuery to help you start reading and loading your data into BigQuery.

### Link - [BigQuery Data Ingestion](https://www.cloudskillsboost.google/course_templates/515/documents/375027)

* [BigQuery Data Ingestion](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-BQORA-I/M4/index.html)

### Quiz - [Module 4 Quiz](https://www.cloudskillsboost.google/course_templates/515/quizzes/375028)

#### Quiz 1.

> [!important]
> **You want to automate the loading of external third-party data into BigQuery on a scheduled basis without writing any code. Which ingestion option can you use to automatically load external data without writing code?**
>
> * [ ] BigQuery Storage Write API for streaming ingestion
> * [ ] BigQuery Storage Write API for batch loading
> * [ ] BigQuery Data Transfer Service
> * [ ] Query materialization

#### Quiz 2.

> [!important]
> **Oracle can ingest streaming data by using Oracle Cloud Infrastructure (OCI) Streaming. How does BigQuery ingest streaming data?**
>
> * [ ] BigQuery can ingest streaming data by using the BigQuery Storage Write API.
> * [ ] BigQuery can ingest streaming data by using the Cloud Spanner API.
> * [ ] BigQuery can ingest streaming data by using a file uploaded to a table in BigQuery.
> * [ ] BigQuery can ingest streaming data by using the COPY command.

#### Quiz 3.

> [!important]
> **You are loading multiple CSV and JSON files into BigQuery and want to optimize for load speed. Which Google best practice can help to optimize load speed?**
>
> * [ ] Load compressed CSV and JSON files.
> * [ ] Load uncompressed CSV and JSON files.
> * [ ] Convert the CSV files to JSON files and then load only compressed JSON files
> * [ ] Convert the CSV and JSON files to binary formats because loading of CSV and JSON files are not supported in BigQuery.

## BigQuery Schema Design and Optimization

This module summarizes common patterns and best practices for designing and optimizing table schemas in BigQuery, including the use of nested and repeated fields, partitioning, and clustering. Drawing upon your knowledge of Oracle, this module also provides a high-level overview of the similarities and differences in schema usage and design between Oracle and BigQuery to help you start structuring and optimizing your data in BigQuery.

### Link - [BigQuery Schema Design and Optimization](https://www.cloudskillsboost.google/course_templates/515/documents/375029)

* [BigQuery Schema Design and Optimization](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-BQORA-I/M5/index.html)

### Quiz - [Module 5 Quiz](https://www.cloudskillsboost.google/course_templates/515/quizzes/375030)

#### Quiz 1.

> [!important]
> **In Oracle, indexes are applied as optimization techniques and can be created using primary and foreign keys or other columns in a table. How are indexes applied differently in BigQuery?**
>
> * [ ] BigQuery offers optional indexes such as search indexes that are automatically enforced at the dataset level.
> * [ ] BigQuery offers optional indexes such as search indexes on the columns defined in the table schema.
> * [ ] BigQuery offers optional indexes such as search indexes that are automatically enforced at the row level.
> * [ ] In BigQuery, indexes are automatically created and enforced at the schema level.

#### Quiz 2.

> [!important]
> **You are coming from a row-based system and want to migrate your table schemas to BigQuery. Which best practice can help you optimize your table schemas in BigQuery?**
>
> * [ ] Normalize your data as much as possible.
> * [ ] Apply search indexes to all numeric fields.
> * [ ] Identify rows that can be used to partition and cluster your data.
> * [ ] Identify columns that can be used to partition and cluster your data.

### Lab - [Designing BigQuery Table Schemas for Oracle Professionals](https://www.cloudskillsboost.google/course_templates/515/labs/375031)

In this lab, you learn how to define and query table schemas in BigQuery including how to create and query nested and repeated fields, partitioned tables, and clustered tables.

* [ ] [Designing BigQuery Table Schemas for Oracle Professionals](../labs/Designing-BigQuery-Table-Schemas-for-Oracle-Professionals.md)

## SQL in BigQuery

This module summarizes the key features and operations of the Google Standard SQL dialect used in BigQuery and best practices for optimizing query performance and controlling costs in BigQuery. Drawing upon your knowledge of Oracle, this module also provides a high-level overview of the similarities and differences in the SQL dialects and features between Oracle and BigQuery to help you start running and optimizing queries in BigQuery.

### Link - [SQL in BigQuery](https://www.cloudskillsboost.google/course_templates/515/documents/375032)

* [SQL in BigQuery](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-BQORA-I/M6/index.html)

### Quiz - [Module 6 Quiz](https://www.cloudskillsboost.google/course_templates/515/quizzes/375033)

#### Quiz 1.

> [!important]
> **You have an application that currently uses Oracle as the SQL backend. The application uses data aggregation queries to provide approximate summary values to users. You want to migrate from Oracle to BigQuery, and leverage the efficient data aggregation queries. What should you do?**
>
> * [ ] Use the BigQuery API to execute data aggregation commands.
> * [ ] Use data sketches in BigQuery.
> * [ ] Schedule the query by using the Query Editor V2.0.
> * [ ] Use the OVER clause in BigQuery to aggregate across window functions.

#### Quiz 2.

> [!important]
> **Which type of statements supported by Google Standard SQL allows you to execute multiple SQL statements in one request?**
>
> * [ ] Data manipulation language statements
> * [ ] Data control language statements
> * [ ] Data definition language statements
> * [ ] Procedural language statements

#### Quiz 3.

> [!important]
> **You need to explore a non-clustered table in BigQuery that has a billion rows. Which option is a cost-effective Google best practice to review a sample of the data?**
>
> * [ ] Run a query by using a SELECT * statement.
> * [ ] Export the data to Cloud Storage, download the exported data file, and review it.
> * [ ] Run a query by using a LIMIT clause.
> * [ ] Use table preview options in BigQuery to view data.

### Lab - [Working with SQL in BigQuery for Oracle Professionals](https://www.cloudskillsboost.google/course_templates/515/labs/375034)

In this lab, you create tables and views using DDL statements, update tables using DML statements, join data using SQL, and define custom user-defined functions (UDFs) and stored procedures.

* [ ] [Working with SQL in BigQuery for Oracle Professionals](../labs/Working-with-SQL-in-BigQuery-for-Oracle-Professionals.md)

## Course Resources

Student PDF links to all modules

### Document - [Course Resources](https://www.cloudskillsboost.google/course_templates/515/documents/375035)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
