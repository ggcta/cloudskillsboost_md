---
id: 521
name: 'Google Cloud Storage and Containers for Azure Professionals'
datePublished: 2023-09-25
topics:
- Data Lake
- GKE
type: Course
url: https://www.cloudskillsboost.google/course_templates/521
---

# [Google Cloud Storage and Containers for Azure Professionals](https://www.cloudskillsboost.google/course_templates/521)

**Description:**

This is the third course of a four-course series for cloud architects and engineers with existing Azure knowledge. It compares Google Cloud and Azure solutions and guides professionals on their use.

This course focuses on storage options and containers in Google Cloud. The learners apply the knowledge of storage and containers in Azure to explore how they differ from Google Cloud. Learners get hands-on practice building and managing Google Cloud resources.

**Objectives:**

- Create and configure Cloud SQL and Cloud Storage.
- Compare Cloud SQL to Azure SQL.
- Compare Google Cloud’s data lake options with Azure.
- Explain how Google Kubernetes Engine (GKE) differs from Azure Kubernetes Service (AKS).
- Provision a Kubernetes cluster by using GKE.

## Storage in Google Cloud

In this module, you will learn about core storage options in Google Cloud and the use cases for each. You will examine the similarities and differences between Azure Blob Storage and Cloud Storage, Azure SQL and Cloud SQL, and the data lake services in both platforms.

### Link - [Storage in Google Cloud](https://www.cloudskillsboost.google/course_templates/521/documents/411231)

