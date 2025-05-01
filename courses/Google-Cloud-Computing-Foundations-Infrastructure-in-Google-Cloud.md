---
id: 154
name: 'Google Cloud Computing Foundations: Infrastructure in Google Cloud'
type: Course
url: https://www.cloudskillsboost.google/course_templates/154
date_published: 2025-04-29
topics:
  - Google Cloud Services
---

# [Google Cloud Computing Foundations: Infrastructure in Google Cloud](https://www.cloudskillsboost.google/course_templates/154)

**Description:**

The Google Cloud Computing Foundations courses are for individuals with little to no background or experience in cloud computing. They provide an overview of concepts central to cloud basics, big data, and machine learning, and where and how Google Cloud fits in.

By the end of the series of courses, learners will be able to articulate these concepts and demonstrate some hands-on skills.

The courses should be completed in the following order:
1. Google Cloud Computing Foundations: Cloud Computing Fundamentals
2. Google Cloud Computing Foundations: Infrastructure in Google Cloud
3. Google Cloud Computing Foundations: Networking and Security in Google Cloud
4. Google Cloud Computing Foundations: Data, ML, and AI in Google Cloud

**Objectives:**

* Implement a variety of structured and unstructured storage models.
* Discuss the different application managed service options in the cloud.
* Outline how security in the cloud is administered in Google Cloud.

## Where do I store this stuff?

Storage: Implement a variety of structured and unstructured storage models

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/154/video/532423)

