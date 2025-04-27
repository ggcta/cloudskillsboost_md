---
id: 578
name: 'Introduction to Data Analytics on Google Cloud'
datePublished: 2025-02-26
topics:
- Business Intelligence
- Data Storage
- Looker
type: Course
url: https://www.cloudskillsboost.google/course_templates/578
---

# [Introduction to Data Analytics on Google Cloud](https://www.cloudskillsboost.google/course_templates/578)

**Description:**

In this beginner-level course, you will learn about the Data Analytics workflow on Google Cloud and the tools you can use to explore, analyze, and visualize data and share your findings with stakeholders. Using a case study along with hands-on labs, lectures, and quizzes/demos, the course will demonstrate how to go from raw datasets to clean data to impactful visualizations and dashboards. Whether you already work with data and want to learn how to be successful on Google Cloud, or you're looking to progress in your career, this course will help you get started. Almost anyone who performs or uses data analysis in their work can benefit from this course.

**Objectives:**

- Describe the data analytics workflow on Google Cloud and summarize the different types of analytics.
- Identify Google Cloud data analytics products and describe how each is used to work with data.
- Describe data sources, data structures, and data storage options in Google Cloud.
- Use BigQuery, Looker, and Looker Studio to answer data questions and influence business decisions.

## Course Introduction

This section welcomes learners to the Introduction to Data Analytics on Google Cloud course. In addition, this section introduces learners to the topics, concepts, and objectives of the course. 

### Video - [Course introduction](https://www.cloudskillsboost.google/course_templates/578/video/526275)

