---
id: 559
name: 'Developing Applications with Cloud Run on Google Cloud: Fundamentals'
type: Course
url: https://www.cloudskillsboost.google/course_templates/559
date: 2025-04-03
datePublished: 2024-07-26
topics:
- IAM
---

# [Developing Applications with Cloud Run on Google Cloud: Fundamentals](https://www.cloudskillsboost.google/course_templates/559)

**Description:**

This course introduces the Cloud Run serverless platform for running applications.

In this course, you learn about the fundamentals of Cloud Run, its resource model and the container lifecycle.

You learn about service identities, how to control access to services, and how to develop and test your

application locally before deploying it to Cloud Run. The course also teaches you how to integrate

with other services on Google Cloud so you can build full-featured applications.

**Objectives:**

- Understand the fundamentals of Cloud Run that include the resource model,  container lifecycle, and autoscaling.
- Develop and test applications locally before deploying to Cloud Run.
- Use service identity and IAM with Cloud Run.
- Integrate Cloud Run applications with Google Cloud services.

## Course Introduction

Introduction to the course structure, and contents.

### Document - [Introduction to course structure and contents.](https://www.cloudskillsboost.google/course_templates/559/documents/496737)

## Fundamentals of Cloud Run

Understand the fundamentals of Cloud Run that include its resource model, and the container 

lifecycle. Learn how autoscaling works and how to control access to your Cloud Run services.

### Document - [Overview](https://www.cloudskillsboost.google/course_templates/559/documents/496738)

### Document - [Resource model](https://www.cloudskillsboost.google/course_templates/559/documents/496739)

### Document - [Container lifecycle](https://www.cloudskillsboost.google/course_templates/559/documents/496740)

### Document - [Autoscaling](https://www.cloudskillsboost.google/course_templates/559/documents/496741)

### Document - [Access control with IAM](https://www.cloudskillsboost.google/course_templates/559/documents/496742)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/559/quizzes/496743)

#### Quiz 1.

> [!important]
> **What are some characteristics of an idle container? Select four.**
>
> - [ ] An idle container can be shut down at any time.
> - [ ] An idle container does not incur charges by default.
> - [ ] An idle container can reliably perform background tasks.
> - [ ] An idle container does not service requests.
> - [ ] An idle container has its CPU throttled.

#### Quiz 2.

> [!important]
> **Which of these statements about autoscaling in Cloud Run are correct? Select three.**
>
> - [ ] When the number of requests to a service decreases, Cloud Run reduces the number of container instances.
> - [ ] In Cloud Run, a container instance can receive and process only a single request at a time.
> - [ ] If there are no incoming requests to your service, by default even the last remaining container instance will be shut down.
> - [ ] Cloud Run automatically increases the number of container instances of a service revision when necessary.
> - [ ] As your service receives requests, the number of active instances might decrease and the number of idle instances increase.

#### Quiz 3.

> [!important]
> **How can you make a Cloud Run service publicly accessible and invokable without authentication?**
>
> - [ ] Use the –-allow-unauthenticated option when you deploy the service to Cloud Run.
> - [ ] A Cloud Run service is publicly accessible and can be invoked without authentication by default.
> - [ ] A Cloud Run service cannot be invoked publicly.

#### Quiz 4.

> [!important]
> **What are some characteristics of Cloud Run services? Select three.**
>
> - [ ] Each deployment of your application container image to Cloud Run creates a service revision.
> - [ ] Cloud Run automatically scales a service revision.
> - [ ] Cloud Run services are regional Google Cloud resources.
> - [ ] You must manually route requests to the latest revision of your Cloud Run service.
> - [ ] A service revision can be modified or updated.

#### Quiz 5.

> [!important]
> **Which of these statements about Cloud Run are correct? Select three.**
>
> - [ ] Cloud Run is serverless.
> - [ ] You cannot access internal Google Cloud resources in your network from Cloud Run.
> - [ ] To access a service on Cloud Run, you must manually provision an HTTP endpoint.
> - [ ] Cloud Run integrates with other Google Cloud services.
> - [ ] On Cloud Run, your code can either run continuously as a service, or as a job.

### Document - [Module review](https://www.cloudskillsboost.google/course_templates/559/documents/496744)

## Service Identity and Authentication

Learn how service accounts provide Cloud Run service identities, and how you can control access 

to Google APIs by implementing the principle of least privilege. Also, learn how to use secrets and 

environment variables in your applications that run on Cloud Run.

### Document - [Service accounts and identity](https://www.cloudskillsboost.google/course_templates/559/documents/496745)

### Document - [Resource hierarchy](https://www.cloudskillsboost.google/course_templates/559/documents/496746)

### Document - [Principle of least privilege](https://www.cloudskillsboost.google/course_templates/559/documents/496747)

### Lab - [Implementing Least Privilege IAM Policy Bindings in Cloud Run [APPRUN]](https://www.cloudskillsboost.google/course_templates/559/labs/496748)

This lab teaches you how to implement IAM policy bindings in Cloud Run to adhere to the security principle of least privilege.

