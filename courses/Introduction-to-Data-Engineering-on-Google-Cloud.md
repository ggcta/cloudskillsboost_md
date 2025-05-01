---
id: 1157
name: 'Introduction to Data Engineering on Google Cloud'
type: Course
url: https://www.cloudskillsboost.google/course_templates/1157
date_published: 2025-01-16
topics:
  - Data Analysis
---

# [Introduction to Data Engineering on Google Cloud](https://www.cloudskillsboost.google/course_templates/1157)

**Description:**

In this course, you learn about data engineering on Google Cloud, the roles and responsibilities of data engineers, and how those map to offerings provided by Google Cloud. You also learn about ways to address data engineering challenges.

**Objectives:**

* Understand the role of a data engineer.
* Identify data engineering tasks and core components used on Google Cloud.
* Understand how to create and deploy data pipelines of varying patterns on Google Cloud.
* Identify and utilize various automation techniques on Google Cloud.

## Course Introduction

This section welcomes you to the Introduction to Data Engineering on Google Cloud course, and provides an overview of the course structure and goals.

### Video - [Course Introduction](https://www.cloudskillsboost.google/course_templates/1157/video/521317)

* [YouTube: Course Introduction](https://www.youtube.com/watch?v=Ndg2jT_CIk0)

Hello, and welcome to Introduction to Data Engineering on Google Cloud. I'm Damon, and I am a curriculum developer at Google. Whether you already work in data engineering and want to learn how to be successful on Google Cloud, or you are looking to progress in your career, this course will help you get started. Through a series of lectures, quizzes, and hands-on labs, you will learn the fundamentals of data engineering on Google Cloud. This course was designed for data engineers or anyone interested in preparing and sorting datasets for further usage in their organization. This involves using tools such as, but not limited to, Dataflow, Dataproc, Cloud Composer, BigQuery, Bigtable, and Datastream. In this course, you learn about the duties and responsibilities of a data engineer, identify data engineering tasks and core components used on Google Cloud to accomplish those tasks, understand how to create and deploy data pipelines of varying patterns on Google Cloud, and identify and utilize various automation techniques on Google Cloud to complete data engineering tasks. The course is divided into six modules designed to address the learning objectives. First, you look at data engineering tasks and components on Google Cloud. Next, you explore data replication and migration. Then you explore each of the three main data pipeline patterns; extract and load, extract, load, and transform, and extract, transform, and load. You conclude the course by examining automation techniques important to a data engineer.

## Data Engineering Tasks and Components

This module provides an introduction to the role of a data engineer. It covers key concepts such as data sources and sinks, data formats, storage options on Google Cloud, metadata management, and the use of Analytics Hub for data sharing within and outside an organization.

### Video - [Module Introduction](https://www.cloudskillsboost.google/course_templates/1157/video/521318)

* [YouTube: Module Introduction](https://www.youtube.com/watch?v=n1BVcs5H5f8)

In this module, first you'll learn about the role of a data engineer. Second, we will cover the differences between a data source and a data sync. Then, we will review different types of data formats that a data engineer will encounter. The next topic addresses the options for storing data on Google Cloud. Then we cover the choices available for metadata management. Finally, we will look at the features of Analytics Hub, that allow you to easily share datasets both within and outside your organization.

### Video - [The Role of a Data Engineer](https://www.cloudskillsboost.google/course_templates/1157/video/521319)

* [YouTube: The Role of a Data Engineer](https://www.youtube.com/watch?v=ynZeQntvICU)

What does a data engineer do? At a basic level, a data engineer builds data pipelines. Why does the data engineer build data pipelines? Because they want to get their data into a place such as a dashboard, or report, or machine learning model, from where the business can make data-driven decisions. The data has to be in a usable condition so that someone can use this data to make decisions. Many times, the raw data is by itself not very useful. Once data becomes useful, the data engineer will often apply updates or transformations to add new value to the data. Of course, new data environments require data management practices to ensure currency and accuracy. Finally, data engineers create processes and operations to move data usage into production settings. In the most basic sense, a data engineer moves data from data sources to data syncs in four stages: replicate and migrate, ingest, transform, and store. The replicate and migrate stage of a data pipeline focuses on the tools and options to bring data from external or internal systems into Google cloud for further refinement. There are a wide variety of tools and options at your disposal. They will be covered in more detail throughout this course.

### Video - [Data Sources Versus Data Sinks](https://www.cloudskillsboost.google/course_templates/1157/video/521320)

* [YouTube: Data Sources Versus Data Sinks](https://www.youtube.com/watch?v=Rbr6_uM964k)

The ingest stage of a data pipeline is the point where data becomes a data source and is available for usage downstream. Think of a data source as the starting point of your data journey. It is raw, unprocessed data waiting to be transformed into valuable insights. Any system, application, or platform that creates, stores, or shares data can be considered a data source. Two examples of Google Cloud products used in the ingest phase are Cloud storage, a data lake holding various types of data sources, and Pub/Sub, an asynchronous messaging system delivering data from external systems. The transform stage of a data pipeline represents action taken on a data source to adjust, modify, join, or customize a data source so that it matches a specific downstream data or reporting requirement. There are three main transformation patterns: extract and load, extract, load, and transform, and extract, transform, and load. You explore each of these patterns in their own modules later in the course. The store stage of a data pipeline represents the last step when we deposit data in its final form. A data sync is the final stop in the data journey. It's where processed and transformed data is stored for future use, analysis, and decision-making. Think of it as the reservoir at the end of the river, where valuable information is collected and readily available. Two examples of Google Cloud products used in the store phase are BigQuery, a serverless data warehouse, and Bigtable, a highly scalable no SQL database.

### Video - [Data Formats](https://www.cloudskillsboost.google/course_templates/1157/video/521321)

* [YouTube: Data Formats](https://www.youtube.com/watch?v=AXZSmupbh_8)

Data exists in two primary formats, unstructured and structured. Unstructured data is information stored in a non-tabular form, such as documents, images, and audio files. Unstructured data is usually suited for Cloud Storage, but BigQuery also offers the capability to store unstructured data via object tables. There is also structured data, which represents information stored in tables, rows, and columns.

### Video - [Storage Solution Options on Google Cloud](https://www.cloudskillsboost.google/course_templates/1157/video/521322)

* [YouTube: Storage Solution Options on Google Cloud](https://www.youtube.com/watch?v=ln5kPPut2jc)

There are several key products on Google Cloud that are used by data engineers. One main product is Cloud storage. Unstructured data is usually well suited to be stored in Cloud Storage. Within Cloud Storage, objects are accessed by using HTTP requests, including ranged GETS to retrieve portions of the data. The only key is the object name. There is object metadata, but the object itself is treated as unstructured bytes. The scale of the system allows for serving large static content and accepting user-uploaded content including videos, photos, and files. Objects can be up to five terabytes each. Cloud Storage is built for availability, durability, scalability, and consistency. It's an ideal solution for hosting static websites and storing images, videos, objects, and blobs, and any unstructured data. Cloud Storage has four primary storage classes; standard storage, nearline storage, coldline storage, and archive storage. The classes are differentiated by the expected period of object access. You have a full range of cost effective storage services for structured data to choose from when developing with Google Cloud. No one size fits all, and your choice of storage and database solutions will depend on your application and workload. Cloud SQL is Google Cloud's managed relational database service. AlloyDB is a fully managed, high- performance PostgreSQL database service from Google Cloud. Spanner is Google Cloud's fully managed relational database service that offers both strong consistency and horizontal scalability. Firestore is a fast, fully managed, serverless, NoSQL document database built for automatic scaling, high performance, and ease of application development. BigQuery is a fully managed, serverless enterprise data warehouse for analytics. Bigtable is a high-performance NoSQL database service. Bigtable is built for fast key-value lookup and supports consistent sub-10 millisecond latency. The two key concepts in data engineering are that of the data lake and the data warehouse. A data lake is a vast repository for storing raw unprocessed data in various formats, including unstructured, semi-structured, and structured. It serves as a centralized storage solution for diverse data types, enabling flexible use cases like data science, applications, and business decision making. A data warehouse is a structured repository designed for storing pre-processed and aggregated data from multiple sources. Primarily used for long term business analysis, it enables efficient querying and reporting for informed decision making. Data warehouses often operate as standalone systems, independent of other data storage solutions. BigQuery is a fully managed, serverless enterprise data warehouse for analytics. BigQuery has built-in features like machine learning, geospatial analysis, and business intelligence. BigQuery can scan terabytes in seconds and petabytes in minutes. BigQuery is a great solution for online analytical processing, or OLAP, workloads for big data exploration and processing. BigQuery is also well-suited for reporting with business intelligence tools. BigQuery has several easy to use options for accessing data. The first is via the Google Cloud console's SQL editor. The second is via the bq command line tool which is part of the Cloud SDK. The last is via a robust REST API which supports calls in seven programming languages. BigQuery organizes data tables into units called datasets. These datasets are scoped to your Google Cloud project. When you reference a table from the command line in SQL queries or code, you refer to it by using the construct, project.dataset.table. Access control is through IAM and is at the dataset, table, view, or column level. In order to query data in a table or view, you need at least read permissions on the table or view.

### Video - [Metadata Management Options on Google Cloud](https://www.cloudskillsboost.google/course_templates/1157/video/521323)

* [YouTube: Metadata Management Options on Google Cloud](https://www.youtube.com/watch?v=SieqK7lhrgs)

Metadata is a key element to making data more manageable and useful across an organization. Dataplex is a comprehensive data management solution that allows you to centrally discover, manage, monitor, and govern distributed data across your organization. With Dataplex, you can break down data silos, centralize security and governance, while enabling distributed ownership, and easily search and discover data based on business contexts. Dataplex also offers built-in data intelligence, support for open-source tools, and a robust partner ecosystem, helping you to trust your data and accelerate time to insights. Dataplex lets you standardize and unify metadata, security policies, governance, classification, and data life cycle management across this distributed data. Another common use case is when your data is accessible only to data engineers, and is later refined and made available to data scientists and analysts. In this case, you can set up a lake to have the following: A raw zone for the data, which is accessed by data engineers and data scientists. A curated zone for the data, which is accessed by all users.

### Video - [Sharing Datasets using Analytics Hub](https://www.cloudskillsboost.google/course_templates/1157/video/521324)

* [YouTube: Sharing Datasets using Analytics Hub](https://www.youtube.com/watch?v=nnFaIYZx3qc)

Sharing data is challenging especially outside of your organization. You need to consider security and permissions, destination options for data pipelines, data freshness and accuracy, and finally, usage monitoring. Analytics Hub was created to meet these data sharing challenges. Analytics Hub helps organizations unlock the value of data sharing, leading to new insights and business value. With Analytics Hub, you create a rich data ecosystem by publishing and subscribing to analytics-ready datasets. Because data is shared in place, data providers are able to control and monitor how their data is being used. Analytics Hub provides a self-service way to access valuable and trusted data assets, including data provided by Google. Finally, Analytics Hub provides an opportunity to monetize data assets. Analytics Hub removes the tasks of building the infrastructure required for monetization.

### Video - [Lab Intro: Loading Data into BigQuery](https://www.cloudskillsboost.google/course_templates/1157/video/521325)

* [YouTube: Lab Intro: Loading Data into BigQuery](https://www.youtube.com/watch?v=4VjEt6reSis)

In this lab, you practice loading data into BigQuery. The primary objective of this lab is to load data into BigQuery using both the command-line interface and the Google Cloud console. You also experience loading several datasets into BigQuery and using the Data Description Language, or DDL.

### Lab - [Loading data into BigQuery](https://www.cloudskillsboost.google/course_templates/1157/labs/521326)

This lab focuses on how to ingest data into tables inside of BigQuery.

* [ ] [Loading data into BigQuery](../labs/Loading-data-into-BigQuery.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/1157/quizzes/521327)

## Data Replication and Migration

This module provides an overview of data replication and migration on Google Cloud. It covers the basic architecture, the 'gcloud' command-line tool, Storage Transfer Service, Transfer Appliance, and Datastream, along with their functionalities and use cases.

### Video - [Module Introduction](https://www.cloudskillsboost.google/course_templates/1157/video/521328)

* [YouTube: Module Introduction](https://www.youtube.com/watch?v=u8y0ZL-FY74)

In this module, first, you review the baseline Google Cloud data replication and migration architecture. Second, you will cover the options and use cases for the gcloud command line tool. Then you will review the functionality and use cases for the Storage Transfer Service. The next topic addresses the functionality and use cases for the Transfer Appliance. Finally, you will look at the features and deployment of Datastream.

### Video - [Replication and Migration Architecture](https://www.cloudskillsboost.google/course_templates/1157/video/521329)

* [YouTube: Replication and Migration Architecture](https://www.youtube.com/watch?v=ES1LVwZaa08)

The replicate and migrate stage of a data pipeline focuses on the tools and options to bring data from external or internal systems into Google Cloud for further refinement. Google Cloud provides a comprehensive suite of tools to migrate and replicate your data. Start replicating and migrating data by using tools like the 'gcloud storage' command, Transfer Appliance, Storage Transfer Service, or Datastream. You can then transform the data as needed before finally storing it within Google Cloud. Data can originate from on-premises or multi-cloud environments, including file systems, object stores, HDFS, and relational databases. Google Cloud offers options for one-off transfers, scheduled replications, and change data capture, ultimately landing data in Cloud Storage or BigQuery. Google Cloud provides additional workload migration with options for various database types. Leverage Database Migration Service for seamless transitions from Oracle, MySQL, PostgreSQL, and SQL Server. For other data formats or complex migrations, use ETL tools like DataFlow with a wide range of templates that handle NoSQL or non-relational databases. Your target destination can be Cloud SQL, AlloyDB, or BigQuery, depending on your needs. The ease of migrating data depends heavily on data size and network bandwidth. With one terabyte of data, a 100 gigabits per second network takes about two minutes to transfer, while the same size on a 100 megabits per second network takes 30 hours. The 'gcloud storage' command or Storage Transfer Service are suitable for smaller datasets. For larger datasets, consider Transfer Appliance for faster offline transfer.

### Video - [The gcloud Command Line Tool](https://www.cloudskillsboost.google/course_templates/1157/video/521330)

* [YouTube: The gcloud Command Line Tool](https://www.youtube.com/watch?v=dD4Hds0L2X0)

You can use the 'gcloud storage' command to transfer small to medium-sized datasets to Cloud Storage. The data can originate from various on-premise sources like file systems, object stores, or HDFS. The 'cp' command, shown in the code snippet, facilitates these ad-hoc transfers directly to Cloud Storage.

### Video - [Moving Datasets](https://www.cloudskillsboost.google/course_templates/1157/video/521331)

* [YouTube: Moving Datasets](https://www.youtube.com/watch?v=ZoGHYwmOR1c)

To move larger datasets, consider using Storage Transfer Service. Storage Transfer Service efficiently moves large datasets from on-premises, multicloud file systems, object stores (including Amazon S3 and Azure Blob Storage), and HDFS into Cloud Storage. It boasts high transfer speeds (up to tens of gigabits per second) and supports scheduled transfers for convenient data migration. Transfer appliance is Google's solution for moving massive datasets offline. Google provides the hardware, you transfer your data onto it, then ship it back. It is ideal for scenarios with limited bandwidth or very large transfers, and it comes in multiple sizes to suit your needs.

### Video - [Datastream](https://www.cloudskillsboost.google/course_templates/1157/video/521332)

* [YouTube: Datastream](https://www.youtube.com/watch?v=4frrH0UB2Bs)

Datastream enables continuous replication of your on-premises or multi-cloud relational databases such as Oracle, MySQL, PostgresSQ,L or SQL Server into Google Cloud. Datastream offers change data capture options for historical backfill or allows you to just propagate new changes with data landing in Cloud Storage or BigqQuery for analytics. You have flexibility in connectivity options and can selectively replicate data at the schema, table, or column level. Datastream enables real-time data replication from source systems for various use cases. It supports direct replication into BigQuery for analytics, allows custom data processing in Dataflow before loading into BigQuery, and facilitates event-driven architectures. Additionally, Datastream can be used with Dataflow templates for seamless database replication and migration tasks, making it a versatile tool for integrating data into Google Cloud. Datastream taps into the source database's write-ahead log (WAL) to capture and process changes for propagation downstream. Datastream supports reading the logging mechanisms for the specific source database such as LogMiner for Oracle, binary log for MySQL, PostgreSQL's logical decoding, and transaction logs from SQL Server. These change events such as inserts, updates, and deletes are then processed by Datastream and transformed into structured formats like Avro or JSON, ready for storage in Google Cloud, typically in BigQuery tables, enabling near real-time data replication for analytics and other use cases. Datastream event messages contain two main sections: generic metadata and payload. Metadata provides context about the data, like source table, timestamps, and related information. Payload contains the actual data changes in a key-value format, reflecting column names and their corresponding values. This structure allows for efficient and organized data replication and tracking of changes. Datastream event messages also include source-specific metadata in addition to generic metadata and payload. This metadata provides context about the data's origin within the source system, including details like the database name, schema, table, change type (such as INSERT), and other system-specific identifiers. This additional information helps track data lineage and understand the context of changes replicated from the source database. Datastream simplifies data replication by using unified data types to map between different source and destination databases. This means that regardless of whether your source data is in Oracle as number, MySQL as decimal, PostgreSQL, as numeric, or SQL Server as decimal, Datastream will consistently represent it as decimal during replication. When this data lands in Google Cloud, it can be further transformed into format-specific data types in different file types or destinations, such as Avro as decimal, JSON as number, or stored natively in BigQuery tables as numeric. This ensures data type consistency and compatibility across different database systems, streamlining the data replication process. In summary, Google Cloud offers several data migration and replication options. The 'gcloud storage' command is suitable for smaller online transfers. Storage Transfer Service handles larger online transfers efficiently. Transfer Appliance is ideal for massive offline data migrations, and Datastream provides continuous online replication of structured data, supporting both batch and streaming velocities. Choose the option that best fits your data size, transfer type, and data availability requirements.

### Video - [Lab Intro: Datastream: PostgreSQL Replication to BigQuery](https://www.cloudskillsboost.google/course_templates/1157/video/521333)

* [YouTube: Lab Intro: Datastream: PostgreSQL Replication to BigQuery](https://www.youtube.com/watch?v=M9FnojDCRT0)

In this lab, you use Datastream to replicate data from PostgreSQL to BigQuery. You prepare and load a Cloud SQL for PostgreSQL instance. You create Datastream connection profiles for the source and target. You then create a Datastream processing stream and start replication. Finally, you validate the replication in BigQuery.

### Lab - [Datastream: PostgreSQL Replication to BigQuery](https://www.cloudskillsboost.google/course_templates/1157/labs/521334)

In this lab you will replicate data from a PostgreSQL database to BigQuery.

* [ ] [Datastream: PostgreSQL Replication to BigQuery](../labs/Datastream-PostgreSQL-Replication-to-BigQuery.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/1157/quizzes/521335)

## The Extract and Load Data Pipeline Pattern

This module focuses on data extraction and loading processes on Google Cloud, particularly with BigQuery. It covers the basic extraction and loading architecture, the bq command-line tool, BigQuery Data Transfer Service, and BigLake as an alternative to traditional extract-load patterns.

### Video - [Module Introduction](https://www.cloudskillsboost.google/course_templates/1157/video/521336)

* [YouTube: Module Introduction](https://www.youtube.com/watch?v=4FJvxi-spdg)

In this module, first, you review the baseline extract and load architecture diagram. Second, you explore the options of the bq command line tool. Then, you review the functionality and use cases for the BigQuery Data Transfer Service. Finally, you look at the functionality and use cases for BigLake as a non extract-load pattern.

### Video - [Extract and Load Architecture](https://www.cloudskillsboost.google/course_templates/1157/video/521337)

* [YouTube: Extract and Load Architecture](https://www.youtube.com/watch?v=pWTh92YnHUo)

The extract and load data pipeline pattern focuses on the tools and options to bring data into BigQuery by eliminating the need for upfront transformation. Extract and load greatly simplifies data ingestion into BigQuery. Extract and load leverages tools like 'bq load' and Data Transfer Service to directly load data from various sources or uses external tables and BigLake tables to make data accessible via BigQuery. This pattern also offers scheduling capabilities and eliminates the need for data copying, promoting efficiency in data pipelines. BigQuery provides extensive flexibility in data handling. It supports loading data from various formats like Avro, Parquet, ORC, CSV, JSON, as well as Google Cloud Firestore exports. Similarly, you can export BigQuery artifacts, including query results and table data, into formats like CSV, JSON, Avro, and Parquet, facilitating easy integration with other tools and systems. BigQuery offers two ways to load data: through its friendly user interface for file uploads, or via the LOAD DATA SQL statement. The UI simplifies the process, allowing you to select files, specify formats, and even auto-detect schema. LOAD DATA provides more control, ideal for automation and appending or overriding existing tables.

### Video - [The bq Command Line Tool](https://www.cloudskillsboost.google/course_templates/1157/video/521338)

* [YouTube: The bq Command Line Tool](https://www.youtube.com/watch?v=-Al2502VDRI)

The Cloud SDK's bq command offers a programmatic way to interact with BigQuery. You can create BigQuery objects like datasets and tables, put the familiar Linux command, bq mk. The bq load command efficiently loads data into BigQuery tables. Key parameters for bq load include specifying the source format such as CSV, skipping header rows, and defining the target dataset and table. You can load data from multiple files in Cloud Storage using wildcards and optionally provide a schema file for the table structure. These options provide flexibility and control for loading data into BigQuery from various sources.

### Video - [BigQuery Data Transfer Service](https://www.cloudskillsboost.google/course_templates/1157/video/521339)

* [YouTube: BigQuery Data Transfer Service](https://www.youtube.com/watch?v=Mn0-MvbAngY)

The BigQuery Data Transfer Service enables seamless loading of structured data from diverse sources, like SaaS applications, object stores, and other data warehouses into BigQuery. The service provides scheduling options for recurring or on-demand transfers, along with configuration options for data source details and destination settings. It is a managed and serverless solution, eliminating infrastructure management overhead. In addition, its no code approach simplifies data transfer setup and management.

### Video - [BigLake](https://www.cloudskillsboost.google/course_templates/1157/video/521340)

* [YouTube: BigLake](https://www.youtube.com/watch?v=CbAmAHNRU_4)

BigQuery's data access capabilities extend beyond its own storage. BigQuery allows you to query data residing in sources like Cloud Storage, Google Sheets, and Bigtable using external tables. Additionally, BigLake tables provide a way to query data across Cloud Storage, and even other cloud object stores, expanding BigQuery's reach and flexibility for data analysis. BigQuery offers flexibility in analyzing structured data. You can load data into permanent BigQuery tables for high-performance analytics, but with data movement involved. External tables allow you to query data directly in Cloud Storage without loading it into BigQuery, which is suitable for less frequent access. BigLake tables provide the best of both worlds: high-performance analytics on data in Cloud Storage without the need to load it into BigQuery, and without data movement. BigQuery external tables bridge the gap between Google Sheets and BigQuery, enabling direct querying of sheets data within BigQuery. By specifying the Google Sheets URL and format, users can treat the sheet as a table in BigQuery, simplifying data analysis across platforms. However, be aware that querying external tables may have limitations, like slower performance and the unavailability of cost estimation, table preview, and query caching. BigLake extends BigQuery's capabilities, providing a unified interface to query data directly from your data lake and other sources without moving or copying it. BigLake leverages Apache Arrow for efficient data handling and offers fine-grained security and metadata caching. With BigLake, you can seamlessly access data across data lakes and data warehouses using familiar BigQuery tools. BigLake tables provide a seamless querying experience, allowing you to interact with data stored in external sources, like Cloud Storage, just like you would with data in native BigQuery tables. You can use standard SQL queries to access and analyze the data within BigLake tables, including SELECT statements and joins. Behind the scenes, BigLake leverages metadata caching to enhance query performance, even though the data physically resides outside BigQuery. However, some features like query cost estimation and table preview are not available for BigLake tables due to the external nature of the data. BigLake maintains a metadata cache. The cache stores details about external data. For example, it can contain details about Parquet files stored in Cloud Storage, such as file size, row count, and column statistics like minimum/maximum values. This cache allows querying via BigQuery to skip listing all objects, prune files, and partitions faster, and enable dynamic predicate pushdown, resulting in improved query performance. The cache allows querying by Spark to access metadata statistics that the Spark-BigQuery connector can leverage to speed up queries. The metadata cache has configurable staleness from 30 minutes to seven days, and it can be refreshed automatically or manually. External tables in BigQuery require users to have separate permissions for both the table itself and the underlying data source. This can lead to more complex access management. BigLake tables offer a streamlined approach. Access is delegated through a service account decoupling table access from the data source. This simplifies permission management and enhances security. In summary, both external and BigLake tables enable querying data residing outside of BigQuery, but BigLake offers broader capabilities. BigLake supports a wide range of data formats and storage locations, including object stores across multiple cloud providers, and provides advanced security features like column-level and row-level security. External tables are simpler to set up, but lack fine-grained security controls. BigLake tables offer enhanced performance, security, and flexibility for querying external data, making them suitable for enterprise data lake use cases.

### Video - [Lab Intro: BigLake: Qwik Start](https://www.cloudskillsboost.google/course_templates/1157/video/521341)

* [YouTube: Lab Intro: BigLake: Qwik Start](https://www.youtube.com/watch?v=W10IlLwPZbY)

In this lab, you use BigLake to connect to various external data sources. You configure a connection resource and set up access to a Cloud Storage data lake. You create and query a BigLake table and set up access control policies. Finally, you upgrade an existing external table to be a BigLake table.

### Lab - [BigLake: Qwik Start](https://www.cloudskillsboost.google/course_templates/1157/labs/521342)

In this lab, you will learn how to implement BigLake tables.

* [ ] [BigLake: Qwik Start](../labs/BigLake-Qwik-Start.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/1157/quizzes/521343)

## The Extract, Load, and Transform Data Pipeline Pattern

This module provides an overview of ELT (extract, load, transform) processes on Google Cloud. It covers the basic ELT architecture, a common ELT pipeline example, BigQuery's capabilities for scripting and scheduling SQL, and the functionality and use cases of Dataform.

### Video - [Module Introduction](https://www.cloudskillsboost.google/course_templates/1157/video/521344)

* [YouTube: Module Introduction](https://www.youtube.com/watch?v=xeUkgVVEoGo)

In this module, first, you review the baseline extract, load, and transform architecture diagram. Second, you look at a common ELT pipeline on Google Cloud. Then you review BigQuery's SQL scripting and scheduling capabilities. Finally, you look at the functionality and use cases for Dataform.

### Video - [Extract, Load, and Transform (ELT) Architecture](https://www.cloudskillsboost.google/course_templates/1157/video/521345)

* [YouTube: Extract, Load, and Transform (ELT) Architecture](https://www.youtube.com/watch?v=7HUvm61x0b4)

Extract, load, and transform centers around data being loaded into BigQuery first. Once data is loaded, there are multiple ways to transform it. Procedural languages like SQL can be used to transform data. Scheduled queries can be used to transform data on a regular basis. Scripting and programming languages like Python can be used to transform data. And a tool like Dataform simplifies transformation beyond basic programming options. In an extract, load, and transform pattern pipeline, structured data is first loaded into BigQuery staging tables. Transformations are then applied within BigQuery itself using SQL scripts or tools like Dataform with SQL workflows. The transformed data is finally moved to production tables in BigQuery ready for use. This approach leverages BigQuery's processing power for efficient data transformation.

### Video - [SQL Scripting and Scheduling with BigQuery](https://www.cloudskillsboost.google/course_templates/1157/video/521346)

* [YouTube: SQL Scripting and Scheduling with BigQuery](https://www.youtube.com/watch?v=SW3JMSV3nVo)

With support for procedural language, BigQuery allows the execution of multiple SQL statements in sequence with shared state. This enables the automation of tasks like table creation, implementation of complex logic using constructs like IF and WHILE, and the use of transactions for data integrity. You can also declare variables and reference system variables within your procedural code. BigQuery supports user-defined functions, or UDFs, for custom data transformations using SQL or JavaScript. These UDFs can be persistent or temporary, and it is recommended to use SQL UDFs when possible. JavaScript UDFs offer the flexibility to use external libraries, and community-contributed UDFs are available for reuse. Stored procedures are pre-compiled SQL statement collections, streamlining database operations by encapsulating complex logic for enhanced performance and maintainability. Benefits include reusability, parameterization for flexible input, and transaction handling. Stored procedures are called from applications or within SQL scripts, promoting modular design. BigQuery supports running stored procedures for Apache Spark. Apache Spark stored procedures on BigQuery can be defined in the BigQuery PySpark editor or using the CREATE PROCEDURE statement with Python, Java, or Scala code. The code can be stored in a Cloud Storage file or defined inline within the BigQuery SQL editor. Remote functions extend BigQuery's capabilities by integrating with Cloud Run functions. This enables complex data transformations using Python code. You define the remote function in BigQuery, specifying the connection and endpoint to your Cloud Run function. This function can then be called directly within your SQL queries, similar to a UDF, allowing for seamless integration of custom logic. The example here shows a Python function that gets a list of signed URLs pointing to Cloud Storage objects and returns the length for these objects. In BigQuery, we just need to register the function. We call it object_length(). Then, we can use it as is in SQL. Jupyter Notebooks coupled with BigQuery DataFrames facilitate efficient data exploration and transformation. This integration emphasizes the ability to handle large datasets that exceed runtime memory, perform complex data manipulations using SQL or Python, and schedule notebook executions. The seamless integration of BigQuery DataFrames and popular visualization libraries further streamlines the entire process. BigQuery offers the option to save and schedule queries for repeated use. You can save queries, manage versions, and share them with others. Scheduling allows you to automate query execution by setting frequency, start and end times, and result destinations. Dataform is recommended for more complex SQL workflows. Often, there are needs to perform additional tasks after a scheduled query is executed in BigQuery. These include tasks such as triggering subsequent SQL scripts, running data quality tests on the output, or configuring security measures. In an ideal situation, these actions can be automated, ensuring data pipelines remain efficient and reliable.

### Video - [Dataform](https://www.cloudskillsboost.google/course_templates/1157/video/521347)

* [YouTube: Dataform](https://www.youtube.com/watch?v=zdRQzqTwXNE)

Dataform is a serverless framework that simplifies the development and management of ELT pipelines using SQL, Dataform enables data transformation within BigQuery, ensuring data quality and providing documentation, This approach streamlines the process of moving data from source systems to production tables in BigQuery, making operations more efficient and manageable, Dataform streamlines data operations in BigQuery by unifying transformation, assertion, and automation, Without Dataform, tasks like defining tables, managing code, testing data quality, and scheduling pipelines would be time-consuming and prone to errors, They could also involve multiple tools and manual processes, Dataform simplifies these tasks within BigQuery, improving efficiency and data reliability, Dataform and BigQuery work together to manage SQL workflows, With Dataform, developers create and compile SQL workflows using SQL and JavaScript, Dataform then performs real-time compilation, including dependency checks and error handling, Finally, the compiled SQL workflows are executed within BigQuery, enabling SQL transformations and materialization either on-demand or through scheduled runs, Development using Dataform utilizes workspaces containing default files and folders, Key folders include 'definitions' for sqlx files and 'includes' for JavaScript files, The ,gitignore file is used for managing Git commits, Developers may also use package,json and package-lock,json for handling JavaScript dependencies, The 'workflow settings,yaml' file stores, project compilation settings, and custom files like README,md can also be added, The sqlx file structure provides a clear framework for organizing SQL code and associated tasks, It begins with a config block for metadata and data quality tests, followed by a js block to define reusable JavaScript functions. The pre_operations block handles SQL statements executed before the main SQL body, which defines the core SQL logic. Finally, the post_operations block contains SQL statements to be run after the main execution, ensuring a structured and efficient workflow. sqlx development streamlines SQL code by replacing repetitive patterns with concise definitions. The code example demonstrates how a complex CASE statement for categorizing countries can be replaced with a simple function call $(mapping.region("country")). This approach improves code readability and maintainability by reducing boilerplate code and promoting reusability. With Dataform, table and view definitions should be created in a specific manner so that they can be compiled into SQL statements. Key configuration types are: declaration for referencing existing BigQuery tables. table for creating or replacing tables with a SELECT statement, incremental for creating tables and updating them with new data, and view for creating or replacing views, which can optionally be materialized. Dataform offers assertions to define data quality tests, ensuring data consistency and accuracy. Assertions can be written in SQL or JavaScript, providing flexibility for complex checks. Operations allow you to run custom SQL statements before, after, or during pipeline execution. These two options enable custom data transformations, data quality checks, and other tasks within your workflows. By combining assertions and operations, Dataform empowers you to create robust and reliable data pipelines in BigQuery. Dataform provides two methods to manage dependencies, implicit declaration and explicit declaration. Implicit declaration is when you reference tables or views directly within your SQL using the ref() function. Explicit declaration is when you list dependencies within a config block using the dependencies array. It is also possible to use the resolve() function to reference without creating a dependency. Dataform allows you to compile user-defined table definitions into executable SQL scripts. The sample code shows a customer_details table being created or replaced based on a customer_source table using a SELECT statement. Dataform manages the dependencies between these tables and orchestrates their execution within a workflow. This process streamlines data transformation and ensures efficient data pipeline management. Dataform SQL workflows are best visualized in graph format. The sample workflow starts with a declaration of customer_source followed by a customer_intermediate table, likely derived from a source system as a pre-processed data source. Next, customer_rowConsistency applies assertions for data quality checks. The graph then splits into two paths. In one path, an operation named customer_ml_training is invoked. It performs operations on the validated data. In the other path, a view named customer_prod_view is created. There are several scheduling and execution mechanisms for Dataform SQL workflows. One path is through internal triggers. These include manual execution in the Dataform UI or scheduled configurations within Dataform itself. The other path is through external triggers. These include tools like Cloud Scheduler and Cloud Composer. Ultimately, all workflows are executed within BigQuery, showcasing its central role in this process.

### Video - [Lab Intro: Create and Execute a SQL Workflow in Dataform](https://www.cloudskillsboost.google/course_templates/1157/video/521348)

* [YouTube: Lab Intro: Create and Execute a SQL Workflow in Dataform](https://www.youtube.com/watch?v=PMDta9Ydk_8)

In this lab, you use Dataform to create and execute a SQL workflow. First, you create a Dataform repository. Second, you create and initialize a Dataform development workspace, then you create and execute a SQL workflow. Finally, you view execution logs in Dataform to confirm completion.

### Lab - [Create and execute a SQL workflow in Dataform](https://www.cloudskillsboost.google/course_templates/1157/labs/521349)

This lab walks you through the process to create and execute a SQL workflow in Dataform to load data in BigQuery.

* [ ] [Create and execute a SQL workflow in Dataform](../labs/Create-and-execute-a-SQL-workflow-in-Dataform.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/1157/quizzes/521350)

## The Extract, Transform, and Load Data Pipeline Pattern

This module provides an overview of ETL (extract, transform, load) processes on Google Cloud. It covers the basic ETL architecture, GUI tools, batch and streaming data processing options (Dataproc, Dataproc Serverless), and the role of Bigtable in data pipelines.

### Video - [Module Introduction](https://www.cloudskillsboost.google/course_templates/1157/video/521351)

* [YouTube: Module Introduction](https://www.youtube.com/watch?v=h4DwiOcJtho)

In this module, first, you review the baseline extract, transform, and load architecture diagram. Second, you look at the GUI tools on Google Cloud used for ETL data pipelines. Third, you review batch data processing using Dataproc. Then, you examine using Dataproc Serverless for Spark for ETL. Next, you review streaming data processing options on Google Cloud. Finally, you examine the role Bigtable plays in data pipelines.

### Video - [Extract, Transform, and Load (ETL) Architecture](https://www.cloudskillsboost.google/course_templates/1157/video/521352)

* [YouTube: Extract, Transform, and Load (ETL) Architecture](https://www.youtube.com/watch?v=m8am0U-gCFw)

The extract, transform, and load data pipeline pattern focuses on data being adjusted or transformed prior to being loaded into BigQuery. Google Cloud offers a variety of services to handle distributed data processing. For developers who prefer visual interfaces, there are user-friendly tools like Dataprep and Data Fusion. If you favor open-source frameworks, Dataproc and Dataflow are an option. And to streamline your workflows, template support is provided across various stages of data processing, from extraction and loading to full-fledged transformation.

### Video - [Google Cloud GUI Tools for ETL Data Pipelines](https://www.cloudskillsboost.google/course_templates/1157/video/521353)

* [YouTube: Google Cloud GUI Tools for ETL Data Pipelines](https://www.youtube.com/watch?v=gGW6duNZfWQ)

Dataprep by Trifacta simplifies data transformation by offering a serverless, no-code solution. It connects to various data sources, provides pre-built transformation functions, and allows users to chain these functions together into recipes. The resulting transformation flows can be executed seamlessly with Dataflow, while also providing capabilities for scheduling and monitoring. Dataprep provides a visual interface where you can see the impact of your data transformations before applying them. It also offers intelligent suggestions to help you refine your data cleaning and preparation process, like extracting specific values or replacing patterns within your data. Data Fusion is a user friendly, GUI-based tool designed for enterprise data integration. Data Fusion seamlessly connects to various data sources, both on-premises and in the cloud. You can build data pipelines without coding using its drag-and-drop interface and pre-built transformations. The platform is extensible, allowing for custom plugins, and it executes on powerful Hadoop/Spark clusters for efficient processing. Data Fusion Studio easily allows the creation of data pipelines with visual tools. The example pipeline shows two SAP tables being used as data sources. The two tables are joined together and then one outbound leg is written to a Cloud Storage bucket. The other leg undergoes an Add-Datetime transformation and is outputted to BigQuery. The pipeline also highlights the ability to preview data at different stages.

### Video - [Batch Data Processing Using Dataproc](https://www.cloudskillsboost.google/course_templates/1157/video/521354)

* [YouTube: Batch Data Processing Using Dataproc](https://www.youtube.com/watch?v=oQYWHvH4K6Q)

Dataproc allows you to seamlessly run your Apache Hadoop and Spark workloads on Google Cloud. You can leverage HDFS data stored on Cloud Storage and use Dataproc to perform transformations with Spark jobs. The results can then be easily stored in various destinations like Cloud Storage, BigQuery, or NoSQL databases like Bigtable, all within the Google Cloud ecosystem. Dataproc is Google Cloud's managed service for data processing using Hadoop and Spark. It offers flexibility with runtimes on GCE, GKE, and Serverless Spark, and provides a rich, open-sourced ecosystem. Dataproc simplifies cluster management with workflow templates, autoscaling, and the option for both permanent and ephemeral clusters. It also integrates seamlessly with other Google Cloud storage services, eliminating the need for disk-based HDFS. Dataproc clusters on Google Compute Engine offer flexible storage options. Clusters can utilize HDFS on persistent disks for cluster storage, or leverage other Google Cloud storage services like Cloud Storage for persistent data. Additionally, Dataproc integrates with BigQuery and Bigtable using connectors, enabling seamless interaction with these data stores. This setup allows users to choose the most suitable storage solution for their specific needs while taking advantage of Dataproc's processing capabilities. Dataproc Workflow Templates allow you to define and manage complex data processing workflows with dependencies between jobs. You can specify these workflows in a YAML file, providing details about the jobs like Hadoop or Spark, their order of execution, and any required parameters. These templates can then be submitted to Google Cloud using the gcloud command line tool, where they will be executed on either a managed ephemeral cluster or an existing predefined cluster. Apache Spark is a versatile framework for data processing, offering various capabilities through its components like Spark SQL for structured data, Spark Streaming for real-time data, MLlib for machine learning, and GraphX for graph processing. Spark supports multiple languages including R, SQL, Python, Scala and Java, making it accessible to a wide range of users. With these features, Spark excels in tasks like data engineering, machine learning, analytics, and many more. Dataproc Serverless for Spark simplifies Spark workload execution by eliminating cluster management. It offers automatic scaling, cost efficiency with pay-per-execution pricing, faster deployment, and no resource contention. Users can focus solely on writing and executing their code, making it ideal for various Spark use cases like batch processing, interactive notebooks, and Vertex AI pipelines. Dataproc Serverless for Spark offers two main execution modes: Serverless for batches and Serverless for interactive notebook sessions. Batches are submitted using the gcloud command-line tool and are ideal for automated or scheduled jobs. Interactive sessions leverage JupyterLab, either locally or within the Google Cloud environment, for interactive development and exploration. The platform also supports features like BigQuery external procedures, templates, custom containers, and a pay-as-you-go pricing model. Dataproc Serverless for Spark seamlessly integrates with various Google Cloud services, enhancing its functionality and usability. It leverages Dataproc History Server and Dataproc Metastore for persistent storage and metadata management. It interacts with BigQuery for data warehousing and analytics, and with Vertex AI workbench for machine learning tasks. Additionally, it utilizes Cloud Storage and other storage services for data storage and retrieval. Behind the scenes, it creates and manages ephemeral clusters for efficient job execution. The lifecycle of an interactive notebook session begins with its creation, where various configurations like runtime version and network settings are defined. Once active, the session allows for code development and execution, with the kernel transitioning between idle and busy states. The session eventually reaches a shutdown phase, either manually triggered or due to inactivity, leading to the kernel being shut down and its state becoming unknown.

### Video - [Lab Intro: Use Dataproc Serverless for Spark to Load BigQuery](https://www.cloudskillsboost.google/course_templates/1157/video/521355)

* [YouTube: Lab Intro: Use Dataproc Serverless for Spark to Load BigQuery](https://www.youtube.com/watch?v=Wq6PjZrsJSo)

In this lab, you use Dataproc Serverless for Spark to load BigQuery. First, you configure the environment. Next, you download lab assets. You then configure and execute the Spark code. Finally, you view the data in BigQuery.

### Lab - [Use Dataproc Serverless for Spark to Load BigQuery](https://www.cloudskillsboost.google/course_templates/1157/labs/521356)

This hands-on lab shows you how to use Dataproc Serverless for Spark to load BigQuery.

* [ ] [Use Dataproc Serverless for Spark to Load BigQuery](../labs/Use-Dataproc-Serverless-for-Spark-to-Load-BigQuery.md)

### Video - [Streaming Data Processing Options](https://www.cloudskillsboost.google/course_templates/1157/video/521357)

* [YouTube: Streaming Data Processing Options](https://www.youtube.com/watch?v=_TLVlZwg_lA)

Batch processing involves analyzing a fixed set of store data, suitable for tasks like payroll or billing systems. On the other hand, streaming data processing handles a continuous flow of data from various sources, making it ideal for real-time applications like fraud or intrusion detection. Streaming ETL workflows on Google Cloud involve the continuous ingestion of event data, often through Pub/Sub. This data is often processed in real-time using Dataflow, allowing for transformations and enrichment. Finally, the processed data is loaded into various destinations like BigQuery for analytics, enabling near real-time insights, or a Bigtable for NoSQL storage. Pub/Sub can efficiently manage high volumes of event data. Pub/Sub acts as a central hub, receiving events like 'New employee' or 'New contractor' from various sources. Pub/Sub then distributes these events to relevant systems like badge activation, facilities, and account provisioning, ensuring reliable delivery and enabling decoupled, asynchronous communication between systems. Dataflow leverages the Apache Beam programming framework to efficiently process both batch and streaming data. This unified approach simplifies development, allowing you to use languages like Java, Python, or Go. Dataflow seamlessly integrates with other Google Cloud services and offers features like a pipeline runner, serverless execution, templates, and notebooks for a streamlined experience. This code example demonstrates how to use Apache Beam to stream messages from Pub/Sub, transform them using a parsing function, and then write the results into BigQuery. The ReadFromPubSub function retrieves messages, Beam. Map() applies the parsing transformation, and WriteToBigQuery loads the transformed data into a specified BigQuery table, creating the table if necessary and appending new data to it. Dataflow templates allow you to create reusable pipelines for recurring tasks. You can separate the pipeline design from its deployment, making it easier to manage and update. By using parameters, you can customize the pipeline for different inputs, increasing its versatility. These templated pipelines can be easily deployed through various methods, and Google provides pre-built templates for common scenarios.

### Video - [Bigtable and Data Pipelines](https://www.cloudskillsboost.google/course_templates/1157/video/521358)

* [YouTube: Bigtable and Data Pipelines](https://www.youtube.com/watch?v=5nYcpP20X-A)

Bigtable is an excellent choice for handling streaming data pipelines that require millisecond-level latency analytics. Bigtable utilizes a wide-column data model with column families, allowing for flexible schema design. Row keys serve as efficient indexes for quick data access. Bigtable's high-throughput and low latency capabilities make it suitable for applications like time series data, IoT, financial data, and machine learning, especially when dealing with large datasets. In summary, Google Cloud provides various services for ETL processing. Dataprep is ideal for data wrangling tasks and offers a serverless option. Data Fusion excels at data integration, particularly in hybrid and multicloud environments, utilizing the open-source CDAP framework. Dataproc handles ETL workloads with support for Hadoop, Spark, and other open source tools, with Serverless Spark as a serverless option. Lastly, Dataflow, built on Apache Beam, is recommended for both batch and streaming ETL workloads, and provides a serverless architecture.

### Video - [Lab Intro: Creating a Streaming Data Pipeline for a Real-Time Dashboard with Dataflow](https://www.cloudskillsboost.google/course_templates/1157/video/521359)

* [YouTube: Lab Intro: Creating a Streaming Data Pipeline for a Real-Time Dashboard with Dataflow](https://www.youtube.com/watch?v=-LsNqUHi_e4)

In this lab, you create a streaming data pipeline for a real-time dashboard with Dataflow. You create a Dataflow job from a template. You then monitor a pipeline loading data into BigQuery. After that, you examine the data loaded using SQL. Finally, you visualize key metrics using Looker Studio.

### Lab - [Creating a Streaming Data Pipeline for a Real-Time Dashboard with Dataflow](https://www.cloudskillsboost.google/course_templates/1157/labs/521360)

Want to build streaming data pipelines that feed management dashboards? In this lab you will build a pipeline that streams large volumes of records into BigQuery for analysis and visualization.

* [ ] [Creating a Streaming Data Pipeline for a Real-Time Dashboard with Dataflow](../labs/Creating-a-Streaming-Data-Pipeline-for-a-Real-Time-Dashboard-with-Dataflow.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/1157/quizzes/521361)

## Automation Techniques

This module focuses on automation patterns and options for pipelines on Google Cloud. It covers various tools and services like Cloud Scheduler, Workflows, Cloud Composer, Cloud Run functions, and Eventarc, along with their functionalities and use cases for automation.

### Video - [Module Introduction](https://www.cloudskillsboost.google/course_templates/1157/video/521362)

* [YouTube: Module Introduction](https://www.youtube.com/watch?v=Ce_-rSH6xyA)

In this module, first, you review the automation patterns and options available for pipelines. Second, you explore Cloud Scheduler and workflows. Then, you review the functionality and use cases for Cloud Composer. Next, you review the capabilities of Cloud Run functions. Finally, you look at the functionality and automation use cases for Eventarc.

### Video - [Automation Patterns and Options for Pipelines](https://www.cloudskillsboost.google/course_templates/1157/video/521363)

* [YouTube: Automation Patterns and Options for Pipelines](https://www.youtube.com/watch?v=W-O-6DAc5g8)

On Google Cloud, ELT and ETL workloads can be automated for recurring execution. For example, in a scheduled ELT, a defined schedule triggers data extraction from BigQuery, transformation via Dataform, and loading back into BigQuery. Meanwhile, in the example shown for an event-driven ETL, a file upload to Cloud Storage initiates a batch process using Dataproc, culminating in data landing in Cloud Storage. Google Cloud offers a suite of services to automate and orchestrate your workloads. For scheduled tasks or one-off jobs, you can leverage Cloud Scheduler and Cloud Composer. If your workflows require orchestration, Cloud Composer is the ideal choice. To trigger actions based on events, consider using Cloud Run functions or Eventarc.

### Video - [Cloud Scheduler and Workflows](https://www.cloudskillsboost.google/course_templates/1157/video/521364)

* [YouTube: Cloud Scheduler and Workflows](https://www.youtube.com/watch?v=Njyn9dYqFpc)

Cloud Scheduler empowers you to automate tasks by invoking your workloads at specified recurring intervals. It grants you the flexibility to define both the frequency and precise time of day for job execution. Triggers can be based on HTTP/S calls, App Engine HTTP calls, Pub/Sub messages, or Workflows. Cloud Scheduler can be used to trigger a Dataform SQL workflow. In the example code, a scheduled job in Cloud Scheduler initiates the process defined in a YAML config file. The workflow involves two main steps: creating a compilation result from your Dataform code, and then triggering a workflow invocation using that result, ensuring only specific parts of your Dataform project execute based on included tags.

### Video - [Cloud Composer](https://www.cloudskillsboost.google/course_templates/1157/video/521365)

* [YouTube: Cloud Composer](https://www.youtube.com/watch?v=waH0q2AoYd4)

Cloud Composer acts as a central orchestrator, seamlessly integrating your pipelines across diverse systems, whether on Google Cloud, on-premises, or even multicloud environments. Cloud Composer leverages Apache Airflow, incorporating essential elements like operators, tasks, and dependencies to define and manage your workflows. Additionally, Cloud Composer offers robust features for triggering, monitoring, and logging, ensuring comprehensive control over your pipeline executions. Developing and executing workflows using Apache Airflow and Cloud Composer is easily done using Python. First, you leverage Apache Airflow operators to craft your directed acyclic graph, or DAG, defining the tasks and their dependencies. Next, the DAG is deployed to Cloud Composer, which handles the parsing and scheduling of your workflow. Cloud Composer further manages the execution of your tasks, incorporating features like error handling, retries, and monitoring to ensure smooth operation. With minimal effort, Cloud composer can be used to run a data analytics DAG. In the example code, the workflow retrieves a file from Cloud storage, loads it into BigQuery, and then performs a JOIN operation with an existing BigQuery table. The joined results are then inserted into a new BigQuery table. Finally, Dataproc is used for further data transformation.

### Video - [Cloud Run Functions](https://www.cloudskillsboost.google/course_templates/1157/video/521366)

* [YouTube: Cloud Run Functions](https://www.youtube.com/watch?v=ioQLEwX8mSQ)

Cloud Run functions allow you to execute code in response to various Google Cloud events. These events can originate from sources like HTTP requests, Pub/Sub messages, Cloud Storage changes, Firestore updates, or custom events through Eventarc. When triggered, a Cloud Run function provides a serverless execution environment where your code runs, supporting multiple programming languages for flexibility. Cloud Run functions easily automate routine tasks on Google Cloud. In the example code, a Dataproc workflow template is triggered after a file is uploaded to Cloud Storage. A Cloud Run function is used to capture the Cloud Storage new file event and call the Dataproc API. The Dataproc API then executes the specified workflow template, using the uploaded file as an input parameter. The final result of the workflow execution is stored in Cloud Storage.

### Video - [Eventarc](https://www.cloudskillsboost.google/course_templates/1157/video/521367)

* [YouTube: Eventarc](https://www.youtube.com/watch?v=ebJWjYst6G8)

Eventarc enables the creation of a unified event-driven architecture for loosely coupled services. Eventarc connects various event sources, including Google Cloud services, third-party systems, and custom events via Pub/Sub to a range of event targets like Cloud Run functions, and more. By using a standardized CloudEvent message format, Eventarc simplifies the integration of diverse systems and facilitates the development of responsive scalable applications. Eventarc enables deep monitoring of logging and other events which occur less frequently on Google Cloud. In the example code, Eventarc is used to trigger actions in response to data insertion events in BigQuery. When an insert operation occurs in a BigQuery table, it generates a Cloud Audit Log event. Eventarc can capture this event and initiate various actions such as rebuilding a dashboard, retraining an ML model, or executing any other custom action based on the specific requirements. In summary, there are various Google Cloud data-related automation options. Cloud Scheduler and Cloud Composer are suitable for scheduled or manual triggers, while Cloud Run functions and Eventarc are event-driven. Cloud Scheduler offers low coding effort with YAML, and Cloud Composer requires medium effort with Python. Cloud Run functions support multiple languages, while Eventarc is language agnostic. As a final note, all options except Cloud Composer are serverless.

### Video - [Lab Intro: Use Cloud Run Functions to Load BigQuery](https://www.cloudskillsboost.google/course_templates/1157/video/521368)

* [YouTube: Lab Intro: Use Cloud Run Functions to Load BigQuery](https://www.youtube.com/watch?v=1h34buDR7Fo)

In this lab, you create a Cloud Run function to load BigQuery. You create a Cloud Run function using the Cloud SDK. You then deploy and test the Cloud Run function. Finally, you view data in BigQuery and review Cloud Run function logs.

### Lab - [Use Cloud Run Functions to Load BigQuery](https://www.cloudskillsboost.google/course_templates/1157/labs/521369)

This hands-on lab shows you how to use Cloud Run functions to load data into BigQuery.

* [ ] [Use Cloud Run Functions to Load BigQuery](../labs/Use-Cloud-Run-Functions-to-Load-BigQuery.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/1157/quizzes/521370)

## Course Summary

In this final section, we review what was presented in this course and discuss the next steps to continue your cloud learning journey.

### Video - [Course Summary](https://www.cloudskillsboost.google/course_templates/1157/video/521371)

* [YouTube: Course Summary](https://www.youtube.com/watch?v=Sbc9YS9PD-A)

This concludes our course, Introduction to Data Engineering on Google Cloud. In this course, you learned about the duties and responsibilities of a data engineer, how to accomplish data engineering tasks, and core components used on Google Cloud to accomplish those tasks. How to create and deploy data pipelines of varying patterns on Google Cloud, and how to identify and utilize various automation techniques on Google Cloud to complete data engineering tasks. We hope you had a great learning experience.

### Document - [Course Resources](https://www.cloudskillsboost.google/course_templates/1157/documents/521372)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