- [Storage in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-MODULE01&utm_medium=aRT-clicks&utm_campaign=MODULE01&destination=MODULE01&url=https://storage.googleapis.com/cloud-training/T-INFRAZR3-I/1.0.1/od/en/web/MODULE01/Storage_in_Google_Cloud/content/index.html)

### Lab - [Cloud Storage (Azure)](https://www.cloudskillsboost.google/course_templates/521/labs/411232)

In this lab you create and use Cloud Storage buckets and exercise many of the advanced features including restricting access with Access Lists, implementing version control, loading and managing your own encryption keys, directory synch and more.

- [ ] [Cloud Storage (Azure)](../labs/Cloud-Storage-(Azure).md)

### Link - [Database services in Google Cloud](https://www.cloudskillsboost.google/course_templates/521/documents/411233)

- [Database services in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-MODULE01&utm_medium=aRT-clicks&utm_campaign=MODULE01&destination=MODULE01&url=https://storage.googleapis.com/cloud-training/T-INFRAZR3-I/1.0.1/od/en/web/MODULE01/Database_services_in_Google_Cloud/content/index.html)

### Lab - [Implementing Cloud SQL (Azure)](https://www.cloudskillsboost.google/course_templates/521/labs/411234)

In this lab you create a Cloud SQL instance and a client VM instance.  Then configure encrypted access using SSL certificates.

- [ ] [Implementing Cloud SQL (Azure)](../labs/Implementing-Cloud-SQL-(Azure).md)

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/521/quizzes/411235)

#### Quiz 1.

> [!important]
> **In your Azure environment, you have set up an Azure SQL database. To authorize connections, you have set up VNet firewall rules. You have been asked to set up a Cloud SQL database of an equivalent size. You want to use a Google-recommended method to authorize connections in a Cloud SQL database. What should you do?**
>
> - [ ] Use VPC firewalls.
> - [ ] Authorize networks by adding IP addresses to an denylist.
> - [ ] Encrypt the data.
> - [ ] Create a replica in Cloud SQL.

#### Quiz 2.

> [!important]
> **In your current Azure environment, you have blobs stored in a container, which is owned by an Azure account. You need to move these files to Cloud Storage. Which option describes the hierarchy in Google Cloud?**
>
> - [ ] Project -> Bucket -> Object
> - [ ] Project -> Object -> Bucket
> - [ ] Object -> Bucket -> Project
> - [ ] Bucket -> Project -> Object

#### Quiz 3.

> [!important]
> **You have a requirement to serve media files. Which is the best storage option?**
>
> - [ ] Filestore
> - [ ] Cloud Storage
> - [ ] Cloud Spanner
> - [ ] Cloud SQL

#### Quiz 4.

> [!important]
> **In your Azure environment, you are using Azure Synapse Analytics, Azure Data Factory, and Azure Data Lake Gen 2 to analyze structured and unstructured data. You need to set up a data lake environment using Google Cloud. As part of this requirement, you have opted to choose a low-code, no code solution similar to Azure Data Factory. Which option can you use to load data?**
>
> - [ ] Compute Engine
> - [ ] Cloud Storage
> - [ ] Cloud Data Fusion
> - [ ] Dataflow

### Document - [Module 1 Student Guide (Storage in Google Cloud)](https://www.cloudskillsboost.google/course_templates/521/documents/411236)

### Document - [Module 1 Student Guide (Database services in Google Cloud)](https://www.cloudskillsboost.google/course_templates/521/documents/411237)

## Containers in Google Cloud

In this module, you will learn how Google Kubernetes Engine (GKE) and Anthos let you orchestrate containers in Google Cloud and in hybrid or multi-cloud environments. You will examine key concepts related to containers and Kubernetes, and explore concepts specific to GKE and the similarities and differences with Azure Kubernetes Service (AKS). Additionally, you will examine how to create and update Deployments to support your workloads in GKE. You will also learn about the purpose of Anthos and how it provides consistent container orchestration across GKE and on-premises environments.

### Link - [GKE Concepts and Architecture](https://www.cloudskillsboost.google/course_templates/521/documents/411238)

- [GKE Concepts and Architecture](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-MODULE02&utm_medium=aRT-clicks&utm_campaign=MODULE02&destination=MODULE02&url=https://storage.googleapis.com/cloud-training/T-INFRAZR3-I/1.0.1/od/en/web/MODULE02/GKE_concepts_and_architecture/content/index.html)

### Lab - [Google Cloud Fundamentals: Getting Started with GKE (Azure)](https://www.cloudskillsboost.google/course_templates/521/labs/411239)

In this lab you create a Google Kubernetes Engine cluster containing several containers, each containing a web server. You place a load balancer in front of the cluster and view its contents.


- [ ] [Google Cloud Fundamentals: Getting Started with GKE (Azure)](../labs/Google-Cloud-Fundamentals-Getting-Started-with-GKE-(Azure).md)

### Lab - [Deploying Google Kubernetes Engine (Azure)](https://www.cloudskillsboost.google/course_templates/521/labs/411240)

Architecting with Google Kubernetes Engine: Creating a GKE Cluster via Google Cloud Console

- [ ] [Deploying Google Kubernetes Engine (Azure)](../labs/Deploying-Google-Kubernetes-Engine-(Azure).md)

### Link - [Deployments in Kubernetes](https://www.cloudskillsboost.google/course_templates/521/documents/411241)

- [Deployments in Kubernetes](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-MODULE02&utm_medium=aRT-clicks&utm_campaign=MODULE02&destination=MODULE02&url=https://storage.googleapis.com/cloud-training/T-INFRAZR3-I/1.0.1/od/en/web/MODULE02/Deployments_in_Kubernetes/content/index.html)

### Lab - [Creating Google Kubernetes Engine Deployments (Azure)](https://www.cloudskillsboost.google/course_templates/521/labs/411242)

Architecting with Google Kubernetes Engine: Creating Kubernetes Engine Deployments

- [ ] [Creating Google Kubernetes Engine Deployments (Azure)](../labs/Creating-Google-Kubernetes-Engine-Deployments-(Azure).md)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/521/quizzes/411243)

#### Quiz 1.

> [!important]
> **What is the purpose of the Deployment object in Kubernetes?**
>
> - [ ] To group nodes within a cluster that all have the same configuration.
> - [ ] To launch one or more Pods and ensure that a specified number of them successfully run to completion and exit.
> - [ ] To ensure that a defined set of Pods is running at any given time.
> - [ ] To launch one or more Pods on a time-based schedule.

#### Quiz 2.

> [!important]
> **How do Pods within the same node communicate with one another?**
>
> - [ ] Through service mesh
> - [ ] Using the node's VM network interface controller
> - [ ] Using a shared Alias IP address
> - [ ] Through the node networking namespace

#### Quiz 3.

> [!important]
> **What is one benefit of Anthos?**
>
> - [ ] You can enable automatic A/B testing before updating Deployments.
> - [ ] You can use the same configurations for on-premises and GKE clusters.
> - [ ] You can use Anthos Service Mesh to manage and secure microservices using VPC peering.
> - [ ] You receive additional IP address ranges for cluster-wide Services in your VPC network.

#### Quiz 4.

> [!important]
> **In Azure Kubernetes Services, a cluster has at least one node which is an Azure Virtual Machine. In Google Cloud, where do the compute resources come from that are used to build Google Kubernetes Engine clusters?**
>
> - [ ] Cloud Run
> - [ ] Compute Engine
> - [ ] Cloud Storage
> - [ ] Bare-metal servers

### Document - [Module 2 Student Guide (GKE Concepts and Architecture)](https://www.cloudskillsboost.google/course_templates/521/documents/411244)

### Document - [Module 2 Student Guide (Deployments in Kubernetes)](https://www.cloudskillsboost.google/course_templates/521/documents/411245)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