* [YouTube: Introduction](https://www.youtube.com/watch?v=oAuQ3IbeGVo)

Welcome to Module 4 of the Google Cloud Computing Foundations course: Where do I store this stuff? In this module, you’ll learn about storage and database options available in Google Cloud. This means that you’ll: Explore the different storage options available in Google Cloud. Learn to differentiate between structured and unstructured storage in the cloud. Examine how you can use Cloud Storage for unstructured data storage. And explore the use case for relational versus NoSQL storage options and identify the options available with Google Cloud. Here’s the agenda for this module. We’ll begin by learning about different storage options in the cloud, which includes structured and unstructured storage. Next, we’ll learn how to leverage unstructured storage using Cloud Storage and complete a hands-on lab that explores a range of activities applicable to Cloud Storage. We’ll move on to understanding the use case for SQL managed services. Next, we’ll explore Cloud SQL, before completing another lab where we’ll create and connect to a Cloud SQL for MySQL instance and perform basic SQL operations using the Google Cloud console and the mysql client. We’ll discover how to leverage Spanner and explore the available NoSQL options. We’ll then discuss using Firestore as a fully managed, scalable, and serverless document database. We’ll complete the module by describing how Bigtable can be used as a NoSQL option. The module concludes with a short quiz and a summary of the topics covered. Let’s get started!

### Video - [Storage options in the cloud](https://www.cloudskillsboost.google/course_templates/154/video/532424)

* [YouTube: Storage options in the cloud](https://www.youtube.com/watch?v=ue_jy-Z4duA)

Let’s begin by exploring the different storage options available in Google Cloud. Every application needs to store data, like media to be streamed or perhaps even sensor data from devices, and different applications and workloads require different storage databases solutions. Google Cloud offers relational and non-relational databases and worldwide object storage. These options help users save costs, reduce the time it takes to launch, and make the most of their datasets by being able to analyze a wide variety of data. Choosing the right option to store and process data often depends on the data type that needs to be stored and the business need. Google Cloud provides managed storage and database services that are scalable, reliable, and easy to operate. These include: Cloud Storage, Cloud SQL, Spanner, Firestore, and Bigtable. The goal of these products is to reduce the time and effort needed to store data. This means creating an elastic storage bucket directly in a web interface or through a command line. There are three common cloud storage use cases. The first is content storage and delivery. This is when content, such as images or videos, needs to be served to users wherever they are. People want their content fast, so running on the global network that Google provides makes for a great experience for end users. The second use case is storage for data analytics and general compute. Users can process or expose their data to analytics tools, like the analytics stack of products that Google Cloud offers, and do things like genomic sequencing or IoT data analysis. The third use case is backup and archival storage. Users can save storage costs by migrating infrequently accessed content to cheaper cloud storage options. Also, if anything happens to their data on-premises, it's critical to have a copy in the cloud for recovery purposes. For users with databases, Google’s first priority is to help them migrate existing databases to the cloud and move them to the right service. This will usually be users moving MySQL or Postgre workloads to Cloud SQL. The second priority is to help users innovate, build or rebuild for the cloud, offer mobile applications, and plan for future growth.

### Video - [Structured and unstructured data storage](https://www.cloudskillsboost.google/course_templates/154/video/532425)

* [YouTube: Structured and unstructured data storage](https://www.youtube.com/watch?v=A2soo1a3ksQ)

Now you’ll learn to differentiate between structured and unstructured storage in the cloud. Let’s start with unstructured versus structured data. Unstructured data is information stored in a non-tabular form, such as documents, images, and audio files. Unstructured data is usually best suited to Cloud Storage. It’s estimated that around 80 percent of all data is unstructured. It’s far more difficult to process or analyze unstructured data using traditional methods because the data has no internal identifier to enable search functions to identify it. Unstructured data often includes text and multimedia content, for example, email messages, documents, photos, videos, presentations, and web pages. Organizations are focusing increasingly on mining unstructured data for insights that will provide them with a competitive edge. Alternatively, there is structured data, which represents information stored in tables, rows, and columns. Structured data is what most people are used to working with and typically fits within columns and rows in spreadsheets or relational databases. You can expect this type of data to be organized and clearly defined and usually easy to capture, access, and analyze. Examples of structured data include names, addresses, contact numbers, dates, and billing info. The benefit of structured data is that it can be understood by programming languages and can be manipulated relatively quickly. Structured data comes in two types: transactional workloads and analytical workloads. Transactional workloads stem from Online Transaction Processing systems, which are used when fast data inserts and updates are required to build row-based records. This is usually to maintain a system snapshot. They require relatively standardized queries that affect only a few records. So, if your data is transactional and you need to access it using SQL, Cloud SQL and Spanner are two options. Cloud SQL works best for local to regional scalability, but Spanner is best to scale a database globally. If the transactional data will be accessed without SQL, Firestore might be the best option. Firestore is a transactional NoSQL, document-oriented database. Then there are analytical workloads, which stem from Online Analytical Processing systems, which are used when entire datasets need to be read. They often require complex queries, for example, aggregations. If you have analytical workloads that require SQL commands, BigQuery may be the best option. BigQuery, Google’s data warehouse solution, lets you analyze petabyte-scale datasets. Alternatively, Bigtable provides a scalable NoSQL solution for analytical workloads. It’s best for real-time, high-throughput applications that require only millisecond latency.

### Video - [Unstructured storage using Cloud Storage](https://www.cloudskillsboost.google/course_templates/154/video/532426)

* [YouTube: Unstructured storage using Cloud Storage](https://www.youtube.com/watch?v=CK9NjUC81RM)

Now let’s examine how you can use Cloud Storage for unstructured data storage. Cloud Storage is a fully managed scalable service that has a wide variety of uses. A few examples include serving website content, storing data for archival and disaster recovery, and distributing large data objects to end users through Direct Download. Cloud Storage’s primary use is whenever binary large-object storage (also known as a “BLOB”) is needed for online content such as videos and photos, for backup and archived data, and for storage of intermediate results in processing workflows. But what is object storage? Object storage is a computer data storage architecture that manages data as “objects” and not as a file and folder hierarchy (file storage), or as chunks of a disk (block storage). These objects are stored in a packaged format that contains the binary form of the actual data itself, relevant associated metadata (such as date created, author, resource type, and permissions), and a globally unique identifier. These unique keys are in the form of URLs, which means object storage interacts well with web technologies. Data commonly stored as objects includes video, pictures, and audio recordings. Cloud Storage is Google’s object storage product. It allows customers to store any amount of data and to retrieve it as often as needed. In this lesson, we’ll learn more about Cloud Storage use cases, features, and pricing. There are four primary storage classes in Cloud Storage, and stored data is managed and billed according to which class it belongs in. The first is Standard Storage. Standard Storage is considered best for frequently accessed, or “hot,” data. It’s also great for data that is stored for only brief periods of time. The second storage class is Nearline Storage. This is best for storing infrequently accessed data, like reading or modifying data once per month on average. Examples include data backups, long-tail multimedia content, or data archiving. The third storage class is Coldline Storage. This is also a low-cost option for storing infrequently accessed data. However, as compared to Nearline Storage, Coldline Storage is meant for reading or modifying data, at most, once every 90 days. The fourth storage class is Archive Storage. This is the lowest-cost option, used ideally for data archiving, online backup, and disaster recovery. It’s the best choice for data that you plan to access less than once a year, because it has higher costs for data access and operations and a 365-day minimum storage duration. Although each of these four classes has differences, it’s worth noting that several characteristics apply across all these storage classes. These include: Unlimited storage with no minimum object size requirement, Worldwide accessibility and locations, Low latency and high durability, A uniform experience, which extends to security, tools, and APIs, and geo-redundancy if data is stored in a multi-region or dual-region. So this means placing physical servers in geographically diverse data centers to protect against catastrophic events and natural disasters and load-balancing traffic for optimal performance. Cloud Storage files are organized into buckets. A bucket needs a globally unique name and a specific geographic location for where it should be stored, and an ideal location for a bucket is where latency is minimized. For example, if most of your users are in Europe, you probably want to pick a European location - either a specific Google Cloud region in Europe, or else the EU multi-region. The storage objects offered by Cloud Storage are “immutable,” which means that you don’t edit them, but instead a new version is created with every change made. Administrators can either allow each new version to completely overwrite the older one or keep track of each change made to a particular object by enabling “versioning” within a bucket. If you choose to use versioning, Cloud Storage will keep a detailed history of modifications -- that is, overwrites or deletes -- of all objects contained in that bucket. If you don’t turn on object versioning, by default new versions will always overwrite older versions. With object versioning enabled, you can list the archived versions of an object, restore an object to an older state, or permanently delete a version of an object, as needed. Cloud Storage also offers lifecycle management policies for your objects. For example, you could tell Cloud Storage to delete objects older than 365 days, or to delete objects created before January 1, 2013, or to keep only the 3 most recent versions of each object in a bucket that has versioning enabled. We’ll look more closely at object lifecycle management a little bit later on. Cloud Storage’s tight integration with other Google Cloud products and services means that there are many additional ways to move data into the service. For example, you can import and export tables to and from both BigQuery and Cloud SQL. You can also store App Engine logs, Firestore backups, and objects used by App Engine applications like images. Cloud Storage can also store instance startup scripts, Compute Engine images, and objects used by Compute Engine applications.

### Video - [Lab Intro: Cloud Storage: Qwik Start - CLI/SDK](https://www.cloudskillsboost.google/course_templates/154/video/532427)

* [YouTube: Lab Intro: Cloud Storage: Qwik Start - CLI/SDK](https://www.youtube.com/watch?v=bdeNqmZdcpU)

It’s time for some hands-on practice with Cloud Storage. In the lab titled “Cloud Storage: Qwik Start - CLI/SDK,” you’ll create a storage bucket, upload objects, create folders and subfolders, and make objects publicly accessible using the Google Cloud command line. During this lab, you’ll upload an object to a bucket, download an object from a bucket, copy an object to a folder in the bucket, list contents of a bucket or folder, list details for an object, and make an object publicly accessible.

### Lab - [Cloud Storage: Qwik Start - CLI/SDK](https://www.cloudskillsboost.google/course_templates/154/labs/532428)

This hands-on lab shows you how to perform basic tasks in Cloud Storage using the gsutil command-line tool. Watch the short video <A HREF="https://youtu.be/081hh6EzlTk">Google Cloud Storage: Massive Scalability Plus More</A>. 

* [ ] [Cloud Storage: Qwik Start - CLI/SDK](../labs/Cloud-Storage-Qwik-Start-CLI-SDK.md)

### Video - [SQL managed services](https://www.cloudskillsboost.google/course_templates/154/video/532429)

* [YouTube: SQL managed services](https://www.youtube.com/watch?v=jytglmK_ako)

Now we’ll explore the use case for SQL-managed services. But first, let’s revisit what a database is and how it’s used. A database is a collection of information that’s organized so that it can easily be accessed and managed. Users are building software applications using databases to answer business questions such as buying a ticket, filing an expense report, storing a photo, or storing medical records. Computer applications run databases to get a fast answer to questions like: What’s this user’s name, given their sign-in information, so I can display it? What’s the cost of product Y so I can show it on my dynamic web page? What were my top 10 best selling products this month? And what’s the next ad that I should show the user currently browsing my site? These apps must be able to write data in and read data out of databases. When a database is used, it’s usually run by a computer application. So when we say that “a database is useful for doing X,” it’s usually because it’s designed to make answering a question simple, fast, and efficient for the app. Relational database management systems, abbreviated to RDBMS, or just relational databases, are used extensively and are the kind of database you encounter most of the time. They’re organized based on the relational model of data. They’re very good when you have a well-structured data model and when you need transactions and the ability to join data across tables to retrieve complex combinations of your data. Because they make use of the Structured Query Language, they are sometimes called SQL databases. Google Cloud offers two managed relational database services, Cloud SQL and Spanner. Let’s explore each of them in detail.

### Video - [Exploring Cloud SQL](https://www.cloudskillsboost.google/course_templates/154/video/532430)

* [YouTube: Exploring Cloud SQL](https://www.youtube.com/watch?v=U45xAi9Ajno)

We’ll begin with Cloud SQL. Cloud SQL offers fully managed relational databases, including MySQL, PostgreSQL, and SQL Server as a service. It’s designed to hand off mundane, but necessary and often time-consuming, tasks to Google, like applying patches and updates, managing backups, and configuring replications, so your focus can be on building great applications. Cloud SQL: Doesn't require any software installation or maintenance. Can scale up to 96 processor cores, 624 GB of RAM, and 64 TB of storage. Supports automatic replication scenarios, such as from a Cloud SQL primary instance, an external primary instance, and external MySQL instances. Supports managed backups, so backed-up data is securely stored and accessible if a restore is required. The cost of an instance covers seven backups. Encrypts customer data when on Google’s internal networks and when stored in database tables, temporary files, and backups. And includes a network firewall, which controls network access to each database instance.

### Video - [Lab Intro: Cloud SQL for MySQL: Qwik Start](https://www.cloudskillsboost.google/course_templates/154/video/532431)

* [YouTube: Lab Intro: Cloud SQL for MySQL: Qwik Start](https://www.youtube.com/watch?v=ZsQefAbsIS0)

To help you learn more about using Cloud SQL, let’s complete a hands-on lab. In the lab titled “Cloud SQL for MySQL: Qwik Start,” you’ll create and connect to a Cloud SQL for MySQL instance and perform basic SQL operations using the Google Cloud console and the mysql client. During this lab, you’ll create a Cloud SQL instance, and connect to an instance using the mysql client in the Cloud Shell.

### Lab - [Cloud SQL for MySQL: Qwik Start](https://www.cloudskillsboost.google/course_templates/154/labs/532432)

In this lab, you create a Google Cloud SQL MySQL instance and perform SQL operations using Google Cloud Platform Console and mysql client. Watch this short video, <a HREF="https://youtu.be/EQJK0tNW-g4">Manage PostgreSQL and MySQL Databases Easily with Cloud SQL</a>.

* [ ] [Cloud SQL for MySQL: Qwik Start](../labs/Cloud-SQL-for-MySQL-Qwik-Start.md)

### Video - [Spanner as a managed service](https://www.cloudskillsboost.google/course_templates/154/video/532433)

* [YouTube: Spanner as a managed service](https://www.youtube.com/watch?v=adOnlL_30ro)

In this next section, you’ll explore how Spanner can be leveraged as a managed service. Spanner is a fully managed relational database service that scales horizontally, is strongly consistent, and speaks SQL. Vertical scaling is where you make a single instance larger or smaller, while horizontal scaling is when you scale by adding and removing servers. Spanner users are often in the advertising, finance, and marketing technology industries, where they need to manage end-user metadata. Tested by Google’s own mission-critical applications and services, Spanner is the service that powers Google’s $80 billion business. Spanner is especially suited for applications that require: A SQL relational database management system with joins and secondary indexes, Built-in high availability, Strong global consistency, And high numbers of input/output operations per second, such as tens of thousands of reads/writes per second. So how does Spanner work? Data is automatically and instantly copied across regions, which is called synchronous replication. As a result, queries always return consistent and ordered answers regardless of the region. Google uses replication within and across regions to achieve availability, so if one region goes offline, the user’s data can still be served from another region.

### Video - [NoSQL managed services options](https://www.cloudskillsboost.google/course_templates/154/video/532434)

* [YouTube: NoSQL managed services options](https://www.youtube.com/watch?v=wJTm4gwotmM)

Now we’ll explore the NoSQL managed services options currently available. Google offers two managed NoSQL database options, Firestore and Bigtable. Firestore is a fully managed, serverless NoSQL document store that supports ACID transactions. Bigtable is a petabyte scale, sparse wide column NoSQL database that offers extremely low write latency. Let’s explore each option in detail.

### Video - [Firestore, a NoSQL document store](https://www.cloudskillsboost.google/course_templates/154/video/532435)

* [YouTube: Firestore, a NoSQL document store](https://www.youtube.com/watch?v=ifpUh4hlpsw)

In this next section, you’ll explore Firestore, a database that lets you develop rich applications using a fully managed, scalable, and serverless document database. Firestore is a flexible, horizontally scalable, NoSQL cloud database for mobile, web, and server development. With Firestore, incoming data is stored in a document structure, and these documents are then organized into collections. Documents can contain complex nested objects in addition to subcollections. Firestore’s NoSQL queries can then be used to retrieve individual, specific documents or to retrieve all the documents in a collection that match your query parameters. Queries can include multiple, chained filters and combine filtering and sorting options. They're also indexed by default, so query performance is proportional to the size of the result set, not the dataset. Firestore uses data synchronization to update data on any connected device. However, it's also designed to make simple, one-time fetch queries efficiently. It caches data that an app is actively using, so the app can write, read, listen to, and query data even if the device is offline. When the device comes back online, Firestore synchronizes any local changes back to Firestore. Firestore leverages Google Cloud’s powerful infrastructure: automatic multi-region data replication, strong consistency guarantees, atomic batch operations, and real transaction support.

### Video - [Bigtable as a NoSQL option](https://www.cloudskillsboost.google/course_templates/154/video/532436)

* [YouTube: Bigtable as a NoSQL option](https://www.youtube.com/watch?v=qS84shcBUUI)

The final topic of this module describes how to leverage Bigtable as a NoSQL option. Bigtable is Google's NoSQL big data database service. It's the same database that powers many core Google services, including Search, Analytics, Maps, and Gmail. Bigtable is designed to handle massive workloads at consistent low latency and high throughput, so it's a great choice for both operational and analytical applications, including Internet of Things, user analytics, and financial data analysis. When deciding which storage option is best, customers often choose Bigtable if: They’re working with more than 1 TB of semi-structured or structured data. Data is fast with high throughput, or it’s rapidly changing. They’re working with NoSQL data. This usually means transactions where strong relational semantics are not required. Data is a time-series or has natural semantic ordering. They’re working with big data, running asynchronous batch or synchronous real-time processing on the data. Or they’re running machine learning algorithms on the data. Bigtable can interact with other Google Cloud services and third-party clients. Using APIs, data can be read from and written to Bigtable through a data service layer like Managed VMs, the HBase REST Server, or a Java Server using the HBase client. Typically this is used to serve data to applications, dashboards, and data services. Data can also be streamed in through various popular stream processing frameworks like Dataflow Streaming, Spark Streaming, and Storm. And if streaming isn’t an option, data can also be read from and written to Bigtable through batch processes like Hadoop MapReduce, Dataflow, or Spark. Often, summarized or newly calculated data is written back to Bigtable or to a downstream database. BigQuery isn’t mentioned in this module because it sits on the edge between data storage and data processing and is covered in more depth in other courses. The usual reason to store data in BigQuery is so you can use its big data analysis and interactive querying capabilities. It is not purely a data storage product.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/154/quizzes/532437)

#### Quiz 1.

> [!important]
> **Which storage solution is a petabyte scale, NoSQL database?**
>
> * [ ] Firestore
> * [ ] Spanner
> * [ ] Bigtable
> * [ ] Cloud SQL

#### Quiz 2.

> [!important]
> **You are looking for an unstructured storage solution for archiving files that might never be accessed again. Which Cloud Storage class is the best option?**
>
> * [ ] Archive storage
> * [ ] Nearline storage
> * [ ] Coldline storage
> * [ ] Standard storage

#### Quiz 3.

> [!important]
> **Which storage service is best suited to unstructured data?**
>
> * [ ] Cloud Storage
> * [ ] Firestore
> * [ ] Bigtable
> * [ ] Spanner

#### Quiz 4.

> [!important]
> **Google Cloud offers two managed relational database services. What are they?**
>
> * [ ] Spanner
> * [ ] Cloud SQL
> * [ ] Bigtable
> * [ ] Firestore

### Video - [Summary](https://www.cloudskillsboost.google/course_templates/154/video/532438)

* [YouTube: Summary](https://www.youtube.com/watch?v=fSpbQgIleC4)

This brings us to the end of the fourth module of the Google Cloud Computing Foundations course. Let’s do a quick summary. In this module, you’ve explored the different storage options available in Google Cloud. This list includes Cloud Storage, Cloud SQL, Spanner, Firestore, and Bigtable. Learned to differentiate between structured and unstructured storage in the cloud. Unstructured data is information stored in a non-tabular form such as documents, images, and audio files. Alternatively, structured data represents information stored in tables, rows, and columns. Examined how you can use Cloud Storage for unstructured data storage. Cloud Storage’s primary use is whenever binary large-object storage (also known as a “BLOB”) is needed for online content such as videos and photos, for backup and archived data, and for storage of intermediate results in processing workflows. And explored the use case for relational versus NoSQL storage options, and identified the options available with Google Cloud.

## There’s an API for that!

Managed Services: Discuss the different application managed service options in the cloud

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/154/video/532439)

* [YouTube: Introduction](https://www.youtube.com/watch?v=WkXuIWPZQ74)

Welcome to module five of the Google Cloud Computing Foundations course: There’s an API for that! In this section of the course, you’ll explore how to build applications with managed services. This means that you’ll: 1. Explore the purpose and benefit of APIs. 2. Compare Cloud Endpoints and Apigee API Management, two different API management tools, and 3. Examine Pub/Sub, a Google Cloud tool to handle distributed message-oriented architectures at scale. The module agenda follows the objectives. It begins with an exploration of the purpose of APIs, including the REST API, which is currently the most popular style for services. From there, you’ll explore Cloud Endpoints, which is a distributed API management system, before completing a hands-on lab where you’ll deploy a sample API with Cloud Endpoints. After that, you’ll explore Apigee API Management, which is a platform for developing and managing API proxies. Then, you’ll learn about the use case for managed services, followed by Pub/Sub, which is Google’s managed message system. The module concludes with another hands-on lab, followed by a short quiz and a summary of the topics covered. Let’s get started!

### Video - [The purpose of APIs](https://www.cloudskillsboost.google/course_templates/154/video/532440)

* [YouTube: The purpose of APIs](https://www.youtube.com/watch?v=tak-JtvyiiM)

Let's start by discussing the purpose of APIs. What is an API, exactly? A software service’s implementation can be complex and changeable. If other software services had to be explicitly coded in detail in order to use that service, the result would be brittle and error-prone. So instead, application developers structure the software they write so that it presents a clean, well-defined interface that hides unnecessary detail, and then they document that interface. That’s an application programming interface. The underlying implementation can change, as long as the interface doesn’t, and other pieces of software that use the API don’t have to know or care. APIs are used to simplify the way different, disparate, software resources communicate. By using a universal structure of communications, we open up a wide range of opportunities. Sometimes you do have to change an API, perhaps to add or deprecate a feature. To cleanly make this kind of change to the API, developers create versions. For example, version 2 of an API might contain calls that version 1 does not. This means that programs that consume the API can specify the API version they want to use in their calls. REpresentational State Transfer, or REST, is currently the most popular architectural style for services. It outlines a key set of constraints and agreements that a service must comply with. If a service complies with these REST constraints, it’s said to be RESTful. The web is HTTP-based and provides an architectural structure that scales well and stands the test of time. REST transfers the ideas that worked so well for the web and applies them to services. APIs intended to be spread widely to consumers and deployed to devices with limited computing resources, like mobile, are well suited to a REST structure. REST APIs use HTTP requests to perform GET, PUT, POST, and DELETE operations. Having different software services leverage a universal communication channel ensures that applications can be updated or rewritten and still work with other applications, as long as they conform to the agreed-upon API standard. One of the main reasons REST APIs work well with the cloud is due to their stateless nature. State information does not need to be stored or referenced for the API to run. Also, authentication can be done through OAuth, and security can be used by leveraging tokens. When deploying and managing APIs on your own, there are several issues to consider. These include the language or format you’ll use to describe the interface, how you’ll authenticate services and users who invoke your API, how you’ll ensure that your API scales to meet demand, and whether your infrastructure log details API invocations and provides monitoring metrics.

### Video - [Apigee Edge](https://www.cloudskillsboost.google/course_templates/154/video/532441)

* [YouTube: Apigee Edge](https://www.youtube.com/watch?v=ukVnGYjLbrU)

Another Google Cloud platform available for developing and managing API proxies is Apigee API Management. Unlike Cloud Endpoints, Apigee API Management has a specific focus on business problems, like rate limiting, quotas, and analytics. In fact, many Apigee API Management users provide a software service to other companies. Backend services for Apigee API Management don't have to be in Google Cloud, and as a result, engineers also often use it to take apart legacy applications. So, instead of replacing a large, important application in one move, they can use Apigee API Management to peel off its services individually. This allows them to stand up microservices to implement each in turn, until the legacy application can finally be retired.

### Video - [Pub/Sub](https://www.cloudskillsboost.google/course_templates/154/video/532442)

* [YouTube: Pub/Sub](https://www.youtube.com/watch?v=Q_yUa1mWPQU)

Now let’s explore Pub/Sub, a Google Cloud asynchronous messaging service and API that supports distributed message-oriented architectures at scale. One of the early stages in a data pipeline is data ingestion, which is where large amounts of streaming data are received. Data, however, may not always come from a single, structured database. Instead, the data might stream from a thousand, or even a million, different events that are all happening asynchronously. A common example of this is data from IoT, or Internet of Things, applications. These can include sensors on taxis that send out location data every 30 seconds or temperature sensors around a data center to help optimize heating and cooling. These IoT devices present new challenges to data ingestion, which can be summarized in four points: 1. The first is that data can be streamed from many different methods and devices, many of which might not talk to each other and might be sending bad or delayed data. 2. The second is that it can be hard to distribute event messages to the right subscribers. Event messages are notifications. A method is needed to collect the streaming messages that come from IoT sensors and broadcast them to the subscribers as needed. 3. The third is that data can arrive quickly and at high volumes. Services must be able to support this. 4. And the fourth challenge is ensuring that services are reliable and secure, and perform as expected. The name Pub/Sub is short for Publisher/Subscriber, or publish messages to subscribers. Pub/Sub is a distributed messaging service that can receive messages from various device streams such as gaming events, IoT devices, and application streams. Pub/Sub ensures at-least-once delivery of received messages to subscribing applications, with no provisioning required. Pub/Sub’s APIs are open, the service is global by default, and it offers end-to-end encryption. Let’s explore the end-to-end Pub/Sub architecture. * Upstream source data comes in from devices all over the globe and is ingested into Pub/Sub, which is the first point of contact within the system. Pub/Sub reads, stores, and broadcasts to any subscribers of this data topic that new messages are available. * As a subscriber of Pub/Sub, Dataflow can ingest and transform those messages in an elastic streaming pipeline and output the results into an analytics data warehouse like BigQuery. * Finally, you can connect a data visualization tool, like Looker or Looker Studio, to visualize and monitor the results of a pipeline, or an AI or ML tool such as Vertex AI to explore the data to uncover business insights or help with predictions. A central element of Pub/Sub is the topic. A topic is a named resource to which messages are sent by publishers. You can think of a topic like a radio antenna. Whether your radio is playing music or it’s turned off, the antenna itself is always there. If music is being broadcast on a frequency that nobody’s listening to, the stream of music still exists. Similarly, a publisher can send data to a topic that has no subscriber to receive it. Or a subscriber can be waiting for data from a topic that isn’t getting data sent to it, like listening to static from a bad radio frequency. Or you could have a fully operational pipeline where the publisher is sending data to a topic that an application is subscribed to. That means there can be zero, one, or more publishers, and zero, one or more subscribers related to a topic. And they’re completely decoupled, so they’re free to break without affecting their counterparts. It’s helpful to describe this using an example. Say you’ve got a human resources topic. A new employee joins your company, and several applications across the company need to be updated. Adding a new employee can be an event that generates a notification to the other applications that are subscribed to the topic, and they’ll receive the message about the new employee starting. Now, let’s assume that there are two different types of employees: a full-time employee and a contractor. Both sources of employee data could have no knowledge of the other but still publish their events saying “this employee joined” into the Pub/Sub HR topic. After Pub/Sub receives the message, downstream applications like the directory service, facilities system, account provisioning, and badge activation systems can all listen and process their own next steps independent of one another. Pub/Sub is a good solution to buffer changes for lightly coupled architectures, like this one, that have many different sources and sinks. Pub/Sub supports many different inputs and outputs, and you can even publish a Pub/Sub event from one topic to another. The next task is to get these messages reliably into our data warehouse, and we’ll need a pipeline that can match Pub/Sub’s scale and elasticity to do it.

### Video - [Lab Intro: Pub/Sub: Qwik Start - Python](https://www.cloudskillsboost.google/course_templates/154/video/532443)

* [YouTube: Lab Intro: Pub/Sub: Qwik Start - Python](https://www.youtube.com/watch?v=Vxxb7hrBu6k)

Now it’s time for some hands-on practice with Pub/Sub. In the lab titled “Pub/Sub: Qwik Start - Python,” you’ll publish messages with Pub/Sub using the Python client library. During this lab, you’ll: Learn the basics of Pub/Sub. Create and list a Pub/Sub topic. Create and list a Pub/Sub subscription. Publish messages to a topic. Use a pull subscriber to output individual topic messages.

### Lab - [Pub/Sub: Qwik Start - Python](https://www.cloudskillsboost.google/course_templates/154/labs/532444)

In this lab, you learn about Pub/Sub and how to create a topic and subscriber with a Python script, and then publish and view messages. Watch the short video <A HREF="https://youtu.be/oKU2wbTXMTY">Simplify Event Driven Processing with Cloud Pub/Sub</A>.

* [ ] [Pub/Sub: Qwik Start - Python](../labs/Pub-Sub-Qwik-Start-Python.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/154/quizzes/532445)

#### Quiz 1.

> [!important]
> **Which platform for developing and managing API proxies has a specific focus on business problems, like rate limiting, quotas, and analytics?**
>
> * [ ] Apigee API Management
> * [ ] Pub/Sub
> * [ ] Cloud Endpoints
> * [ ] REST API

#### Quiz 2.

> [!important]
> **Which statement about Pub/Sub is true?**
>
> * [ ] Pub/Sub is regional by default.
> * [ ] Pub/Sub is unencrypted.
> * [ ] Pub/Sub requires provisioning.
> * [ ] Pub/Sub's APIs are open.

#### Quiz 3.

> [!important]
> **What does API stand for?**
>
> * [ ] Applied Programming Interface
> * [ ] Asynchronous Programming Interface
> * [ ] Application Programming Interface
> * [ ] Artificial Programming Interface

#### Quiz 4.

> [!important]
> **Which API management system supports applications running in App Engine, Google Kubernetes Engine, and Compute Engine?**
>
> * [ ] Cloud Endpoints
> * [ ] Pub/Sub
> * [ ] REST API
> * [ ] Apigee

### Video - [Summary](https://www.cloudskillsboost.google/course_templates/154/video/532446)

* [YouTube: Summary](https://www.youtube.com/watch?v=5WShSNQbKcM)

This brings us to the end of the fifth module of the Google Cloud Computing Foundations course. Let’s do a quick summary. 1. You started by exploring the purpose and benefit of application programming interfaces, or APIs. 2. Next, you compare Cloud Endpoints and Apigee API Management, two different API management tools. 3. And finally, you examined Pub/Sub, a Google Cloud tool to handle distributed message-oriented architectures at scale.

## You can’t secure the cloud, right?

Security: Outline how security in the cloud is administered in Google Cloud

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/154/video/532447)

* [YouTube: Introduction](https://www.youtube.com/watch?v=Xben1lzkf8E)

Welcome to module six of the Google Cloud Computing Foundations course: You can’t secure the cloud, right? In this section of the course, you’ll learn about security best practices for the cloud. This means that you’ll: Outline how security is administered in Google Cloud, including the shared security model. Explore the different encryption options with Google Cloud. Identify best practices when you configure authentication and authorization with Identity and Access Management (IAM). The module agenda follows the objectives. You’ll begin by exploring what security in the cloud means, followed by an overview of the shared security model. After that, you’ll compare Google's security responsibilities with a customer's responsibilities. Then, you’ll learn about encryption options, including authentication and authorization with IAM. You’ll be introduced to Identity-Aware Proxy (IAP), and then complete a lab where you’ll use IAP to set up user authentication. From there, you’ll identify authorization best practices for using IAM, followed by a hands-on lab. And finally, the module concludes with a short quiz and a recap of the topics covered. Let’s get started!

### Video - [Security in the cloud](https://www.cloudskillsboost.google/course_templates/154/video/532448)

* [YouTube: Security in the cloud](https://www.youtube.com/watch?v=WDVLDbzmYZA)

Let’s begin with an introduction to security in the cloud. Because Google has nine* services with more than a billion users, security is always on the minds of Google's employees. Design for security is prevalent, throughout the infrastructure, that Google Cloud and Google services run-on. Let's talk about the different fiver layers of protection Google provides to keep customers' data safe: Hardware infrastructure Service deployment Storage services Internet communication Operational security At the hardware infrastructure layer: Hardware design and provenance: Both the server boards and the networking equipment in Google data centers are custom designed by Google. Google also designs custom chips, including a hardware security chip that's currently being deployed on both servers and peripherals. Secure boot stack: Google server machines use various technologies to ensure that they are booting the correct software stack, such as cryptographic signatures over the BIOS, bootloader, kernel, and base operating system image. Premises security: Google designs and builds its own data centers, which incorporate multiple layers of physical security protections. Access to these data centers is limited to only a small fraction of Google employees. Google also hosts some servers in third-party data centers, where we ensure that there are Google-controlled physical security measures on top of the security layers provided by the data center operator. At the service deployment layer: Encryption of inter-service communication: Google’s infrastructure provides cryptographic privacy and integrity for remote procedure call (“RPC”) data on the network. Google’s services communicate with each other using RPC calls. The infrastructure automatically encrypts all infrastructure RPC traffic which goes between data centers. Google has started to deploy hardware cryptographic accelerators that will allow it to extend this default encryption to all infrastructure RPC traffic inside Google data centers. User identity: Google’s central identity service, which usually manifests to end users as the Google login page, goes beyond asking for a simple username and password. The service also intelligently challenges users for additional information based on risk factors such as whether they have logged in from the same device or a similar location in the past. Users also have the option of employing secondary factors when signing in, including devices based on the Universal 2nd Factor (U2F) open standard. At the storage services layer: Encryption at rest: Most applications at Google access physical storage (in other words, “file storage”) indirectly by using storage services, and encryption (using centrally managed keys) is applied at the layer of these storage services. Google also enables hardware encryption support in hard drives and SSDs. At the internet communication layer: Google Front End (GFE): Google services that want to make themselves available on the internet register themselves with an infrastructure service called the Google Front End, which ensures that all TLS connections are ended using a public-private key pair and an X.509 certificate from a Certified Authority (CA), and follows best practices such as supporting perfect forward secrecy. The GFE also applies protections against Denial of Service attacks. Denial of Service (DoS) protection: The sheer scale of its infrastructure enables Google to simply absorb many DoS attacks. Google also has multi-tier, multi-layer DoS protections that further reduce the risk of any DoS impact on a service running behind a GFE. Finally, at Google’s operational security layer: Intrusion detection: Rules and machine intelligence give Google’s operational security teams warnings of possible incidents. Google conducts Red Team exercises to measure and improve the effectiveness of its detection and response mechanisms. Reducing insider risk: Google aggressively limits and actively monitors the activities of employees who have been granted administrative access to the infrastructure. Employee U2F use: To guard against phishing attacks against Google employees, employee accounts require use of U2F-compatible security keys. Software development practices: Google employs central source control and requires two-party review of new code. Google also provides its developers with libraries that prevent them from introducing certain classes of security bugs. Google also runs a Vulnerability Rewards Program where we pay anyone who can discover and inform us of bugs in our infrastructure or applications.

### Video - [The shared security model](https://www.cloudskillsboost.google/course_templates/154/video/532449)

* [YouTube: The shared security model](https://www.youtube.com/watch?v=j7TlkaNNBew)

Now that you have some insights into Google’s security model, let’s explore users’ security responsibilities in the cloud. Security responsibilities are shared between the customer and Google Cloud. When a customer deploys an application to their on-premises infrastructure, they are responsible for the security of the entire stack: from the physical security of the hardware and the premises in which they are housed, through to the encryption of the data on disk, the integrity of the network, all the way up to securing the content stored in those applications. But when they move an application to Google Cloud, Google handles many of the lower layers of security, like the physical security, disk encryption, and network integrity. The upper layers of the security stack, including the securing of data, remain the customer’s responsibility. Google provides tools like the resource hierarchy and IAM to help them define and implement policies, but ultimately this part is their responsibility. Data access is usually the customer’s responsibility. They control who or what has access to their data. Google Cloud provides tools that help them control this access, such as Identity and Access Management, but they must be properly configured to protect your data.

### Video - [Encryption options](https://www.cloudskillsboost.google/course_templates/154/video/532450)

* [YouTube: Encryption options](https://www.youtube.com/watch?v=rFWOkh7snbA)

Now let’s explore the different options Google Cloud offers to encrypt data. Several encryption options are available on Google Cloud. These range from simple but with limited control, to greater control flexibility but with more complexity. The simplest option is Google Cloud default encryption, followed by customer-managed encryption keys (CMEK), and the option that provides the most control: customer-supplied encryption keys (CSEK). A fourth option is to encrypt your data locally before you store it in the cloud. This is often called client-side encryption. Google Cloud will encrypt data in transit and at rest by default. Data in transit is encrypted by using Transport Layer Security (TLS). Data encrypted at rest is done with AES 256-bit keys. The encryption happens automatically. With customer-managed encryption keys, you manage your encryption keys that protect data on Google Cloud. Cloud Key Management Service, or Cloud KMS, automates and simplifies the generation and management of encryption keys. The keys are managed by the customer and never leave the cloud. Cloud KMS supports encryption, decryption, signing, and verification of data. It supports both symmetric and asymmetric cryptographic keys and various popular algorithms. Cloud KMS lets you both rotate keys manually and automate the rotation of keys on a time-based interval. Cloud KMS also supports both symmetric keys and asymmetric keys for encryption and signing. Customer-supplied encryption keys give users more control over their keys, but with greater management complexity. With CSEK, users use their own AES 256-bit encryption keys. They are responsible for generating these keys. Users are responsible for storing the keys and providing them as part of Google Cloud API calls. Google Cloud will use the provided key to encrypt the data before saving it. Google guarantees that the key only exists in-memory and is discarded after use. Persistent disks, such as those that back virtual machines, can be encrypted with customer-supplied encryption keys. With CSEK for persistent disks, the data is encrypted before it leaves the virtual machine. Even without CSEK or CMEK, persistent disks are still encrypted. When a persistent disk is deleted, the keys are discarded, and the data is rendered irrecoverable by traditional means. To have more control over persistent disk encryption, users can create their own persistent disks and redundantly encrypt them. And finally, client-side encryption is always an option. With client-side encryption, users encrypt data before they send it to Google Cloud. Neither the unencrypted data nor the decryption keys leave their local device.

### Video - [Authentication and authorization with IAM](https://www.cloudskillsboost.google/course_templates/154/video/532451)

* [YouTube: Authentication and authorization with IAM](https://www.youtube.com/watch?v=8xERsepsq-4)

In the next section, you’ll learn how to improve the security of an infrastructure by using authentication and authorization with IAM. When an organization node contains lots of folders, projects, and resources, it’s likely this workforce might need to restrict access. To help with this task, administrators can use Identity and Access Management, or IAM. With IAM, administrators can apply policies that define who can do what on which resources. The “who” part of an IAM policy can be a Google Account, a Google group, a service account, or Cloud Identity domain. The “can do what” part of an IAM policy is defined by a role. An IAM role is a collection of permissions. For example, to manage virtual machine instances in a project, you need to create, delete, start, stop, and change virtual machines. So, these permissions are grouped into a role to make them easier to understand and manage. When a user, group, or service account is given a role on a specific element of the resource hierarchy, the resulting policy applies to the chosen element and to all the elements below it in the hierarchy. You can define deny rules that prevent certain principals from using certain permissions, regardless of the roles they're granted. This is because IAM always checks relevant deny policies before checking relevant allow policies. Deny policies, like allow policies, are inherited through the resource hierarchy. When new Google Cloud customers start using the platform, it’s common to log into the Google Cloud console with a Gmail account, and then use Groups to collaborate with teammates who are in similar roles. Although this approach is easy to start with, it can be challenging later because the team’s identities are not centrally managed. This can be problematic if someone leaves the organization. With this setup, it’s not easy to immediately remove a user’s access to the team’s cloud resources. With a tool called Cloud Identity, organizations can define policies and manage their users and groups by using the Google Admin console. Admins can log in and manage Google Cloud resources by using the same usernames and passwords they already use in existing Active Directory or LDAP systems. With Cloud Identity, when someone leaves an organization, an administrator can use the Google Admin console to disable their account and remove them from groups. Cloud Identity is available in a free edition, and a premium edition that provides capabilities to manage mobile devices. If you’re a Google Cloud and a Google Workspace customer, this functionality is already available to you in the Google Admin console. There are three kinds of roles in IAM: basic, predefined, and custom. The first role type is basic. Basic roles are broad in scope. When applied to a Google Cloud project, they affect all resources in that project. Basic roles include owner, editor, viewer, and billing administrator. Let’s have a look at these basic roles: Project viewers can examine resources, but can’t modify them. Project editors can examine and modify a resource. And project owners can also examine and modify a resource. In addition, project owners can manage the associate roles and permissions, and set up billing. Often companies want someone to control the billing for a project, but not have permissions to change the resources in the project. This is possible through a billing administrator role. Note: If several people are working together on a project that contains sensitive data, basic roles are probably too broad. Fortunately, IAM provides other ways to assign permissions that are more specifically tailored to meet the needs of typical job roles. This brings us to the second type of role: predefined roles. Specific Google Cloud services offer sets of predefined roles, and they even define where those roles can be applied. Let’s take Compute Engine, a Google Cloud product that offers virtual machines as a service. With Compute Engine, you can apply specific predefined roles, such as “instanceAdmin,” to Compute Engine resources in a given project, a given folder, or an entire organization. This then allows whoever has these roles to perform a specific set of predefined actions. But what if you need to assign a role that has even more specific permissions? You’d use a custom role. Many companies use a “least-privilege” model, in which each person in your organization is given the minimal amount of privilege needed to do their job. So, for example, maybe you want to define an “instanceOperator” role to allow some users to stop and start Compute Engine virtual machines, but not reconfigure them. Custom roles allow for that. Before you start creating custom roles, please note two important details. First, you must manage the permissions that comprise the custom role you’ve created. Because of this, some companies decide to stick with the predefined roles. And second, custom roles can only be applied to either project or organization level. They can’t be applied to the folder level. Let’s say you have an application running in a virtual machine that needs to store data in Cloud Storage, but you don’t want just anyone on the internet to have access to that data, just that particular virtual machine. You can create a service account to authenticate that VM to Cloud Storage. Service accounts are named with an email address, but instead of passwords, they use cryptographic keys to access resources. So, if a service account has been granted Compute Engine’s Instance Admin role, this would allow an application that runs in a VM with that service account to create, modify, and delete other VMs. Service accounts must be managed. For example, maybe Alice needs to manage which Google Accounts can act as service accounts, but Bob just needs to view a list of service accounts. Fortunately, in addition to being an identity (a user), a service account is also a resource! So it can have IAM policies of its own attached to it. This means that Alice can have the editor role on a service account, and Bob can have the viewer role. This is just like granting roles for any other Google Cloud resource.

### Video - [Lab Intro: User Authentication: Identity-Aware Proxy](https://www.cloudskillsboost.google/course_templates/154/video/532452)

* [YouTube: Lab Intro: User Authentication: Identity-Aware Proxy](https://www.youtube.com/watch?v=tV_DzWDCaGI)

Identity-Aware Proxy, or IAP, is a resource that can be used to set up authentication to https-based applications without the use of VPNs. In this section of the course, you’ll use IAP to set up user authentication. IAP lets you establish a central authorization layer for applications over TLS, so you can use an application-level access control model instead of relying on network-level firewalls. Only users and groups can access applications and resources protected by IAP through the proxy with the correct IAM role. The proxy provides a layer of protection between the outside world and an internal service. When you grant a user access to an application or resource by IAP, they’re subject to the granular access controls implemented by the product in use, without requiring a VPN. IAP performs authentication and authorization checks when a user tries to access a IAP-secured resource. IAP secures authentication and authorization of external requests through TLS. IAP doesn't protect against activities inside your VM, such as if someone uses SSH to access the VM. IAP also doesn’t protect against activities within a project, such as VM-to-VM communication within your project over the local network. In the lab titled, “User Authentication: Identity-Aware Proxy,” you’ll build a minimal web application with App Engine and explore ways to use IAP to restrict access to the application and provide user identity information to it. During this lab, you’ll: Use Python to write and deploy a simple App Engine app. Enable and disable IAP to restrict access to your app. Get user identify information from IAP into your app. Cryptographically verify information from IAP to protect against spoofing.

### Lab - [User Authentication: Identity-Aware Proxy](https://www.cloudskillsboost.google/course_templates/154/labs/532453)

Learn how to restrict access selected authenticated users with Identity-Aware Proxy without special programming. Discover how to retrieve user identity information from IAP.

* [ ] [User Authentication: Identity-Aware Proxy](../labs/User-Authentication-Identity-Aware-Proxy.md)

### Video - [IAM authorization best practices](https://www.cloudskillsboost.google/course_templates/154/video/532454)

* [YouTube: IAM authorization best practices](https://www.youtube.com/watch?v=8i28OBvoZc4)

Finally, let's use IAM to examine some best practices for authorization. For starters, it’s a smart decision to leverage and understand the resource hierarchy. Specifically: Use projects to group resources that share the same trust boundary. Check the policy granted on each resource and ensure to recognize the inheritance. Because of inheritance, use the principle of least privilege when you grant roles. Finally, audit policies by using Cloud Audit Logs and audit the memberships of groups that are used in policies. (Optional content available for use if required.) Next, we recommend granting roles to groups instead of individuals. This lets you update group memberships instead of changing an IAM policy. If you do this, make sure to audit memberships of groups used in policies and control the ownership of the Google group used in IAM policies. You can also use multiple groups to get better control. This example shows a network admin group. Some of those members also need a read_write role, which allows them to read and write to a Cloud Storage bucket, but others need the read_only role. Adding and removing individuals from all three groups controls their total access. Therefore, groups are associated with job roles and can exist for role assignment. Here are some best practices to consider when you use service accounts. Use caution when you grant the Service Account Users role, because it provides access to all the resources for which the service account has access. Also, when you create a service account, give it a display name that clearly identifies its purpose. Ideally use an established naming convention for your organization. And for service account keys, establish key rotation policies and methods.

### Video - [Lab Intro: IAM: Qwik Start](https://www.cloudskillsboost.google/course_templates/154/video/532455)

* [YouTube: Lab Intro: IAM: Qwik Start](https://www.youtube.com/watch?v=9ePSNZWdPJw)

Let’s get some hands-on practice using IAM. In the lab titled “ IAM: Qwik Start” you’ll learn how to assign a role to a second user and remove assigned roles associated with IAM. During this lab, you’ll: Explore editor roles. Prepare a resource for access testing. Remove project access. Add storage permissions. Verify access.

### Lab - [Cloud IAM: Qwik Start](https://www.cloudskillsboost.google/course_templates/154/labs/532456)

Google Cloud IAM unifies access  control for Cloud Platform services into a single system to present a consistent set of operations. Watch the short video <A HREF="https://youtu.be/PqMGmRhKsnM">Manage Access Control with Google Cloud IAM</A>.

* [ ] [Cloud IAM: Qwik Start](../labs/Cloud-IAM-Qwik-Start.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/154/quizzes/532457)

#### Quiz 1.

> [!important]
> **Which IAM role is the most broad in scope?**
>
> * [ ] Custom
> * [ ] Predefined
> * [ ] Basic

#### Quiz 2.

> [!important]
> **When a customer moves an application to Google Cloud, which one of the following does the customer remain responsible for?**
>
> * [ ] Physical security
> * [ ] Data security
> * [ ] Disk encryption
> * [ ] Network integrity

#### Quiz 3.

> [!important]
> **With which encryption option does a customer encrypt data before sending it to Google Cloud?**
>
> * [ ] Customer-managed encryption keys (CMEK)
> * [ ] Client-side encryption
> * [ ] Google encryption by default
> * [ ] Customer-supplied encryption Keys (CSEK)

#### Quiz 4.

> [!important]
> **At which level of Google Cloud's infrastructure security will you find intrusion detection?**
>
> * [ ] The storage services level
> * [ ] The hardware infrastructure level
> * [ ] The operational security level
> * [ ] The internet communication level

### Video - [Summary](https://www.cloudskillsboost.google/course_templates/154/video/532458)

* [YouTube: Summary](https://www.youtube.com/watch?v=FfOCZIi-ZGo)

This brings us to the end of the sixth module of the Google Cloud Computing Foundations course. Let’s do a quick summary. You started by outlining how security is administered in Google Cloud, and this includes the shared security model, which describes the different responsibilities of the customer and Google Cloud. After that, you explored the different encryption options with Google Cloud. The list includes Google Cloud default encryption, customer-managed encryption keys (CMEK), customer-supplied encryption keys, and local data encryption. And finally, you identified best practices when configuring authentication and authorization by using Identity and Access Management (IAM).

### Document - [Demonstrate your capabilities further!](https://www.cloudskillsboost.google/course_templates/154/documents/532459)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
