---
id: 523
name: 'Deploy and Monitor in Google Cloud for AWS Professionals'
type: Course
url: https://www.cloudskillsboost.google/course_templates/523
date_published: 2023-09-21
topics:
  - Deployment
---

# [Deploy and Monitor in Google Cloud for AWS Professionals](https://www.cloudskillsboost.google/course_templates/523)

**Description:**

This is the fourth course of a four-course series for cloud architects and engineers with existing AWS knowledge. It compares Google Cloud and AWS solutions and guides professionals on their use.

This course focuses on deploying and monitoring applications in Google Cloud. The learners apply the knowledge of monitoring and application deployment processes in AWS to explore the differences with Google Cloud. Learners get hands-on practice building and managing Google Cloud resources.

**Objectives:**

* Describe use cases for Cloud Source Repositories and Cloud Functions.
* Create charts, alerts, and uptime checks for resources with Cloud Monitoring.
* Compare Cloud Monitoring with Amazon CloudWatch.
* Describe how Cloud Run differs from AWS Fargate
* Deploy a containerized application on Cloud Run.

## Applications in the Cloud

In this module, you will explore Google Cloud services for deploying applications by considering these questions: How do you store, organize, and rapidly deploy your code? How do you perform automated actions in response to triggers in a distributed fashion? How can you run fully-fledged applications without worrying about scalability or uptime? You will learn about using Cloud Source Repositories, Cloud Functions, and Cloud Run. You will also compare Cloud Functions to AWS Lambda and Cloud Run to AWS Fargate.

### Document - [Course Introduction](https://www.cloudskillsboost.google/course_templates/523/documents/410213)

### Link - [Applications in Google Cloud](https://www.cloudskillsboost.google/course_templates/523/documents/410214)

* [Applications in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-T-INFRAWS4-I-MODULE01&utm_medium=aRT-clicks&utm_campaign=T-INFRAWS4-I-MODULE01&destination=T-INFRAWS4-I-MODULE01&url=https://storage.googleapis.com/cloud-training/T-INFRAWS4-I/1.0.1/od/en/web/MODULE01/content/index.html)

### Lab - [Hello Cloud Run [APPRUN] (AWS)](https://www.cloudskillsboost.google/course_templates/523/labs/410215)

In this lab you'll learn how to get started with Cloud Run by deploying and running a stateless container serverless-ly (with the infrastructure abstracted away).

* [ ] [Hello Cloud Run [APPRUN] (AWS)](../labs/Hello-Cloud-Run-[APPRUN]-(AWS).md)

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/523/quizzes/410216)

#### Quiz 1.

> [!important]
> **Where can Cloud Run pull container images from?**
>
> * [ ] Artifact Registry
> * [ ] Any self-hosted registry
> * [ ] Docker Hub
> * [ ] GitHub

#### Quiz 2.

> [!important]
> **You use AWS Elastic Beanstalk to autoscale your container application in response to HTTP traffiC: What service in Google Cloud provides you similar compute functionality?What is one of the key differences about AWS Elastic Beanstalk and Cloud Run?**
>
> * [ ] AWS Elastic Beanstalk does not require user configuration to support HTTPS endpoints.
> * [ ] Cloud Run cannot scale to meet demand without any user interaction
> * [ ] AWS Elastic Beanstalk requires the user to configure scaling targets.
> * [ ] Cloud Run cannot scale to zero when the application is not receiving requests

#### Quiz 3.

> [!important]
> **What is the advantage of using Cloud Functions for event-driven components of your application?**
>
> * [ ] Cloud Functions process is free of charge.
> * [ ] Cloud Functions eliminates the need to use a separate service to trigger application events.
> * [ ] Cloud Functions handles scaling these components seamlessly.
> * [ ] Cloud Functions can be written in C++

#### Quiz 4.

> [!important]
> **Why might a Google Cloud customer choose to use Cloud Source Repositories?**
>
> * [ ] They don't want to host their own git instance, and they want to integrate with IAM permissions.
> * [ ] They don't want to host their own git instance, and they don't want to integrate with IAM permissions.
> * [ ] They want to host and manage their own git instance, and they want to integrate with IAM permissions.
> * [ ] They want to host and manage their own git instance, and they don't want to integrate with IAM permissions.

### Document - [Module 1 Student Guide](https://www.cloudskillsboost.google/course_templates/523/documents/410217)

## Monitoring in Google Cloud

In this module, you will learn about the integrated monitoring tools provided by Google Cloud's operations suite. You will explore key features of the Google Cloud tools, focusing on metrics and Cloud Monitoring. You will also examine Google Cloud monitoring tools and metrics to maintain the performance of your Google Kubernetes Engine (GKE) clusters post deployment. Then, you will compare tools such as Cloud Monitoring and Cloud Trace to Amazon CloudWatch and AWS X-Ray.

### Link - [Monitoring in Google Cloud](https://www.cloudskillsboost.google/course_templates/523/documents/410218)

* [Monitoring in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-T-INFRAWS4-I-MODULE02&utm_medium=aRT-clicks&utm_campaign=T-INFRAWS4-I-MODULE02&destination=T-INFRAWS4-I-MODULE02&url=https://storage.googleapis.com/cloud-training/T-INFRAWS4-I/1.0/od/en/web/MODULE02/content/index.html)

### Lab - [Monitoring a Compute Engine using Ops Agent (AWS)](https://www.cloudskillsboost.google/course_templates/523/labs/410219)

In this lab you will learn how to monitor an Apache Web Server installed on a Compute Engine virtual machine (VM) instance using Ops Agent.

* [ ] [Monitoring a Compute Engine using Ops Agent (AWS)](../labs/Monitoring-a-Compute-Engine-using-Ops-Agent-(AWS).md)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/523/quizzes/410220)

#### Quiz 1.

> [!important]
> **You are ingesting GKE metrics into Cloud Monitoring. What is the prefix that helps you to identify the GKE system metrics?**
>
> * [ ] GKE.io
> * [ ] Pod.io
> * [ ] kubernetes.io
> * [ ] helm.io

#### Quiz 2.

> [!important]
> **AWS X-Ray lets you report on latency to manage performance of your AWS applications. What Google Cloud service can you use to report on latency for your applications in Google Cloud?**
>
> * [ ] Cloud Trace
> * [ ] Cloud Logging
> * [ ] Cloud Monitoring
> * [ ] Cloud Profiler

#### Quiz 3.

> [!important]
> **What type of GKE metrics provides information about CPU utilization?**
>
> * [ ] Managed Service for Prometheus
> * [ ] Control plan metrics
> * [ ] System metrics
> * [ ] Workload metrics

#### Quiz 4.

> [!important]
> **Google Cloud's operations suite integrates several technologies, including monitoring, logging, error reporting, and debugging, that are commonly implemented in other environments as separate solutions using separate products. What are key benefits of integration of these services?**
>
> * [ ] Reduces over head, reduces noise, streamlines use, and fixes problems faster
> * [ ] Better for Google Cloud only so long as you don't need to monitor other applications or clouds
> * [ ] Detailed control over the connections between the technologies
> * [ ] Ability to replace one tool with another from a different vendor

#### Quiz 5.

> [!important]
> **In AWS, you use Amazon CloudWatch to define alarms that notify you when health checks on your AWS resources fail. Which product can you use in Google Cloud to define similar alerts for your Google Cloud resources?**
>
> * [ ] Cloud Trace
> * [ ] Cloud Logging
> * [ ] Cloud Monitoring
> * [ ] Cloud Profiler

### Document - [Module 2 Student Guide](https://www.cloudskillsboost.google/course_templates/523/documents/410221)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