- [YouTube: Course introduction](https://www.youtube.com/watch?v=kTWOpIIXnUE)



## Understand the Data Analytics Lifecycle on Google Cloud

 In this module, you receive a high-level introduction to a typical Google Cloud data analytics workflow, including what data sources and storage options are available, and examples of what types of data are best suited for data analysis versus machine learning training data.

### Video - [Understand the data analytics lifecycle on Google Cloud: Introduction](https://www.cloudskillsboost.google/course_templates/578/video/526276)

- [YouTube: Understand the data analytics lifecycle on Google Cloud: Introduction](https://www.youtube.com/watch?v=NDqEkvf2ulI)

This module of the Introduction to Data Analytics on Google Cloud course examines the Google Cloud data analytics workflow and describes Google Cloud data sources and storage methods. Capturing managing, and using data is central to redefining customer experiences and creating new value. To analyze and gain insight from your data, it’s imperative that you understand the data analytics lifecycle on Google Cloud. The data analytics lifecycle provides a framework for organizing the different steps involved in data analytics. This framework can help to ensure that the necessary steps are taken, and that they are taken in the correct order. Storing, managing, and organizing your data is the foundation for data analytics on Google Cloud. In this section, you learn to: Detail and describe a data analytics workflow on Google Cloud. Compare and contrast data sources and storage methods available in Google Cloud. And compare how different data types can be used for data analytics versus machine learning.

### Video - [Introducing a Google Cloud data analytics workflow](https://www.cloudskillsboost.google/course_templates/578/video/526277)

- [YouTube: Introducing a Google Cloud data analytics workflow](https://www.youtube.com/watch?v=ATbzzaERX9o)

Data is an essential ingredient for driving innovation and differentiation, and is the key to unlocking value from artificial intelligence. Data comes from various different sources and inputs, including operational systems, web sources, social media, and Internet of Things, or IoT. Data can also be structured or unstructured. To generate insights, you need to combine and make sense of different types of data, regardless of the state it’s in or how it was created. Google Cloud provides serverless, comprehensive, and integrated solutions for each step of the data analytics lifecycle. The data analytics lifecycle is the process of collecting, storing, processing, and analyzing data to extract insights. It’s a critical part of any business that wants to make informed decisions based on data. The data analytics lifecycle is an iterative process. You will often go back and forth between different steps as you learn more about your data and what you want to achieve with it. Let’s explore the steps of the data analytics lifecycle. The first step is to ingest data into the cloud. During this step, Google Cloud ingestion and processing tools help break down data silos and increase time to insight. Products such as Pub/Sub, Dataflow, Dataproc, and Cloud Data Fusion are used to ingest and process both real-time and batch data. Cloud Data Fusion is a fully managed, cloud first, data integration service. This code-free, extract, transform, and load–or ETL–tool integrates data across on-premises and cloud sources. Pub/Sub and Dataflow are streaming analytics services. Pub/Sub is for ingestion and messaging, And Dataflow is for analytics and processing. After data is ingested, it needs to be processed. Dataproc can be used to batch process data, Dataflow to stream data, or Cloud Data Fusion to integrate data from multiple sources. Once data has been ingested and processed, the next step is to store the data securely. Storage solutions also need to scale with your data. Google Cloud storage options include databases, data lakes, and data warehouses. Google Cloud storage products include: Cloud Storage, Cloud SQL, Cloud Spanner, Bigtable, Firestore, AlloyDB for PostgreSQL, and BigQuery. Cloud SQL, Cloud Spanner, and AlloyDB for PostgreSQL are relational databases, whereas Bigtable and Firestore are NoSQL databases. BigQuery is Google Cloud’s data warehouse solution. After your data has been ingested, processed, and stored, it can be analyzed. This course focuses on the analyze stage of the data analytics lifecycle. BigQuery is at the core of data analytics on Google Cloud. BigQuery is an elastic, flexible, secure, and reliable data warehouse that works across clouds and scales with your data. This fully managed data warehouse can be used to analyze data through SQL commands. BigQuery is deeply integrated with Google Cloud’s analytical and data processing services, which lets you build a cloud-first data warehouse. In addition to BigQuery, you can analyze data and visualize results by using Looker And Looker Studio. You explore BigQuery, Looker, and Looker Studio in this course. Data is also the key to unlocking the value of machine learning on Google Cloud. The primary product of the machine learning development platform is Vertex AI, which includes: AutoML, Vertex AI Workbench, and TensorFlow. These products unlock insights that only large amounts of data can provide. Knowledge of the data analytics lifecycle will help you identify the right data, prepare it for analysis, and extract insights from it.

### Video - [Google Cloud data sources and storage methods](https://www.cloudskillsboost.google/course_templates/578/video/526278)

- [YouTube: Google Cloud data sources and storage methods](https://www.youtube.com/watch?v=U2YlP_8-qoE)

Before learning about the analysis stage, it’s important to understand the various storage solutions Google Cloud offers. Every application needs to store data, and different applications and workloads require different storage solutions. This section focuses on the storage step of the data analytics lifecycle. Google Cloud offers several core storage products. This list includes: Cloud Storage, Cloud SQL, Cloud Spanner, BigQuery, Firestore, Cloud Bigtable, and AlloyDB for PostgreSQL. Depending on your use case, you might use one or several of these services to do the job. Before getting into the details of each of these storage options, let’s differentiate between data sources. Data sources are connectors that let you query data from various sources. You can use data sources to create datasets, which are collections of data that can be used for analysis and machine learning. Google Cloud data sources can be classified into two categories: Cloud data sources are data sources that are stored on Google Cloud. For example, you can connect to a Cloud Storage bucket or a Cloud SQL database. External data sources can be stored on-premises or in another cloud provider. For example, you can connect to an Amazon S3 bucket or a Microsoft SQL Server database. You can create a data source connection by using the Google Cloud console, the Cloud SDK, or the Google Cloud API. What are some benefits of using Google Cloud data sources? First, Google Cloud data sources give centralized access to your data, which makes it easier to find and analyze data, regardless of where it’s stored. Google Cloud data sources also help you integrate data from different sources. This integration can be helpful for building data warehouses and data lakes. We discuss these storage options in this course. They can also be used to analyze your data, so you can identify trends, make predictions, and make better business decisions. Finally, in general, data sources can be used to visualize your data, to help you communicate your findings to others and make your data more actionable. Now that you know what data sources are and the benefits of using Google Cloud data sources, let’s explore storage options. The list of storage options includes databases, data warehouses, and data lakes. A database is an organized collection of data stored in tables and accessed electronically from a computer system. and accessed electronically from a computer system. Google Cloud offers relational and non-relational database options. Relational databases, such as Cloud SQL, Cloud Spanner, and AlloyDB for PostgreSQL store and provide access to data points that are related to one another. A relational database can establish links–or relationships–between information by joining tables, and structured query language, or SQL, can be used to query and manipulate data. This type of database is highly consistent, reliable, and best suited for dealing with large amounts of structured data. A non-relational database, sometimes known as a NoSQL database, is less structured in format and doesn’t use a tabular format of rows and columns like relational databases. Non-relational databases follow a flexible data model, which makes them ideal for storing data that changes its organization frequently or for applications that handle diverse types of data. Bigtable is a non-relational database product. While a database is designed to capture data for storage, retrieval, and use, a data warehouse is designed to analyze data. A data warehouse is an enterprise system used for the analysis and reporting of structured and semi-structured data from multiple sources. BigQuery is Google Cloud's data warehouse offering. This course focuses on analyzing data in BigQuery and visualizing it with Looker and Looker Studio. A data lake is a repository designed to ingest, store, explore, process, and analyze any type or volume of raw data, regardless of the source. It can store different types of data in its original format; ignoring size limits, and without much pre-processing or adding structure. Data lakes often consist of many different products, depending on the nature of the data that is ingested. Data warehouses and data lakes should be considered complementary instead of competing tools. Although both store data in some capacity, each is optimized for different uses. Different data types have different purposes and uses. Structured data, which is data that has been organized into rows and columns, is best fit for data analytics. This type of data is well-suited for statistical analysis and other techniques used in data analytics. Machine learning can use both structured and unstructured data. Unstructured data is data that does not fit neatly into a table or spreadsheet. This type of data can be text, images, or audio. Machine learning algorithms can learn from unstructured data to identify patterns and make predictions.

### Quiz - [Quiz: Understand the data analytics lifecycle on Google Cloud](https://www.cloudskillsboost.google/course_templates/578/quizzes/526279)

#### Quiz 1.

> [!important]
> **Which Google Cloud product is a relational database used to establish relationships between information in multiple datatables?**
>
> - [ ] Cloud Spanner
> - [ ] BigQuery
> - [ ] BigTable
> - [ ] Dataproc

#### Quiz 2.

> [!important]
> **Data sources are connectors that let you do what with your data?**
>
> - [ ] Ingest and process the data.
> - [ ] Query the data.
> - [ ] Store the data.
> - [ ] Clean the data.

#### Quiz 3.

> [!important]
> **What type of data is used for machine learning?**
>
> - [ ] Structured data only
> - [ ] Relational data
> - [ ] Raw data
> - [ ] Structured and unstructured data

#### Quiz 4.

> [!important]
> **Select the correct steps in the data analytics lifecycle.**
>
> - [ ] Visualize results and share the data.
> - [ ] Visualize, process, and ingest.
> - [ ] Ingest, process, store, analyze, and activate.
> - [ ] Activate, store, and analyze.

#### Quiz 5.

> [!important]
> **Which product is a serverless data warehouse for storage and analytics?**
>
> - [ ] Looker
> - [ ] Cloud Storage
> - [ ] Cloud Spanner
> - [ ] BigQuery

### Video - [Understand the data analytics lifecycle on Google Cloud: Summary](https://www.cloudskillsboost.google/course_templates/578/video/526280)

- [YouTube: Understand the data analytics lifecycle on Google Cloud: Summary](https://www.youtube.com/watch?v=-Ik9Cn4Wx80)

This brings us to the end of this section on the data analytics lifecycle. Let’s take a moment to review what was covered. This section began with an introduction to the data analytics lifecycle, including which Google Cloud products and services are best suited for each step. The next section covered storage methods, data sources, and data types for analytics on Google Cloud. You learned which storage solutions are best for your use cases, and how data can be used for analytics versus machine learning. In the next module of this course, you learn more about finding data and using basic SQL commands in BigQuery to extract insight.

## Explore Data and Extract Insights by Using BigQuery

In this module, you receive a high-level introduction to BigQuery and its solution architecture, and use common SQL commands to locate specific data in BigQuery to answer a data-driven question.

### Video - [Explore data and extract insights using BigQuery: Introduction](https://www.cloudskillsboost.google/course_templates/578/video/526281)

- [YouTube: Explore data and extract insights using BigQuery: Introduction](https://www.youtube.com/watch?v=aNmdGEdO84E)



### Video - [Introduction to BigQuery for data analysts](https://www.cloudskillsboost.google/course_templates/578/video/526282)

- [YouTube: Introduction to BigQuery for data analysts](https://www.youtube.com/watch?v=ALS3-w-gPzQ)

Let’s begin with an introduction to BigQuery for data analysts. In this section, we introduce BigQuery, Google’s data warehouse solution, and discuss its features and uses, and conclude with a demo. What do we mean when we say BigQuery is a fully managed data warehouse? It means that BigQuery takes care of the underlying infrastructure, so you can focus on using SQL queries to answer business questions without worrying about deployment, scalability, and security. At this point, it’s useful to consider what the main difference is between a data warehouse and a data lake. A data lake is just a pool of raw, unorganized, and unclassified data, which has no specified purpose. On the other hand, a data warehouse contains structured and organized data, which can be used for advanced querying. As a data warehouse, BigQuery can store transformed data for business insights. Data sources feed into a data lake and are processed into your data warehouse for analysis and reporting. Of course, the purpose of BigQuery is not to just save data; it’s for analyzing data and helping to make business decisions. BigQuery is optimized for running analytic queries over large datasets. It can perform queries on terabytes of data in seconds and petabytes in minutes. This performance lets you analyze large datasets efficiently and get insights in near real time. To give you an idea of the scale of data BigQuery can work with: One Google Cloud customer has over 350 PB of data stored in BigQuery. Other customers have run queries on over 10 trillion rows and concurrent queries running on over 100 trillion rows over multiple customers. And another customer has run 10,000 concurrent queries at the same time. So what does a typical data warehouse solution architecture look like? BigQuery is the analytics engine that sits at the end of the data pipeline. It stores incoming data and then lets you do your analysis and model building. BigQuery is actually two services in one: it’s both a fast SQL query engine and also a fully managed storage layer for loading and storing your datasets. BigQuery maximizes flexibility by separating the compute resources that analyze your data from your storage choices. You can store and analyze your data within BigQuery or use BigQuery to assess your data where it lives. Federated queries let you read data from external sources while streaming supports continuous data updates. Powerful tools like BigQuery ML and BI Engine let you analyze and understand that data. Let’s look at some of the key features of BigQuery. First, BigQuery provides two services in one. It’s a place to store and analyze petabytes of data, with built-in features like machine learning, geospatial analysis, and business intelligence. BigQuery is a fully managed serverless solution, which means that you don’t need to worry about provisioning any resources or managing servers in the backend but only focus on using SQL queries to answer your organization's questions in the frontend. If you’ve never written SQL before, don’t worry. This course provides resources and labs to help. BigQuery has a flexible on-demand pricing model where you pay for the number of bytes of data your query processes and for any permanent table storage. If you prefer to have a fixed bill every month, you can also subscribe to capacity compute pricing where you have a reserved amount of resources for use. Data in BigQuery is encrypted at rest by default without any action required from a customer. By encryption at rest, we mean encryption used to protect data that is stored on a disk, including solid-state drives, or backup media. And finally, BigQuery has built-in machine learning features so you can write ML models directly in BigQuery using SQL. Also, if you decide to use other professional tools—such as Vertex AI from Google Cloud—to train your ML models, you can export datasets from BigQuery directly into Vertex AI for a seamless integration across the data-to-AI lifecycle. Now it’s time to login to the BigQuery user interface, to demonstrate how you can query Terabytes of data in seconds. First things first, let's open BigQuery, which can be found in the navigation menu. Now this is what the BigQuery user interface looks like. Every resource in Google Cloud exists inside a project, which you can view here. In addition to security and access control, a project is what links usage of a resource to a credit card: it makes a resource billable. BigQuery has numerous public datasets that anyone can query. One of these is all public Wikipedia page metadata. Next, let’s simply paste and run a SQL query to see how fast BigQuery can scan and process 10 billion rows looking for the word “Google” in the Wikipedia page title. BigQuery's scalable, distributed analysis engine lets you query terabytes in seconds and petabytes in minutes. The query includes filtering, grouping, and ordering on a dataset that contains 10 billion records and runs quickly and efficiently in BigQuery. In BigQuery, data is stored inside datasets. Datasets contain tables, and tables contain columns. Access to data in BigQuery is controlled at many levels, from the project and dataset to the individual table, column, and row. A BigQuery slot is a virtual CPU used by BigQuery to execute SQL queries. BigQuery automatically calculates how many slots each query requires, depending on query size and complexity. You don't need to provision resources before using BigQuery, unlike many relational database management systems. BigQuery allocates storage and query resources dynamically based on your usage patterns. Storage resources are allocated as you consume them and deallocated as you remove data or drop tables. Query resources are allocated according to query type and complexity. Each query uses some number of slots, which are units of computation that comprise a certain amount of CPU and RAM. There is no minimum usage commitment. The service allocates and charges for resources based on your actual usage. By default, all BigQuery customers have access to 2,000 slots for query operations. You can also reserve a fixed number of slots for your project.

### Video - [Derive insight from data with BigQuery](https://www.cloudskillsboost.google/course_templates/578/video/526283)

- [YouTube: Derive insight from data with BigQuery](https://www.youtube.com/watch?v=r0PdbCGm9oU)

This section is a bit more technical and explores how BigQuery works. Let’s begin by discussing how BigQuery’s two services, analytics and storage, work together to power your data-driven innovation. Google's high speed internal network connects the two services. This super fast network is what enables us to separate compute and storage. So what does each service do? The short answer is that the services are fully-managed so users like you and me don’t have to worry about how BigQuery stores data on disk or autoscales machines for big queries. That said, it’s a great learning exercise to understand how the services perform their magic so we can better understand what is happening. First up is the BigQuery storage service. The storage service automatically manages the data that you ingest into the platform. BigQuery organizes data tables into units called datasets. These datasets are scoped to your Google Cloud project. When you reference a table from the command line in SQL queries or in code, you refer to it by using the construct: project.dataset.table. The tables are stored as highly compressed columns in Google’s Colossus file system which provides durability and availability. The storage service supports bulk data ingest and streaming ingest. So it can work with huge amounts of data and also real-time data streams. The query service runs interactive or batch queries that are submitted through console, the BigQuery web UI, the bq command line tool, or REST API. The REST API is supported for seven programming languages. Recall, in the demo earlier, we used the BigQuery web UI to submit the query. There are connectors to other services such as Dataproc, which simplify creating complex workflows between BigQuery and other Google Cloud data processing services. The query service can also run query jobs on data contained in other locations, such as tables in CSV files hosted in Cloud Storage or data in Google Sheets. Before you get too excited about running queries on your data in Google Sheets, you should know that BigQuery is most efficient when working with data contained in its own storage service. The storage service and the query service work together to internally organize the data and make queries efficient over huge datasets of Petabytes in size. They even optimize your query processing job after you submit it. One of the most important controls you have over resource consumption and costs is controlling the amount of data processed. In general, you only want to select the columns of data you actually want to process and return. A best practice is to start broad when you’re exploring the dataset and then focus on those critical fields and rows that you need. Exploring your dataset with SQL is your first step in uncovering hidden insights. Let’s briefly go back to the BigQuery user interface and view another example. Here we’re running a query to count the total number of trips taken on the public dataset for San Francisco bike share trips. There is often uncertainty around the quality of the data in your dataset, so you can use SQL to explore and filter for anomalies. Here we filtered customer records that didn’t contain a birth date by setting member_birth_year IS NOT NULL as a filter. We also applied the group by clause to group the results by the starting station name. The order by clause helps with sorting the results, while the limit only shows the top 5 results.

### Video - [Lab introduction: BigQuery: Qwik Start - Console](https://www.cloudskillsboost.google/course_templates/578/video/526284)

- [YouTube: Lab introduction: BigQuery: Qwik Start - Console](https://www.youtube.com/watch?v=9r7uaygWB2o)

It’s time for you to get hands-on practice with BigQuery, by participating in a lab. In the lab that follows this video, you become familiar with the BigQuery user interface and query a public dataset. In this lab, you learn to: Query a public data set, create a new dataset, load data into a new table, and query a custom table. Let’s practice what you learned.

### Lab - [BigQuery: Qwik Start - Console](https://www.cloudskillsboost.google/course_templates/578/labs/526285)

This lab shows you how to query public tables and load sample data into BigQuery using the Web UI. Watch the short videos <A HREF="https://youtu.be/rwZsPjCTkhw">Get Meaningful Insights with Google BigQuery</A> and <A HREF="https://youtu.be/dOpNxH64JIU">BigQuery: Qwik Start - Qwiklabs Preview</A>.

- [ ] [BigQuery: Qwik Start - Console](../labs/BigQuery-Qwik-Start-Console.md)

### Video - [BigQuery organizes data to make analytics easier](https://www.cloudskillsboost.google/course_templates/578/video/526286)

- [YouTube: BigQuery organizes data to make analytics easier](https://www.youtube.com/watch?v=uzYdt7-Y6HI)

In addition to fast query execution times, recall that BigQuery also manages the storage and metadata for your datasets. Let’s discuss how BigQuery organizes data to make exploration and analytics easier. What are some reasons to structure your information into datasets, projects, and tables? These multiple scopes—project, dataset, and table—can help you structure your information logically. You can use multiple datasets to separate tables pertaining to different analytical domains, and you can use project-level scoping to isolate datasets from each other according to your business needs. You can align projects to billing and use datasets for access control. You store data in separate tables based on logical schema considerations. Every table has a schema. You can enter the schema manually through the Google Cloud console or by supplying a JSON file. File formats like Avro, Parquet, ORC, Firestore export, or Datastore export are self-describing, so BigQuery automatically infers the table schema from the source data. BigQuery is called a "columnar store," which means that it is designed for processing columns, not rows. Because BigQuery only reads the relevant columns to execute a query, it is optimized for the high reads of data warehouses. Since each column has data of the same type, BigQuery can compress the column data much more effectively. Each column is automatically compressed, encrypted, and replicated to support availability and durability of data in BigQuery. BigQuery stores data in a massively distributed format. This is the same for Google Cloud Storage and is what powers apps like Gmail, Ads, and many more Google products. BigQuery auto-optimizes the balancing and partitioning of these data shards in the back end. Alternatively, you can also partition and cluster your tables based on your access patterns to control costs and make your queries more performant. Let’s once again demonstrate how to use SQL in BigQuery to analyze data. Following this demo, you’ll get hands-on experience with a lab. The first thing we’ll do is add some data. Let’s click Add Data and then select Public Datasets. And in this case we want to analyze New York Citi bike trip data, so let’s search for that data set and then click View Dataset. In the BigQuery console, you see two projects in the left pane, one named your Qwiklabs project ID, and one named bigquery-public-data. Let’s scroll down and find our table. And then we’ll select the table and then the Preview tab to examine the columns and data. Next, let’s run a new query. This query will tell us the typical duration for the 10 most common one-way rentals. Let’s run one more query, this time to find the total distance traveled by each bicycle in the dataset. Note that in this case we are pulling data from a couple different datatables (citybike_trips and citibike_stations) and joining the tables together to get the intended results.

### Quiz - [Quiz: Explore data and extract insights using BigQuery ](https://www.cloudskillsboost.google/course_templates/578/quizzes/526287)

#### Quiz 1.

> [!important]
> **BigQuery is two services in one. What are the two services?**
>
> - [ ] Warehouse and database services
> - [ ] Relational and non-relational services
> - [ ] Reporting and sharing services
> - [ ] Storage and query services

#### Quiz 2.

> [!important]
> **BigQuery is optimized for reading terabytes and petabytes of data. How can BigQuery read and handle large amounts of data?**
>
> - [ ] BigQuery is optimized to read rows of data, which are easier to process than columns.
> - [ ] BigQuery's storage and analytics services operate independently.
> - [ ] BigQuery is a "columnar store," so it only reads the relevant columns to execute a query.
> - [ ] BigQuery condenses data so that it can be read on the first pass.

#### Quiz 3.

> [!important]
> **What construct is used to reference a data table in a SQL query?**
>
> - [ ] project.dataset.table
> - [ ] dataset.table.row
> - [ ] dataset.table.column
> - [ ] table.dataset

#### Quiz 4.

> [!important]
> **BigQuery is most efficient when working with data contained where?**
>
> - [ ] Its own storage service
> - [ ] Google Sheets
> - [ ] Cloud Storage
> - [ ] Bigtable

#### Quiz 5.

> [!important]
> **BigQuery is a fully managed data warehouse. What is a benefit of a data warehouse being fully managed?**
>
> - [ ] Data management is handled by Google Cloud.
> - [ ] BigQuery takes care of the underlying infrastructure.
> - [ ] Google Cloud handles the analyze step of the data analytics lifecycle.
> - [ ] BigQuery processes data faster than it would if it were not fully managed.

### Video - [Explore data and extract insights using BigQuery: Summary](https://www.cloudskillsboost.google/course_templates/578/video/526288)

- [YouTube: Explore data and extract insights using BigQuery: Summary](https://www.youtube.com/watch?v=jLoFfdCphDQ)

You’ve reached the end of this module on BigQuery, Google’s fully managed enterprise data warehouse for analytics and storage. Let’s briefly recap what you learned. First, you got an introduction to BigQuery, including a brief demo of the platform. Next, you learned how to derive insights from your data with BigQuery, including accessing the data you need, and running basic queries. Finally, you learned more about BigQuery storage and organization. Along the way, you viewed demos and participated in a few labs. In the next section, you learn about Looker, Google Cloud’s data analytics and visualization tool.

## Make Data-driven Decisions by Using Looker

 In this module you learn the fundamentals of data exploration and visualization in Looker. In addition, you learn how to share data from Looker and Looker Studio. 

### Video - [Make data-driven decisions using Looker: Introduction](https://www.cloudskillsboost.google/course_templates/578/video/526289)

- [YouTube: Make data-driven decisions using Looker: Introduction](https://www.youtube.com/watch?v=WNgmeAqfgFQ)

Welcome to this section on Looker, where you learn the fundamentals of analyzing, visualizing, and sharing data by using the Looker platform. With Looker, you can activate and use the data you’ve analyzed to empower your teams to make effective, data-driven decisions. So, what’s Looker? Looker is a powerful tool that helps you: Access and review the data that your company collects. Answer data questions in real-time. Stay up-to-date with the status of your business. And use data to drive decision making. Let’s examine the common data analysis process in Looker. First, identify the data questions you want to answer. Perhaps you’re an analyst for an ecommerce retailer. Some standard questions include: How many sales were made last week? What’s your user or customer demographics? What is the shipment status of all orders? The next step is to identify the data required to answer your questions. Referring to our previous ecommerce example, if you want to determine the shipment status of all orders, you need data on orders, shipments, and perhaps additional info such as distribution center data. If you’re analyzing your users, you might want data on where those users are coming from, such as traffic source and location. Next, it’s time to analyze the data. In Looker, data analysis is referred to as “exploring.” After you identify your data questions and the data that you need, you're ready to combine dimensions and measures in Looker to find the answers. You learn more about dimensions and measures in this course. Finally, interpret the results. After you analyze and visualize the data, you can gain insight, act, and make data-driven decisions. Referring to the ecommerce example, perhaps you discovered that a large percentage of your customers were directed to your website from a recent campaign designed by your marketing team. By using data to show the success of the campaign, you can advocate for more similar campaigns in the future to increase sales. In this section you learn to: Manipulate a Looker Explore to answer data-driven questions. Create a situation-appropriate visualization to highlight the answer for a data-driven question. And share visualizations with others. Let’s get started!

### Video - [Use Looker to analyze and chart data](https://www.cloudskillsboost.google/course_templates/578/video/526290)

- [YouTube: Use Looker to analyze and chart data](https://www.youtube.com/watch?v=J-8nyoT6HnY)

Let’s begin by viewing the Looker interface, and detailing the main components used for data exploration. In Looker, an Explore is a report-builder interface, and a portal to ask questions by using your data. Explores are curated by Looker developers in a proprietary templating language called LookML. The Explores that you were given access to are listed in the Explore section. This Explore example contains ecommerce data. The left side panel displays the field picker, where fields are bundled into groups called views. The two primary fields for exploring data in Looker are dimensions and measures. Dimensions are attributes or characteristics of your data. Each column in a database table is a dimension in Looker. For example, this database table displays data for orders. Each column in the table displays an attribute for the order, such as the date the order was placed, the sale price, and the shipping status. In Looker, all of these columns are dimensions. Measures are calculations performed across multiple rows of data. As such, measures are aggregates of data attributes, or dimensions. Perhaps you want to learn how many orders were placed last week. Anytime you have a question like “how many,” you probably want to look for a measure with the word count or number in it (in this case, count). To find the answer to this data question, you must first group the data by dimension–in this case, the order date–and then add a count measure. You often need to combine dimensions and measures to answer your data questions. These dimensions and measures can also span across multiple views. Let’s look at another example, this time analyzing user data. Notice that the dimensions in the field picker are listed alphabetically, and some dimensions are grouped, like Created Date. Use the search function to quickly find the dimension you’re looking for. In this example, the goal is to identify which cities have the most users, so start by adding the city dimension and then the count measure to see how many users are in each city. Set a row limit to 10 to see the top 10 cities. After all is set, click Run to display the top 10 cities based on the number of users. Let’s go a step further and adjust the visualization. There are various different visualization options to choose from. In this example, it probably makes sense to display the visualization as a column chart. You can also add labels to the side of each bar to see the total bar value. Click Edit, and turn on Value Labels in the Values tab. Each column in the chart now has its value displayed. Now, the column chart showing the top 10 cities with the most users is complete. Next, let’s filter the results. Filters narrow the results returned based on specific criteria, so you can focus on a subset of your data based on desired characteristics. A key feature of filters is that they don’t delete anything from the database; they’re only applied to the data that Looker displays on your screen. You can filter both dimensions and measures. The following example demonstrates how to filter on a dimension. Perhaps the results of our previous query–displaying cities across the United States–is too broad, and instead you want to narrow the results to only show cities in the state of California. You can narrow the results by adding a filter for the state of California. After you rerun the query, The results are filtered to display just the top 10 cities in California. The final exploring technique covered in this section is pivoting. Pivots let you turn a selected dimension into several columns, which creates a matrix of your data. Perhaps in addition to the city dimension, you want to add the age tier dimension to group your users by age. After the query is run, the table doesn’t show the intended results. For example Los Angeles appears on multiple rows, and only four of the top 10 cities are displayed. This is where a pivot can be useful. Pivoting the table by the Age Tier dimension brings the age tier to the top of the table, and now all age tiers and cities are visible. When you pivot on a dimension, each unique possible value of that dimension becomes its own column header. Any measures are then repeated under each column header. After you pivot the results, you can easily compare results by different groupings and identify potential gaps, all while leaving your underlying data unaffected. Let’s go back to the Looker user interface and use another example to demonstrate how pivots work. In the Order Items Explore, the Total Sale Price measure is added. Next, the Product Category and Department dimensions are added to group the results by these characteristics. After the query is run, the two departments appear on multiple rows. This table can be made more useful and easier to read by adding a pivot. Pivoting on the department dimension brings department to the top of the table, so when you rerun the query, each department is displayed in a single column. If you notice some interesting insights or trends in your data, you can save your findings to a dashboard or as a Look. A Look is a single, saved report or visualization. Looks typically answer an individual data question, and they can be added to a dashboard. A dashboard is a series of saved reports, all on one page. A dashboard presents the answers to multiple data questions, and is often where data explorers store their data findings. Explores, Looks, and dashboards can all be shared with others. You learn more about data sharing in this course.

### Video - [Lab introduction: Looker Data Explorer - Qwik Start](https://www.cloudskillsboost.google/course_templates/578/video/526291)

- [YouTube: Lab introduction: Looker Data Explorer - Qwik Start](https://www.youtube.com/watch?v=BqEkBRc6Y60)

It’s time for another lab! In previous lessons, we discussed how to use dimensions, measures, filters, and pivots to find the answers to data-driven questions. Now, let’s put what you learned to practice, and use the Looker interface to explore data. In this lab, you: Use the Explore interface to access data published by LookML developers. Work with Dimensions and Measures to query and select data. Select the appropriate visualization type to best display your data. And Save an Explore query to a dashboard. Let’s get started.

### Lab - [Looker Data Explorer - Qwik Start](https://www.cloudskillsboost.google/course_templates/578/labs/526292)

In this lab, you will create a series of visualizations from the Airports and Flights datasets and save them to a dashboard in Looker.

- [ ] [Looker Data Explorer - Qwik Start](../labs/Looker-Data-Explorer-Qwik-Start.md)

### Video - [Visualize data using Looker studio](https://www.cloudskillsboost.google/course_templates/578/video/526293)

- [YouTube: Visualize data using Looker studio](https://www.youtube.com/watch?v=Io-dMOKJeHk)

In addition to Looker, you can use Looker Studio to visualize your data. Looker provides powerful analytics tools for analyzing data and creating reports. Looker Studio features less analytics functionality and focuses more on a simple, easy to use interface for data visualization. Looker Studio offers several features that make it easy to share and collaborate on reports. You can publish reports to the web, and you can also embed reports in other applications. The benefits of using Looker Studio for data visualizations include: A drag-and-drop interface that makes it easy to create reports and dashboards. Various reports and dashboards, including charts, graphs, and tables. Powerful features that let you create professional-looking reports, such as the ability to add filters and drill down into data. Real-time collaboration on reports and dashboards. And security features that let you control who has access to your data. Looker and Looker Studio can be integrated using the Looker connector for Looker Studio. This integration lets you connect to any Google Cloud-hosted Looker instance and create reports and dashboards by using Looker data. The Looker connector is just one of many different connectors available in Looker Studio. To use the Looker connector, you must first enable the integration in your Looker instance. After the integration is enabled, you can create a new report in Looker Studio and select the Looker connector as your data source. You’re then prompted to enter the URL of your Looker instance and to select an Explore. Once you have selected an Explore, you can start creating your report by using Looker data. To create a situation-appropriate visualization in a report in Looker Studio, you need to consider the following: First, what type of data are you working with? Second, what insights are you trying to communicate? What you’re trying to communicate will influence the type of visualization option you choose. And finally, who is the audience you are creating the report for? The audience may influence how you style and organize your report. Next, let’s examine the most common visualization options in Looker Studio. Bar charts are a great way to compare data across different categories. Line charts are a great way to show how data changes over time. Area charts are similar to line charts, but the area below the line is filled in. Pie charts are useful to show the relative proportions of different categories. Donut charts are similar to pie charts, but they leave a hole in the center. Scatterplots are a great way to show the relationship between two variables. Heatmaps are used to show the distribution of data. And lastly, maps show data that is geographically located. In addition, you can also create custom visualizations with Looker Studio. Let’s demonstrate how to create a simple chart in Looker Studio by using Looker data. In this example, Looker has already been connected as the data source by using the Looker connector. A report in Looker Studio is the same as a dashboard in Looker, and consists of one or several charts. Charts are ways to visualize dimensions and metrics. You can create a chart in Looker Studio by clicking Add a chart in the toolbar, and then selecting the type of chart you want to use. Let’s assume you work at an Ecommerce store, and you want to visualize the count of orders for each category over the past year. A line chart or an area chart would be a great visualization for this type of data. After you select your desired chart, it’s added to the report. Next, customize the data, much like you would in Looker, by adding dimensions for the order created date and product category. Created date is a date range, so it’s added as the date range dimension. And the data will be broken down by the product category, so specify Products category as the breakdown dimension. The chart currently displays all order data from the past few years. To limit the results–in this case, to the past year–add a filter. And now the chart displays the count of orders by date, broken down by category, over the past year. Finally, under the style tab, you can customize the different components of the chart, such as labels, colors, and fonts, or you can switch to a different visualization altogether.

### Video - [Lab introduction: Looker Studio: Qwik Start](https://www.cloudskillsboost.google/course_templates/578/video/526294)

- [YouTube: Lab introduction: Looker Studio: Qwik Start](https://www.youtube.com/watch?v=BJOtWMbPIrk)

You’ve made it to the second lab in this section. In this Lab, you use Looker Studio to visualize query results, and create compelling reports and dashboards. In this lab, you: Create a report by pulling in a public dataset from BigQuery, and add a chart and style a report. Let’s get started.

### Lab - [Looker Studio: Qwik Start](https://www.cloudskillsboost.google/course_templates/578/labs/526295)

Data Studio lets you create dynamic, visually compelling reports and dashboards. Watch the short video <A HREF="https://youtu.be/eSY6daAlk5k">Data Studio: Qwik Start - Qwiklabs Preview</A>.

- [ ] [Looker Studio: Qwik Start](../labs/Looker-Studio-Qwik-Start.md)

### Video - [Share reports and visualizations](https://www.cloudskillsboost.google/course_templates/578/video/526296)

- [YouTube: Share reports and visualizations](https://www.youtube.com/watch?v=yGvHqx9g0j4)

The value of Looker and Looker Studio does not end with data analysis and visualization. Sharing reports and dashboards with others improves collaboration, enables data-driven decision-making, and increases transparency. Data can be shared from both Looker and Looker Studio. In this lesson, you learn the benefits and drawbacks of each. First, let’s explore data sharing from Looker. Sharing data in Looker improves communication and collaboration, which leads to faster decision-making and improved efficiency. In addition, Looker provides a centralized repository for data, which ensures that data is accurate, consistent, and easy to find. Looker is also scalable, and can be integrated with other data sources and applications. However, there are also some drawbacks to using Looker to share data. First, Looker stores data in the cloud, which means that it’s potentially vulnerable to security breaches. However, Looker does offer several security features that can help to protect data, such as encryption and access control. Second, Looker is a paid platform, and the cost can be a factor for some organizations. Finally, Looker is a relatively complex platform, and there can sometimes be a steep learning curve. Alternatively, you can use Looker Studio to share data. Benefits of using Looker Studio include: Ease of use: Looker Studio is a user-friendly platform that makes it easy to share data. Users can create and share dashboards and reports with others, and they can also embed them in websites and applications. Flexibility: Looker Studio offers various features that let you customize the data sharing experiences. For example, you can control who has access to data, and you can also set permissions for different types of data. And lastly, security: Looker Studio offers security features that help to protect data, such as encryption and access control. However, Looker Studio is overall a less powerful platform than Looker, and does not offer the full set of features that Looker has. For example, Looker Studio does not support advanced data modeling or machine learning. Looker Studio also does not integrate with as many data sources as Looker. The lack of integrations can make it difficult to share data from various sources. Ultimately, the best platform for data sharing depends on the specific needs of the organization. Looker is a good choice for organizations that need a powerful and scalable platform for data sharing. Looker Studio is a good choice for organizations that are in search of a user-friendly platform. Now that you understand the benefits and drawbacks of data sharing with Looker and Looker Studio, let’s examine how to share data in Looker. This is often referred to as a “data delivery.” This Explore displays the results of a query. From the Settings menu, you can share your data-driven insights in a few different ways. First, you can save it as a report, called a Look, or to a dashboard, displaying several reports. Alternatively, to export data on a one-time basis, you can download or send it. Downloading extracts the data to your own computer. Looker supports downloading in different file formats, including a CSV, a zip file of one or more CSVs, a PDF, or a PNG. Sending lets you deliver the data somewhere else. The most popular destination is email; for example, you could email the dashboard to yourself and your manager. To send the data more than once, create a schedule, and define how often the report is sent to others. Scheduling is basically the same as sending, except with a delivery frequency such as daily or weekly. This is useful if you want to have a spreadsheet of the Look’s data automatically delivered to your inbox, say every Friday afternoon at the end of your work week. Finally, to send others the most recent data, you can simply click Share, then copy the URL, and send it to the people who need to see it. With the right permissions, those individuals can view the data. Next, let’s transition to data sharing in Looker Studio. Looker Studio is built on top of Google Drive, so you can share your reports and data source the same way you share docs, spreadsheets, and slides. Just like with Google Drive, users are given edit or view permission on the shared data. You can share a report in Looker studio from the Looker Studio home page or from the report itself. From the report, in addition to sharing, you can schedule a delivery, get a link to the report, or download it. Sharing in Looker Studio is very similar to Google Drive. You can choose whether you want recipients to be able to view or edit the report. Simply click Send to share the report. Data can be visualized and shared from both Looker and Looker Studio. What’s right for you and your team depends on the specific needs of your organization.

### Quiz - [Quiz: Making data-driven decisions using Looker ](https://www.cloudskillsboost.google/course_templates/578/quizzes/526297)

#### Quiz 1.

> [!important]
> **You ran a query and have results showing year-over-year sales growth. What type of Looker Studio visualization would be best to display the data?**
>
> - [ ] Line chart
> - [ ] Heatmap
> - [ ] Donut chart
> - [ ] Map

#### Quiz 2.

> [!important]
> **You are exploring data in Looker, and you need to narrow the results of the query. Which should you use?**
>
> - [ ] A pivot
> - [ ] A measure
> - [ ] A filter
> - [ ] A dimension

#### Quiz 3.

> [!important]
> **Which is a benefit of using Looker Studio to share data as opposed to Looker?**
>
> - [ ] Looker Studio features better access control and permissions.
> - [ ] You can create more specific visualizations in Looker Studio.
> - [ ] Looker Studio has more destination options.
> - [ ] Looker Studio has a stronger data analytics engine.

#### Quiz 4.

> [!important]
> **You want to send a report that shows task completion to your manager every Friday morning to give them visibility into your team's productivity. What is the best approach for sending data on a regular cadence?**
>
> - [ ] From the Share window in Looker Studio, grant your manager Manage access.
> - [ ] Copy and send the link to the report to your manager every Friday.
> - [ ] From Looker, create a schedule for the data.
> - [ ] From Looker Studio, schedule the data.

#### Quiz 5.

> [!important]
> **You want to save your query results as a report. What is a report referred to in Looker?**
>
> - [ ] A query
> - [ ] A Look
> - [ ] A chart
> - [ ] A dashboard

### Video - [Make data-driven decisions using Looker: Summary](https://www.cloudskillsboost.google/course_templates/578/video/526298)

- [YouTube: Make data-driven decisions using Looker: Summary](https://www.youtube.com/watch?v=rWBZRQio2MA)

This brings us to the end of this module on making data-driven decisions by using Looker. You’re now ready to get started analyzing, visualizing, and sharing data by using Looker and Looker Studio. Let’s recap what you learned. First, you received an introduction to data exploring in Looker, including manipulating a Looker Explore and using dimensions, measures, filters, and pivots to find the answers to data-driven questions. After that, you learned about the various visualization options available in both Looker and Looker Studio. You also received a demonstration of how to create a chart in Looker Studio. You also received a demonstration of how to create a chart in Looker Studio. Finally, you compared the benefits and drawbacks of using Looker and Looker Studio to share data with others, and learned how to share data from both platforms.

## Course Summary

This module reviews the topics covered in the course and provides resources for further learning. 

### Video - [Course Summary](https://www.cloudskillsboost.google/course_templates/578/video/526299)

- [YouTube: Course Summary](https://www.youtube.com/watch?v=r1XwKwP3GyE)

This brings us to the end of the Introduction to Data Analytics on Google Cloud course. Let’s recap what you learned. In the first section of the course, you learned the foundational steps and concepts for data analytics on Google Cloud. You explored: The end-to-end data analytics lifecycle on Google Cloud, from data ingestion to analysis and activation. How to decide between the various data storage options on Google Cloud. The different types of data and how they are used. The next section covered BigQuery, where you learned how to: Use BigQuery at a high level. Locate the data you need in BigQuery to facilitate your data analysis. And use basic SQL commands to answer a data-driven question. Lastly, in the final section of the course, you learned to: Use Looker to explore, analyze, and visualize data. Derive insights from data and use the data to make decisions. Differentiate between a Look and a dashboard. Decide between Looker and Looker Studio for data visualization and sharing. And create visualizations and share reports with Looker and Looker Studio. Now that you completed the Introduction to Data Analytics on Google Cloud course, you’re ready to start using Google Cloud tools and processes to analyze your organization's data. Thanks for joining us! We’ll see you next time.

### Document - [Course Resources](https://www.cloudskillsboost.google/course_templates/578/documents/526300)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