- [ ] [Implementing Least Privilege IAM Policy Bindings in Cloud Run [APPRUN]](../labs/Implementing-Least-Privilege-IAM-Policy-Bindings-in-Cloud-Run-[APPRUN].md)

### Document - [Secrets and environment variables](https://www.cloudskillsboost.google/course_templates/559/documents/496749)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/559/quizzes/496750)

#### Quiz 1.

> [!important]
> **What are two methods of making a secret available to a Cloud Run service?**
>
> - [ ] Provide the secret as an environment variable when deploying the service.
> - [ ] Provide the secret name and value as query parameters in the request to the service.
> - [ ] Secrets cannot be accessed from a Cloud Run service.
> - [ ] Mount the secret as a volume so that the service can access the secret from a file.

#### Quiz 2.

> [!important]
> **What are some characteristics of an IAM policy? Select three.**
>
> - [ ] An IAM policy is attached to a Google Cloud resource.
> - [ ] An IAM policy consists of at most one policy binding that binds a member to one or more roles.
> - [ ] You can attach only one IAM policy to a resource.
> - [ ] A member can only have a single role in an IAM policy.
> - [ ] An IAM policy consists of a list of policy bindings that binds members to roles.

#### Quiz 3.

> [!important]
> **Which statements about using environment variables with Cloud Run are correct? Select two.**
>
> - [ ] Environment variables set in the container with the ENV statement in a Dockerfile take precedence over variables with the same name set on a Cloud Run service or job.
> - [ ] Once set, the value of an environment variable cannot be updated.
> - [ ] Environment variables are key-value pairs that can be set when deploying a Cloud Run service or job.
> - [ ] Environment variables are injected into your application container and accessed by your code at runtime.

#### Quiz 4.

> [!important]
> **How can you implement the principle of least privilege for a Cloud Run service?**
>
> - [ ] Remove the Editor role on the default service account that is used by Cloud Run.
> - [ ] Use only Google client libraries to access Google Cloud APIs and services.
> - [ ] Create a new service account and configure it as the Cloud Run service's identity. Grant minimal permissions to the account on the resources that the service needs to access.
> - [ ] Use secrets to store data that is needed by the Cloud Run service.

#### Quiz 5.

> [!important]
> **Every Cloud Run service is linked to a service account by default. What role is given to this service account?**
>
> - [ ] Viewer
> - [ ] Owner
> - [ ] Billing Admin
> - [ ] Editor

### Document - [Module review](https://www.cloudskillsboost.google/course_templates/559/documents/496751)

## Application Development, Testing, and Integration

Learn how to develop and test applications to run on Cloud Run. Manage service deployments and revisions on Cloud Run, 

and learn how to integrate your Cloud Run service with other services in Google Cloud.

### Document - [Development and testing](https://www.cloudskillsboost.google/course_templates/559/documents/496752)

### Document - [Managing service deployments and revisions](https://www.cloudskillsboost.google/course_templates/559/documents/496753)

### Document - [Integrating with Google Cloud services](https://www.cloudskillsboost.google/course_templates/559/documents/496754)

### Lab - [Using Cloud PubSub with Cloud Run [APPRUN]](https://www.cloudskillsboost.google/course_templates/559/labs/496755)

In this lab you will learn how Cloud Pub/Sub can be used with Cloud Run.

- [ ] [Using Cloud PubSub with Cloud Run [APPRUN]](../labs/Using-Cloud-PubSub-with-Cloud-Run-[APPRUN].md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/559/quizzes/496756)

#### Quiz 1.

> [!important]
> **Which of these statements regarding service revisions in Cloud Run are correct? Select two.**
>
> - [ ] In Cloud Run, only the newest or latest service revision can receive and process requests to the service.
> - [ ] A revision is created when you update the configuration of a service in Cloud Run.
> - [ ] You cannot control the amount of request traffic received by a service revision.
> - [ ] A revision is created when you deploy a container image to a service in Cloud Run.

#### Quiz 2.

> [!important]
> **What are some characteristics of applications that are a good fit for Cloud Run? Select three.**
>
> - [ ] When run as a service, the application listens for HTTP requests on a specified port.
> - [ ] The application depends on a local persistent file system.
> - [ ] When run as a service, the application responds to a request within a specified time.
> - [ ] The application is containerized.

#### Quiz 3.

> [!important]
> **To integrate a Cloud Run service with other Google Cloud APIs and resources, what are some steps you should take? Select three.**
>
> - [ ] Use the default runtime service account to access Google Cloud APIs and resources from a Cloud Run service.
> - [ ] To connect to internal cloud resources from your Cloud Run service, use Serverless VPC Access.
> - [ ] Use Secret Manager to store credentials required by downstream database services.
> - [ ] Connect to Google Cloud services from your Cloud Run service using client libraries.

#### Quiz 4.

> [!important]
> **What are some products or services that you can use to build containers? Select three.**
>
> - [ ] Cloud Build
> - [ ] Cloud Run
> - [ ] Docker
> - [ ] Artifact Registry

### Document - [Module review](https://www.cloudskillsboost.google/course_templates/559/documents/496757)

## Course Review

Review the topics discussed in the course.

### Document - [Review course topics](https://www.cloudskillsboost.google/course_templates/559/documents/496758)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
