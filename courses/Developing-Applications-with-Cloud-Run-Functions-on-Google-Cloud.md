---
id: 505
name: 'Developing Applications with Cloud Run Functions on Google Cloud'
type: Course
url: https://www.cloudskillsboost.google/course_templates/505
date_published: 2024-11-04
topics:
  - Deployment
  - FaaS
---

# [Developing Applications with Cloud Run Functions on Google Cloud](https://www.cloudskillsboost.google/course_templates/505)

**Description:**

In this course, you learn about Cloud Run functions, Google's serverless, fully-managed functions as a service (FaaS) product that lets you implement single-purpose function code that reponds to HTTP requests and events from your cloud infrastructure.

**Objectives:**

* Recognize the benefits of and use cases for Cloud Run functions in modern application development.
* Understand how to build, test and deploy Cloud Run functions.
* Secure and connect Cloud Run functions to resources, and cloud databases.
* Use best practices with Cloud Run functions.

## Course Introduction

Introduction to the course content.

### Video - [Course Introduction](https://www.cloudskillsboost.google/course_templates/505/video/513258)

* [YouTube: Course Introduction](https://www.youtube.com/watch?v=7vbjfXBm45c)

Cloud Run functions is an event-driven, serverless compute platform. Learn how to use Cloud Run functions to create and scale event driven-apps in the Developing Applications with Cloud Run Functions on Google Cloud course. Hi everyone, I’m Hansel, a Technical Curriculum Developer at Google Cloud. In this course, you learn about Cloud Run functions, Google's serverless, fully-managed functions as a service product that lets you implement single-purpose function code that responds to HTTP requests and events from your cloud infrastructure. This course is for application developers, cloud architects, and cloud developers, and other individuals that are looking to learn about Cloud Run functions and improve their application development skills on Google Cloud. Through a series of video lectures and hands-on labs, you learn about Cloud Run functions, and recognize their benefits and use cases in modern application development. Upon completion of the course, you will understand how to build, test, and deploy Cloud Run functions. In addition, you will learn how to secure and connect Cloud Run functions to resources and cloud databases, and use best practices with functions. Let’s get started!

## Introduction to Cloud Run Functions

An introduction to Cloud Run functions, what they are, and their benefits and use cases.

### Video - [An introduction to Cloud Run functions](https://www.cloudskillsboost.google/course_templates/505/video/513259)

* [YouTube: An introduction to Cloud Run functions](https://www.youtube.com/watch?v=4z9LjMvd8h4)

Welcome to the first module of this course on Cloud Run functions. In this module, we introduce Cloud Run functions and discuss their features, and benefits. We also review some of the use cases for Cloud Run functions, and do a lab to create your first function in the Google Cloud console. In this module, you learn about Cloud Run functions, their features and benefits, and their use cases. We’ll discuss the supported language runtimes and regions for deploying Cloud functions, and how they’re built and deployed on Google Cloud. You’ll also complete a lab to develop and deploy Cloud Run functions from the Google Cloud console and the gcloud CLI. Finally, we review what was discussed in this module. Let’s start by first discussing what are Cloud Run functions. Cloud Run functions is a fully managed serverless execution environment on Google Cloud for you to build, deploy, and run functions. It is a scalable functions-as-a-service platform, where there is no need to provision any infrastructure or manage individual servers. Depending on your requirements, you can connect to other cloud services from Cloud Run functions. It’s fully integrated with Cloud Cloud Observability for observability and diagnosis. There are two versions of Cloud Run functions: Cloud Run functions, formerly known as Cloud Functions (2nd generation), which deploys your functions as services on Cloud Run, allowing you to trigger them using Eventarc and Pub/Sub. Cloud Run functions (1st generation), formerly known as Cloud Functions (1st generation), the original version of functions with limited event triggers and configurability. See Cloud Run functions version comparison for more information. Cloud Run is a managed compute platform that lets you run containers directly on top of Google's scalable infrastructure. You can deploy code written in any programming language on Cloud Run if you can build a container image from it. You can use the source-based deployment option that builds the container for you, when developing your application in Go, Node.js, Python, Java, . NET Core, or Ruby. Cloud Run works well with other services on Google Cloud, so you can build full-featured applications without spending too much time operating, configuring, and scaling your Cloud Run service. A cloud function is simple code that you write that serves a single piece of functionality. It’s triggered by an event that is generated by cloud infrastructure and other services. Cloud functions execute in a fully managed serverless environment. You can develop Cloud functions in any supported language. Cloud Run functions provides a connective layer of logic that lets you write code to connect and extend cloud services. For example, a Cloud function can respond to a file upload to Cloud Storage, or an incoming message on a Pub/Sub topic. To set up and use Cloud Run functions, you: Develop the function code or logic in one of the supported programming languages. Deploy the function. You can deploy the function using the Google Cloud console or the gcloud CLI. Set up a trigger for the function to execute in response to HTTP requests or supported cloud events. Let’s now discuss the features and benefits of Cloud Run functions, and the use cases for deploying them. Here are some of the features and benefits of using Cloud Run functions. Features of Cloud Run functions include: Local development and testing: You can develop and test functions in a local development environment before deploying to Cloud Run functions. Seamlessly authenticate your cloud functions with other Google Cloud services using service accounts. HTTP and event-driven: Cloud Run functions execute in response to cloud events and HTTP requests. Integration with Cloud SQL, Bigtable, Spanner, and Firestore databases. Portability: A function can run in any standard runtime environment for one of the supported languages. Benefits of Cloud Run functions include: Augmenting and extending existing cloud services with programming logic. Serverless. The software and infrastructure are fully managed by Google. You don’t need to manage servers, update frameworks, or patch operating systems. Autoscaling. Resources are automatically provisioned in response to events. A function can scale from a few invocations a day to many millions of invocations without requiring any additional work. Observable. Cloud Run functions are integrated with Google Cloud Observability monitoring and logging tools for observability and error diagnosis. Pricing. A pay as you go pricing model is used. The cost is based on the number of function invocations, how long the function runs (compute time), and any data transfer fees for outbound network traffic. There are two types of Cloud Run functions: HTTP functions, which handle HTTP requests, and Event-driven functions, which handle events from your cloud environment. Use HTTP functions with HTTP triggers when you want to invoke a function with an HTTP(S) request. When you specify an HTTP trigger for a function, the function is assigned a URL at which it can receive requests. An HTTP trigger enables a function to run in response to HTTP(S) requests. A good use case for using HTTP functions is to implement a webhook or API that handles http requests from other services. By default, requests to HTTP functions require authentication. You can choose to allow unauthenticated requests during function deployment. We discuss securing Cloud Run functions in more detail in a later module of this course. To implement an HTTP function, you write an HTTP handler function and register it with the functions framework for your programming language. The handler accepts the request and response arguments, processes the request based on the request method, and sends back an HTTP response. If the function creates any background tasks like threads, processes, or Promise objects, they must be terminated before the response is sent. Use event-driven functions when you want a function to be invoked automatically in response to an event that occurs in your cloud environment. You implement event-driven functions using CloudEvent functions or Background functions depending on your chosen language runtime, and if you’re using Cloud Run functions or Cloud Run functions (1st generation). Event-driven functions use event triggers which react to events within your Google Cloud project. Event triggers are supported by many Google Cloud services based on if the cloud function is from Cloud Run functions or Cloud Run functions (1st generation). You can use event triggers for: Pub/Sub, Cloud Storage, Firestore, Firebase, and Eventarc sources. You can also integrate Cloud Run functions with any other Google Cloud service that supports Pub/Sub as an event bus. We discuss triggers in more detail in a later module of this course. Event-driven functions are executed in response to an event like receipt of a new Pub/Sub message or deletion of a file in Cloud Storage. You implement an event-driven function as a CloudEvent function or a Background function. CloudEvent functions are: Based on the CloudEvents industry standard specification for describing event data. Registered with the Functions Framework, an open source library that wraps user functions within a persistent HTTP application. Used by Cloud Run functions with all language runtimes. Used by Cloud Run functions (1st generation) with . NET, Ruby, and PHP. Background functions are: Older style event-driven functions that receive event data based on the type of event. Used by Cloud Run functions (1st generation) with Node.js, Python, Go, and Java runtimes. Cloud Run functions have the following features: Function instances with up to 32 GB of RAM and 4 vCPUs. Process up to 1000 concurrent requests with a single function instance. This capability reduces cold starts and improves overall latency when scaling. Run time limit of up to 60 minutes for HTTP functions, and up to 10 minutes for event-driven functions to process longer request workloads. With a new revision created every time you deploy your function, you can split traffic between different revisions or rollback your function to a prior revision. Leverage Cloud Run’s scalable container platform to move your function to Cloud Run or to Kubernetes. With Eventarc, event-driven functions can be triggered from more than 90 Google, external SaaS event sources, and custom sources by publishing to Pub/Sub. With the industry-standard CloudEvents format, you can simplify your event handling code. In Google Cloud console configure your function’s triggers, track deployments, and test your functions, and view function metrics. View the documentation on the comparison between Cloud Run functions and Cloud Run functions 1st generation. Some of the use cases for Cloud Run functions include: Data processing By responding to Cloud Storage events on files and objects, you can validate and transform data, process images and videos for further downstream processing. Webhooks and APIs With HTTP functions, you can support webhook and API calls that originate from external systems by processing HTTP requests. Mobile device backend that responds to events triggered by Firebase. With Cloud Run functions, you can develop mobile device backend services that responds to events triggered by Firebase and Firestore. IoT You can develop IoT (internet-of-things) applications with Cloud Run functions by processing and storing data from devices streamed into Pub/Sub. In this section, we discuss the language runtimes and regions supported by Cloud Run functions. You can develop Cloud Run functions in any of these supported languages. There are specific versions of each language runtime that is supported. Please refer to the Cloud Run functions documentation for the version numbers. The language runtime that you choose and the type of function that you want to write determine the structure of your code and function implementation. For Cloud Run functions to locate your function definition, each language runtime has specific requirements for structuring your source code. Here are the basic directory structures for some of the languages. For Node.js, by default, Cloud Run functions loads source code from a file named index.js at the root of your function directory. To specify a different main source file, use the main field in your package.json file. The package.json file also includes the Functions Framework for Node.js as a dependency, along with any additional library dependencies needed by your function. For Python, Cloud Run functions loads source code from a file named main.py at the root of your function directory. The requirements.txt file also includes the Functions Framework for Python as a dependency and any additional library dependencies needed by your function. For Go, your function must be in a Go package at the root of your project. The go.mod file includes the Functions Framework for Go as a dependency, and any additional library dependencies needed by your function. For more details on creating your source code directory structure for your preferred language, refer to the Cloud Run functions documentation. The function entry point is the code that is executed when the Cloud Run function is invoked. Your source code must define an entry point for your function and must be defined in your main file or root package. Depending on the programming language, the entry point is a function or a class. You specify this entry point when you deploy your function. The infrastructure that runs Cloud Run functions is located in a specific region and is managed by Google to be redundantly available across all the zones within that region. When selecting a region to run your Cloud Run functions, your primary considerations should be latency and availability. You can generally select the region closest to your Cloud Run function's users, but you should also consider the location of the other Google Cloud products and services that your app uses. Using services across multiple locations can affect your app's latency, and pricing. Cloud Run functions and Cloud Run functions 1st generation, have different regional availability.

### Video - [Deploying Cloud Run functions](https://www.cloudskillsboost.google/course_templates/505/video/513260)

* [YouTube: Deploying Cloud Run functions](https://www.youtube.com/watch?v=yNIHL5XXD4I)

Let’s review the process to build and deploy Cloud Run functions from source code. The deployment process takes your function source code and configuration settings and builds a runnable image. Cloud Run functions automatically manages the image in order to handle requests to your function. A user deploying Cloud Run functions must have the Cloud Functions Developer IAM role or a role that includes the same permissions. To deploy Cloud Run functions, a user must also be assigned the Service Account User IAM role on the Cloud Run functions runtime service account. You can deploy your function from the Google Cloud console, using Cloud Build, using Cloud Code, or with the gcloud CLI. To deploy Cloud Run functions, specify the gen2 flag. The region flag specifies the region in which to deploy your function. The runtime flag specifies the language runtime of your function. The source flag specifies the location of your function source code. The function can be located on your local machine, in Cloud Storage, or in a source repository. Specify a function or class name in your source code as the entry point of your cloud function with the entry-point flag. The function or class code is executed when your function runs. Cloud Code is a tool that simplifies the development and deployment of Cloud Run functions. It allows you to create, deploy, and invoke functions directly within your IDE, making the process more efficient. To specify the type of trigger and related configuration for your function, provide trigger flags. Refer to the gcloud functions deploy command documentation for more details. You can specify the location of your function source code for deployment with the source flag. You can deploy your function from a local machine. The value of the source flag is a local file system path to the root directory of the function source code. Optionally, use the stage-bucket flag to specify a Cloud Storage bucket to upload your source code to as part of deployment. You can exclude unnecessary files with the . gcloudignore file. Cloud Storage. The value of the source flag is the cloud storage path to the bucket that contains the function source code packaged as a zip file. Your function source files must be located at the root of the zip file. In Cloud Run functions (1st generation), the account performing the deployment needs permission to read from the bucket. In Cloud Run functions, the Cloud Run functions service agent needs permission to read from the bucket. A source repository. The value of the source flag is a source repository reference to the location of your function source code. You can deploy your function source code from a revision in your repository by specifying revisions/revision name in the source repository path. To specify the location of the source code other than the repository root, append the paths/source_directory_path to the source repository path. The Cloud Run functions service agent must have the Source Repository Reader (roles/source.reader) IAM role on the repository. Deploying from Cloud Source Repositories also enables you to deploy code hosted in a GitHub or Bitbucket repository. You can also write and deploy a function directly from the Google Cloud console using the provided inline editor. The editor contains a left pane to view and select source files and the right pane to edit a source file. Let’s review the build process for Cloud Run functions. When you deploy your function's source code to Cloud Run functions, that source is stored in a Cloud Storage bucket. Cloud Build is a service that executes builds on Google Cloud infrastructure. Cloud Build automatically builds your function source code into a container image, and pushes that image to Artifact Registry. Cloud Run functions then accesses this image when it needs to run the container to execute your function. The process of building the image is entirely automatic and requires no direct input from you. The Cloud Build API must be enabled for your project. All the resources used in the build process execute in your own user project, and you have access to all the build logs through Cloud Logging. Cloud Run functions uses Artifact Registry to store the images built from your function source code. Artifact Registry is a service that is used to store and manage software artifacts in private repositories, including container images, and language packages. Artifact Registry integrates with Cloud Build to store the packages from your builds.

### Video - [Lab Intro: Develop and Deploy Cloud Run Functions](https://www.cloudskillsboost.google/course_templates/505/video/513261)

* [YouTube: Lab Intro: Develop and Deploy Cloud Run Functions](https://www.youtube.com/watch?v=IcIrrlcDICo)

Let’s now do a lab to develop and deploy Cloud Run functions. In this lab, you create and deploy simple Cloud Run functions with the Google Cloud console and the gcloud CLI. You’ll first write a HTTP function to process and respond to HTTP requests, and deploy the function in Google Cloud console to Cloud Run functions. Next, you’ll write an event-driven function to respond to Cloud Storage events, when a file is copied to a Cloud Storage bucket. You’ll deploy this function using the gcloud CLI. When developing functions, it’s a good practice to develop unit tests for your function before deploying them. In this task in the lab, you write unit tests for your function and test them locally before deploying the function. Cloud Run functions support multiple deployed revisions of a function. In this task in the lab, you deploy more than one revision of a function and split traffic between the two revisions.

### Lab - [Develop and Deploy Cloud Run Functions](https://www.cloudskillsboost.google/course_templates/505/labs/513262)

In this lab, you will develop and deploy HTTP and event-driven Cloud Run functions.

* [ ] [Develop and Deploy Cloud Run Functions](../labs/Develop-and-Deploy-Cloud-Run-Functions.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/505/quizzes/513263)

#### Quiz 1.

> [!important]
> **An event-driven function: (Select three).**
>
> * [ ] Can only be implemented as a CloudEvent function.
> * [ ] Can be triggered from Eventarc sources.
> * [ ] Responds to events that occur in your cloud infrastructure.
> * [ ] Uses event triggers for various services like Pub/Sub, and Cloud Storage.

#### Quiz 2.

> [!important]
> **An HTTP function: (Select three).**
>
> * [ ] Can only be invoked with authentication credentials.
> * [ ] Is triggered by a request made to its URL endpoint.
> * [ ] Can be used to implement a webhook.
> * [ ] Must send back an HTTP response.

#### Quiz 3.

> [!important]
> **What are some features and benefits of using Cloud Run functions? Select four.Cloud Run functions:**
>
> * [ ] Uses a fixed pricing model.
> * [ ] Supports seamless authentication with IAM.
> * [ ] Are triggered by HTTP requests and events from Cloud Services.
> * [ ] Can be locally developed and tested.
> * [ ] Can be integrated with Cloud databases.

#### Quiz 4.

> [!important]
> **Which of these statements about Cloud Run functions are correct? Select three.Cloud Run functions:**
>
> * [ ] Can be used to extend Cloud services.
> * [ ] Can only be invoked by sending HTTP requests.
> * [ ] Require servers or VMs to be provisioned.
> * [ ] Is a scalable functions-as-a-service platform.
> * [ ] Is integrated with Cloud Logging.

### Video - [Module review](https://www.cloudskillsboost.google/course_templates/505/video/513264)

* [YouTube: Module review](https://www.youtube.com/watch?v=PI-ehi3uLjg)

Let’s review what was discussed in this module. In this module, we introduced Cloud Run functions and discussed the types of Cloud Run functions, their features and their benefits. We reviewed some of the use cases for Cloud Run functions, and completed a lab to create functions in the Google Cloud console, and with the gcloud CLI. You learned that Cloud Run functions is a fully managed, serverless, functions-as-a-service platform that enables you to create single-purpose functions that can be deployed and run on Google Cloud. You learned about the features and benefits of Cloud Run functions, that include local development and testing, integration with Cloud databases, and auto-scalability. And about some of their use cases, that include webhooks and APIs, and data processing. We reviewed the language runtimes that are supported by Cloud Run functions, and their basic directory structure requirements when developing in Node.js, Python, and Go. You learned how Cloud Run functions are built and deployed, and completed a lab on deploying Cloud Run functions from the Google Cloud console and the gcloud CLI.

## Calling and Connecting Cloud Run Functions

Learn how to trigger and call Cloud Run functions, and how to connect them in workflows and to cloud resources in your network.

### Video - [Triggering functions](https://www.cloudskillsboost.google/course_templates/505/video/513265)

* [YouTube: Triggering functions](https://www.youtube.com/watch?v=Obe0-ljTLJ4)

In this module, we’ll discuss how you can call Cloud Run functions with function triggers. You will learn about the different types of function triggers and how to use them when deploying your functions. We will also discuss how to connect Cloud Run functions to Virtual Private Cloud (VPC) networks within your cloud infrastructure. Finally, we will review connecting Cloud Run functions with workflows. We’ll first discuss Cloud Run functions triggers, then how to connect Cloud Run functions with workflows, and how to connect Cloud Run functions to resources in a VPC network. You can then put this in practice by completing an optional lab to connect Cloud Run functions to resources in a VPC network. Finally, we’ll review the topics that were discussed in this module. Let’s get started with Cloud Run functions triggers. You set up Cloud Run functions to execute in response to various scenarios by specifying a trigger for your function. Triggers can be HTTP(S) requests or one of several supported cloud events. There are two categories of triggers: HTTP triggers, which react to HTTP(S) requests, and correspond to HTTP functions, and event triggers, which react to events within your Google Cloud project, and correspond to event-driven functions. You specify triggers as part of function deployment. You can have the same event cause multiple functions to execute by deploying multiple functions with the same trigger source settings. But, you cannot bind the same function to more than one trigger at a time. With event-driven Cloud Run functions, you can create Eventarc event triggers using filters. Event filters can include the service name, method name, event type, and other information. You can create triggers with the correct event filters in the Google Cloud console or with the gcloud CLI. All event driven Cloud Run functions use Eventarc for event delivery. Eventarc supports more than 90 Google Cloud sources, including events from Cloud Audit Logs, external SaaS event sources, and custom sources by publishing to Pub/Sub. You can integrate Cloud Run functions with any other Google service that supports Pub/Sub as an event bus, for example Cloud Logging and Cloud Scheduler. This is possible because Cloud Run functions can be triggered by messages on a Pub/Sub topic. You can also use HTTP Cloud Run functions as task handlers with Cloud Tasks. Using the Gmail Push Notification API, you can send Gmail events to a Pub/Sub topic and consume them with Cloud Run functions. HTTP triggers enable a function to run in response to HTTP(S) requests. When you specify an HTTP trigger for a function, the function is assigned a URL at which it can receive requests. Cloud Run functions are assigned an HTTPS endpoint at which they can be invoked. HTTP triggers support the GET, POST, PUT, DELETE, and OPTIONS request methods. Pub/Sub triggers enable functions to be called in response to Pub/Sub messages. When you specify a Pub/Sub trigger for a function, you also specify a Pub/Sub topic. Your function will be called whenever a message is published to the specified topic. For a function to use a Pub/Sub trigger, it must be implemented as an event-driven function. If a CloudEvent function is used, the Pub/Sub event data is passed to the function in the CloudEvents format. If a Background function is used, the Pub/Sub event data is passed to function in the PubsubMessage format. In Cloud Run functions, Pub/Sub triggers are implemented as a type of Eventarc trigger. Cloud Storage triggers enable functions to be called in response to changes in Cloud Storage. When you specify a Cloud Storage trigger for a function, you choose an event type and provide a specific Cloud Storage bucket. The function will be called whenever a change occurs on an object (file) within the specified bucket. For a function to use a Cloud Storage trigger, it must be implemented as an event-driven function. If a CloudEvent function is used, the Cloud Storage event data is passed to the function in the CloudEvents format. If a Background function is used, the Cloud Storage event data is passed to the function in the StorageObjectData format. In Cloud Run functions, Cloud Storage triggers are implemented as a type of Eventarc trigger. Firestore triggers enable functions to handle events in Firestore that is in the same Google Cloud project as the function. When you specify a Firestore trigger for a function, you choose an event type, and a document path. When an event of the specified type occurs on a document, the function is invoked. Firestore supports create, update, delete, and write events. The function receives a data object with a snapshot of the affected document. Firestore triggers only apply at the document level. It is not possible to create a trigger for a specific document field or collection. Firestore must be in the same Google Cloud project as the function. The function can be a CloudEvent or Background function based on the language runtime. Cloud Run fnctions supports triggers for various Firebase services: Google Analytics for Firebase (Cloud Run functions 1st generation only), Firebase Realtime Database, Firebase Authentication (Cloud Run functions 1st generation only) And Firebase Remote Config. You can handle events in the Firebase service that is in the same Google Cloud project as the function.

### Video - [Connecting Cloud Run functions with workflows](https://www.cloudskillsboost.google/course_templates/505/video/513266)

* [YouTube: Connecting Cloud Run functions with workflows](https://www.youtube.com/watch?v=C3-HeJgyCb0)

Let’s now discuss how you can use Workflows to connect Cloud Run functions and link a series of services together. What is Workflows? Workflows is a fully-managed, serverless orchestration platform that executes services in an order that you define (a workflow). It acts as the central orchestrator for the service orchestration pattern. You design and deploy workflows, which orchestrate and combine Google Cloud services and API calls. To build stateful, automated processes, Workflows can include custom services or functions that are hosted on Cloud Run. A workflow provides a central source-of-truth for the application flow. Each execution of a workflow is logged and is observable, which makes it easier to understand the current state of the workflow and troubleshoot any issues. A workflow can hold state, retry, poll, or wait for up to a year. This flexibility allows for creation of long-running business processes. You can use Workflows to connect a series of services together that include HTTP services built with Cloud Run functions, external APIs, and other Cloud services like Cloud Run. With this approach, you can create a flexible serverless application. The first step to build a workflow is to enable the required Google APIs for Cloud Run functions, Cloud Run, Workflows, and any other services that you use. You may also need to create any service accounts that are required to access these services. Next, write, and deploy the functions. These functions are HTTP functions with HTTP triggers that generate URL endpoints that are used to invoke the functions. Test the functions individually with curl or any other HTTP client. It’s also a best practice to test the functions locally before deployment. You then create the workflow that connects the Cloud Run functions. After the workflow is created, you deploy and execute it. A workflow is made up of a series of steps that are described using the Workflows syntax. The set of steps is the workflow definition and can be written in either YAML or JSON format. In the sample workflow definition, the Cloud Run functions steps cfn1 and cfn2, are invoked from the workflow through an HTTP request using the GET and POST methods respectively. The URLs to the functions are provided as arguments in the function definition. The result generated by the first cloud function is provided as input to the second cloud function. The workflow definition also includes: The configuration to connect to an external REST API endpoint with the result of the second cloud function passed in a query parameter. And, configuration that connects a Cloud Run service in the workflow. The result generated by the Cloud Run service is the result of the workflow. In this section, we discuss how you can connect Cloud Run functions to resources in a VPC network. You use Serverless VPC Access to connect Cloud Run functions directly to your VPC network. A Virtual Private Cloud (VPC) network is a virtual version of a physical network, implemented inside Google's production network. It’s a global resource that consists of a list of regional virtual subnetworks (subnets) in data centers, all connected by a global wide area network. With Serverless VPC Access, you can connect Cloud Run functions directly to your VPC network, and enable access to Compute Engine VM instances, Memorystore, and other resources with an internal IP address. With Serverless VPC Access, you can send requests and receive responses to and from your VPC network using internal DNS and internal IP addresses, so that traffic is not exposed to the internet. To configure Serverless VPC Access, you: Enable the Serverless VPC Access API. Create a Serverless VPC Access connector in your Google Cloud project. A Serverless VPC Access connector is a resource that handles traffic between your serverless Cloud Run functions environment and your VPC network. Attach the connector to a VPC network and region. The region that is configured for the connector must match the region where your Cloud Run functions are deployed. A subnet or CIDR range must be configured exclusively for use by the connector. After you have created a Serverless VPC Access connector, you must configure each function that you want to connect to your VPC network. You can configure a function to use a connector from the Google Cloud console or the gcloud CLI. You can also restrict your connector's access to resources in your VPC network by using firewall rules, and connect Cloud Run functions to resources in a shared VPC network. For more information on configuring Serverless VPC Access connectors, refer to the reading document provided with this course, and the Cloud Run functions website documentation.

### Video - [Lab Intro: Connect Cloud Run Functions](https://www.cloudskillsboost.google/course_templates/505/video/513267)

* [YouTube: Lab Intro: Connect Cloud Run Functions](https://www.youtube.com/watch?v=SUvgmESQ0CM)

This is an optional lab that teaches you how to connect Cloud Run functions to resources in a VPC network. In this lab, you create a Serverless VPC Access connector to connect Cloud Run functions to a Memorystore for Redis instance, and to a VM instance in your VPC network. Memorystore is a fully managed in-memory data store service for Redis and Memcached on Google Cloud. You first create a Memorystore instance for Redis. Next, you create a Serverless VPC Access connector. A connector enables your Cloud Run functions to connect to resources in a VPC network. Then, you write and deploy an event-driven function that receives a message from a Pub/Sub topic and, using the connector, stores the message data in the Memorystore for Redis datastore. You also write an HTTP function to fetch the message data from the Redis datastore using the connector, and return the data in a HTTP response. You then create a VM with a simple web server in your network, and write an HTTP function to access the web server using the Serverless VPC Access connector.

### Lab - [Connect Cloud Run Functions](https://www.cloudskillsboost.google/course_templates/505/labs/513268)

In this lab, you develop Cloud Run functions that connect to resources in your Google Cloud project.

* [ ] [Connect Cloud Run Functions](../labs/Connect-Cloud-Run-Functions.md)

### Document - [Configuring Serverless VPC Access for Cloud Run Functions](https://www.cloudskillsboost.google/course_templates/505/documents/513269)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/505/quizzes/513270)

#### Quiz 1.

> [!important]
> **An HTTP trigger: (Select two)**
>
> * [ ] Generates a URL when it is assigned to a function.
> * [ ] Does not support the DELETE HTTP request method.
> * [ ] Enables a function to respond to HTTP requests.
> * [ ] Enables a function to respond to events from cloud infrastructure.

#### Quiz 2.

> [!important]
> **What are two reasons for using Serverless VPC Access?**
>
> * [ ] To connect Cloud Run functions to internal resources in a VPC network.
> * [ ] To enable Cloud Run functions to access external HTTP endpoints.
> * [ ] To expose requests and responses to and from a VPC network to the internet.
> * [ ] To send requests and receive responses using internal DNS and IP addresses.

#### Quiz 3.

> [!important]
> **Which of these statements about Cloud Run functions triggers are correct? Select three.**
>
> * [ ] Triggers are specified during function deployment.
> * [ ] An event trigger reacts to cloud events.
> * [ ] Multiple functions can be triggered by the same trigger settings.
> * [ ] A function can be bound to multiple triggers at the same time.

#### Quiz 4.

> [!important]
> **Which of these statements about Workflows are correct? Select three.**
>
> * [ ] A workflow step can be defined to make an HTTP call to a URL.
> * [ ] Workflows can combine services or functions hosted on Cloud Run.
> * [ ] Workflows is serverless.
> * [ ] In a workflow, data cannot be shared between steps.

### Video - [Module review](https://www.cloudskillsboost.google/course_templates/505/video/513271)

* [YouTube: Module review](https://www.youtube.com/watch?v=cD_N4hxaSfs)

Let's review what was discussed in this module. In this module, we discussed triggers and how they are used to trigger Cloud Run functions. We also discussed how to connect functions with Workflows, and how to connect functions to resources in a VPC network. You learned about HTTP and event triggers that are used to invoke Cloud Run functions. You learned how to connect Cloud Run functions with Workflows, Google Cloud’s serverless orchestration platform that executes cloud services as a series of steps in a workflow. We discussed how you can connect Cloud Run functions to internal resources in a VPC network. And reviewed an optional lab to connect Cloud Run functions to Memorystore and a VM resource in a network.

## Securing Cloud Run Functions

Secure access to Cloud Run functions, learn about function identity and how to protect data used by functions.

### Video - [Accessing and authenticating to functions](https://www.cloudskillsboost.google/course_templates/505/video/513272)

* [YouTube: Accessing and authenticating to functions](https://www.youtube.com/watch?v=s_sIxTmmmY0)

Welcome to this module on securing Cloud Run functions. In this module, we discuss how to secure Cloud Run functions with identity and network-based access controls. You learn how to authenticate and authorize access to cloud functions, and how to protect Cloud Run functions and related data with encryption keys. We’ll first discuss how you can secure access to your Cloud Run functions, and how to authenticate and authorize to Cloud Run functions during invocation. We’ll also discuss how you can protect Cloud Run functions and their associated data. Finally, we’ll review what was discussed in this module. Let’s get started with securing access to Cloud Run functions. You secure access to Cloud Run functions with identity-based access controls and network-based access controls. To secure access with identity-based access controls, the first step is to validate the identity credential, and make sure that the requestor is who it says it is. Once the requestor's identity has been authenticated, its level of access or permissions can be evaluated. This step is called authorization. By default, functions are deployed as private, and require authentication. You can also deploy a function as public and not require authentication. Cloud Run functions supports two different kinds of identities: Service accounts, which serve as the identity of a non-person, like a function, application, or a VM. And user accounts, which represent people - either as individual Google Account holders or as part of a Google Group. To authenticate to Cloud Run functions, clients create a token based on the service account or user account credential. The token has a limited lifetime, is passed with the request, and serves to safely authenticate the account. The token-based authentication is used to limit the potential damage that might occur if the service or user account credential is leaked. Cloud Run functions uses two types of tokens: OAuth 2.0 access tokens, used to authenticate API calls. And ID tokens, used to authenticate calls to developer-created code, for example, a function calling another function. The tokens are created using the OAuth 2.0 framework and Open Identity Connect (OIDC). Once the identity of the requesting entity has been confirmed, the permissions of the identity are evaluated. The permissions are granted when the authenticated account was set up. Cloud Run functions uses Identity and Access Management (IAM) to evaluate permissions using roles. A role is a set of individual permissions that are grouped together and assigned to the account, either directly or through a policy configuration. Each individual permission in the role set usually corresponds to a single REST API call exposed by the requested service. For more information on this process, see the documentation on Authorizing Access with IAM. To authorize identities to perform administrative actions like creating, updating, and deleting functions, you add principals or identities (a user or service account email) to the function with the appropriate IAM roles. Roles include permissions that define a set of allowed actions that can be performed on the function. The predefined roles that are supported by Cloud Run functions are: Cloud Functions Admin, Cloud Functions Developer, Cloud Functions Invoker, and Cloud Functions Viewer. You can authorize access to a function in the Google Cloud console or with the gcloud CLI. For a complete list of user roles and service accounts used with Cloud Run functions, see the access control with IAM documentation. For a list of permissions in each role, see the Cloud Functions IAM Roles documentation. Event-driven functions can only be invoked by the event source that they are subscribed to. HTTP functions can be invoked by different types of identities, for example, a developer who is testing the function, or a service that uses the function. These identities must provide an ID token with the appropriate permissions for authentication and authorization. When testing a function as a developer, you must have a user account to access Cloud Run functions with a role that contains the appropriate permissions on the function being invoked. Then, generate an ID token using this account, and pass the token in the Authorization header of the request to the function. Functions often need access to other resources in Google Cloud to do their work. Every function is associated with a service account that serves as its identity when the function accesses other resources. The service account that a function uses as its identity is known as its runtime service account. Cloud Run functions uses a default runtime service account for function identity: The Compute Engine Engine default service account, or the App Engine default service account for 1st generation. Use the default service account for testing and development purposes only. For production, specify a different individual runtime service account when deploying a function, and grant the runtime service account only the minimum set of permissions required to achieve its goal. When building services that connect multiple functions, ensure that each function can only send requests to a specific subset of your functions. To configure a receiving function to accept requests from a specific calling function, grant the Cloud Run Invoker (roles/run.invoker) role to the calling function's service account on the receiving function. For Cloud Run functions (1st generation), grant the Cloud Run functions Invoker role (roles/cloudfunctions.invoker). The calling function must also provide a Google-signed ID token for authentication, with the audience field (aud) set to the URL of the receiving function. The ID token must be sent in an Authorization header in the request to the function. To learn more about generating the token, view the documentation. You can also limit access by specifying network settings for Cloud Run functions. Network settings enable you to control network ingress and egress to and from individual functions. Ingress settings restrict whether a function can be invoked by resources outside of your Google Cloud project or VPC Service Controls service perimeter. You can choose to allow all traffic, allow internal traffic only, or allow internal traffic and traffic from Cloud Load Balancing. Internal traffic is traffic from Workflows and VPC networks in the same project or VPC Service Controls perimeter. Egress settings control the routing of outbound HTTP requests from a function. To specify egress settings, you must connect functions to a VPC network using a Serverless VPC Access connector. Egress settings control which types of traffic are routed through the connector to your VPC network. You can set egress settings to route all outbound traffic from the function through the connector, or, route only requests to private IPs through the connector. You can use VPC Service Controls with Cloud Run functions to add additional security to your functions. To do this, you create a service perimeter, and add one or more projects to the perimeter. For Shared VPCs, add the host and service projects to the perimeter. And restrict the Cloud Functions API by setting up organization policies that control the network settings for functions in the service perimeter. With the organization policies in place: HTTP functions will only accept traffic that orginates from a VPC network within the service perimeter. All functions must use a Serverless VPC Access connector. And functions must route all egress traffic through your VPC network. View the VPC Service Controls with Cloud Run functions documentation for more details.

### Video - [Protecting functions and data](https://www.cloudskillsboost.google/course_templates/505/video/513273)

* [YouTube: Protecting functions and data](https://www.youtube.com/watch?v=jztPfU2Dgm0)

Let’s discuss how you can protect your Cloud Run functions and it’s data. You can use Cloud Key Management Service (KMS) to create and manage encryption keys that protect your Cloud Run functions and related data at rest. The keys are known as customer-managed encryption keys (CMEK) and are owned by you and not controlled by Google. They can be stored as software keys, in an HSM cluster, or externally. Deploying a function with a CMEK protects the data associated with it by using an encryption key that only you can access. If the key is disabled or destroyed, no one (including you) can access the data that is protected by the key. The following types of Cloud Run functions data are encrypted when using a CMEK: Function source code uploaded for deployment and stored by Google in Cloud Storage, and used in the build process. The results of the function build process, including: The container image built from your function source code, and each instance of the function that is deployed. The data at rest for internal event transport channels. To set up CMEK for Cloud Run functions: Create a single-region encryption key. To store your function images, create an Artifact Registry repository with CMEK enabled. Use the same key for the repository as the one used to enable CMEK for the function. Grant the Cloud Run functions, Artifact Registry, and Cloud Storage service accounts access to the key. Enable CMEK on your function. A sample use case for using CMEKs involves storing and accessing objects in Cloud Storage buckets. You can use customer-managed encryption keys on individual objects, or configure your bucket to use a key by default on all new objects added to the bucket. Objects that are uploaded are stored encrypted with the CMEK. A Cloud Run function can be triggered from Eventarc whenever there are changes to objects in the Cloud Storage bucket. The function can then retrieve the decrypted object from the bucket in Cloud Storage. You can also implement a function to encrypt individual objects and upload them to Cloud Storage. To use CMEKs, you must grant your project’s Cloud Storage service account or service agent access to the key. To grant service accounts access to the key, add each service account as a principal of the key, and then grant the service account the Cloud KMS CryptoKey Encrypter/Decrypter role. The service account email used is that of the: Cloud Run Functions Service Agent, Artifact Registry Service Agent, Cloud Storage Service Agent. After setting up an Artifact Registry repository with CMEK enabled and granting the required service agents access to your key, you can enable CMEK for your function by deploying the function and specifying the key and repository. Cloud Run functions uses the primary version of a key for CMEK protection. You cannot specify a particular key version to use when enabling CMEK for your functions. If a key is destroyed or disabled, or the requisite permissions on it are revoked: Active instances of functions protected by the key are not shut down. Executions of these functions that are already in progress will continue to run. New executions will fail as long as Cloud Run functions does not have access to the key. Executions that require new function instances will fail.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/505/quizzes/513274)

#### Quiz 1.

> [!important]
> **Which statements about function identity are correct? Select three.**
>
> * [ ] The App Engine default service account is used as the default runtime service account for Cloud Run functions (1st gen).
> * [ ] In production environments, you should use a runtime service account for a function's identity with the maximum set of permissions.
> * [ ] Every function is associated with a runtime service account that serves as its identity.
> * [ ] The Compute Engine default service account is used as the default runtime service account for Cloud Run functions.

#### Quiz 2.

> [!important]
> **Cloud Run functions uses IAM to authorize the requesting identity. Which predefined IAM roles are used by Cloud Run functions? Select four.**
>
> * [ ] Cloud Functions Invoker
> * [ ] Cloud Functions Admin
> * [ ] Cloud Functions Viewer
> * [ ] Cloud Functions Reader
> * [ ] Cloud Functions Developer

#### Quiz 3.

> [!important]
> **A customer-managed encryption key (CMEK) is used to encrypt a function and its related data. What is the impact when such a key is disabled or destroyed?**
>
> * [ ] Executions that require new function instances will fail.
> * [ ] Executions of the function that are already in progress are terminated.
> * [ ] There is no impact to the function.
> * [ ] Active instances of the function are shut down.

#### Quiz 4.

> [!important]
> **Which network setting allows Cloud Run functions to route all outbound traffic from a function through a VPC network?**
>
> * [ ] Egress setting to route traffic only to private IPs through a Serverless VPC connector.
> * [ ] Egress setting to route all traffic through a Serverless VPC connector.
> * [ ] Ingress setting to allow internal traffic and traffic from Cloud Load Balancing.
> * [ ] Ingress setting to allow all traffic.

#### Quiz 5.

> [!important]
> **To limit access to Cloud Run functions, what methods can you use? Select two.**
>
> * [ ] Use HTTPS.
> * [ ] Use network-based access controls.
> * [ ] Use a username and password.
> * [ ] Use an encryption key.
> * [ ] Use identity-based access controls.

### Video - [Module review](https://www.cloudskillsboost.google/course_templates/505/video/513275)

* [YouTube: Module review](https://www.youtube.com/watch?v=8J9btd8UaSU)

Let’s review the topics that were discussed in this module. In this module, we discussed how to securely access and authenticate to Cloud Run functions with identity and network-based access controls. You also learned about function identity, and how to protect Cloud Run functions with customer-managed encryption keys. You learned how to use identity and network ingress and egress settings to secure access to Cloud Run functions. You learned how to use service and user accounts with appropriate roles to authenticate to Cloud Run functions, and how to use a function’s runtime service account or function identity to authenticate to other functions. We also discussed how you can use customer-managed encryption keys to protect Cloud Run functions and their data, and reviewed a sample functions use case of using CMEKs with Cloud Storage.

## Integrating with Cloud Databases

Learn how to integrate Cloud Run functions with Cloud databases.

### Video - [Integrating functions with cloud databases](https://www.cloudskillsboost.google/course_templates/505/video/513276)

* [YouTube: Integrating functions with cloud databases](https://www.youtube.com/watch?v=57gL-C76AL4)

In this module, we discuss how you can integrate your functions with cloud databases. You learn how to securely connect your functions to read and write data from and to Firestore and Memorystore databases in Google Cloud. In this module, we first discuss how to connect Cloud Run functions to Memorystore, Google Cloud’s cache service, and discuss how you can use environment variables with Cloud Run functions. We’ll then discuss how you can connect Cloud Run functions to Firestore, and how you can use secrets with Cloud Run functions. You’ll then complete a lab on integrating Cloud Run functions with Firestore. Finally, we review what was discussed in this module. Let’s begin. You can integrate Cloud Run functions with: Firestore, Cloud SQL, Spanner, Bigtable, BigQuery, and with Memorystore, Google Cloud’s in-memory cache service. In this module, we discuss how you can connect your Cloud Run functions to Memorystore and Firestore. For information about connecting to other Cloud databases, refer to the documentation. Memorystore is a Google Cloud service that provides a highly available, scalable, and secure in-memory cache solution for Redis and Memcached. It’s a fully managed service that automates provisioning, replication, failover, and patching. It’s also integrated with IAM for secure access, and with Cloud Monitoring for service monitoring and alerting. For a complete list of features, see the Memorystore documentation. Redis is an open source in-memory data structure store used as a database, cache, message broker, and streaming engine. Memcached is an open source distributed memory object caching system. You can connect to a Redis instance from Cloud Run functions by using Serverless VPC Access. Once you’ve determined your Redis instance’s authorized VPC network, you create a Serverless VPC Access connector in the same region as your function. Then, attach the connector to the Redis instance’s authorized VPC network. Specify the network, region, and IP address range when the VPC connector is created. Ensure that the connector is in a Ready state before using it. Deploy the function specifying the path and name of the connector, and environment variables for the Redis host IP address and port. Your function code can then use these environment variables to instantiate a client that connects to the Redis service. To invoke the function, send an HTTP GET request to the functions URL endpoint. The source code for this function can be found on GitHub. Cloud Run functions supports the use of environment variables. Environment variables are key-value pairs that can be set for Cloud Run functions at deployment time. The variables are accessed by your function code at runtime, or as configuration information for the buildpack system. They are stored in the Cloud Run functions backend, are bound to a single function, and exist within the same function lifecycle. You can provide the environment variable key-value pairs when you deploy your function with the gcloud CLI or in the Google Cloud console. You can store them in a YAML file in source control and provide the name of the file during function deployment. For more information on using environment variables with Cloud Run functions, see the documentation. To access runtime environment variables in your function written in Python, use the os module. To access environment variables in other language runtimes, view the samples in the documentation on the Cloud Run functions website. Let’s now discuss how you can connect Cloud Run functions to Firestore. Firestore is a Google Cloud service that provides a fully managed serverless NoSQL document database. It provides high availability, scalability with no maintenance windows or downtime required, and multi-region replication. You store a set of key-value pairs known as a document in Firestore and all documents are stored in collections. For a complete list of features, see the Firestore documentation. You can extend Firestore’s capabilities with Cloud Run functions by handling events that are triggered by changes in your Firestore database. By implementing function code to handle these events, you can easily add server-side functionality to your application without running your own servers. You can implement your function code to handle Firestore events that occur when a document is created, updated, deleted, or when any of these events occur. These events are exposed by the Cloud Run functions for Firebase SDK that you use in your function source code. Firestore triggers for Cloud Run functions are available only for Firestore in Native mode. It is not available for Firestore in Datastore mode. Functions that are triggered on Firestore events must specify a document path, and an event type. The document path can reference a specific document or a wildcard pattern, and must not contain a trailing slash. When a function is triggered, a snapshot of the data related to the event is available to the function. You can use this snapshot to read from or write to the document that triggered the event. The document snapshot data before and after the update is available to the function. Each function invocation is associated with a specific document in your Firestore database. You can access that document as a DocumentReference in the ref property of the snapshot returned to your function. This DocumentReference comes from the Firestore Node.js SDK and includes methods that enable you to modify the document that triggered the function. You can also read and write data of documents other than the one that triggered the function using the Firebase Admin SDK. Cloud Run functions supports the use of secrets. Let’s review how you can use secrets with Cloud Run functions. When your function code needs to access certain databases or APIs, it will need to provide credentials like a database username/password or API key. This kind of sensitive information should be securely stored and accessed by the function when it executes. You can use secrets and Google Cloud’s Secret Manager to store this information. A secret is an object that contains a collection of metadata like replication locations, labels, permissions, and other information; and the secret versions. A secret version stores the actual secret data such as an API key or password as a text string or binary blob. To create and manage secrets, you must enable the Secret Manager API. To access a secret, your function must first be granted access to the secret. This is achieved by granting the appropriate role (roles/secretmanager.secretAccessor) to the function’s runtime service account on the secret. To make the secret available to your function, you can: Mount the secret as a volume so that the function can access it from a file. Mounting the secret as a volume allows your function to reference the latest version of the secret each time the file is read. You can also pass the secret to the function as an environment variable. Because environment variables are resolved at function instance startup time, with this method, your function would have access to a specific version of the secret. To provide your function access to a secret that is in a different project than your function: Grant your function’s runtime service account access to the secret as previously described. Make the secret available to the function by specifying the secret’s resource path that includes the project ID and secret name. A sample use case of using a secret is when your function must access an external service or API, that requires an API key to identify the calling application. The key is considered a sensitive piece of information so it is stored as a secret using Secrets Manager. Write your function code to access the secret by reading the contents of a file or environment variable. The file path is provided when the function is deployed. When deploying the function, provide the secret name and the method to access the secret. The method can be a mounted file path or environment variable. To access the secret, the function’s runtime service account must be granted the Secret Manager Secret Accessor role on the secret. Call the API from the function with the secret value which is the API key.

### Video - [Lab Intro: Integrate Cloud Run Functions with Firestore](https://www.cloudskillsboost.google/course_templates/505/video/513277)

* [YouTube: Lab Intro: Integrate Cloud Run Functions with Firestore](https://www.youtube.com/watch?v=mNfxF4l4k84)

You’ll now complete a lab on integrating Cloud Run functions with Firestore. In this lab, you develop a Cloud Run function to read and write a document to and from a Firestore database, and update that document by responding to create events in Firestore. You first set up Firestore by creating and initializing a Firebase project and database. You then write and deploy an HTTP function that creates a document entity in the Firestore database. Next, you write an event-driven function that is triggered when a document is created in the Firestore database. This function will update the data in the document that was originally created. Finally, you create a secret using Secret Manager, and then access that secret in your Cloud Run function.

### Lab - [Integrate Cloud Run Functions with Firestore](https://www.cloudskillsboost.google/course_templates/505/labs/513278)

In this lab, you develop Cloud Run functions that integrate with Firestore, Google Cloud's serverless NoSQL document database.

* [ ] [Integrate Cloud Run Functions with Firestore](../labs/Integrate-Cloud-Run-Functions-with-Firestore.md)

### Document - [BigQuery Remote Functions](https://www.cloudskillsboost.google/course_templates/505/documents/513279)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/505/quizzes/513280)

#### Quiz 1.

> [!important]
> **Which statements about triggering Cloud Run functions from Firestore database events are correct? Select two.**
>
> * [ ] To trigger a function, you must specify an event type and the document path.
> * [ ] A function cannot be triggered when a Firestore document is deleted.
> * [ ] A function can be triggered when a Firestore document is created, updated, or deleted.
> * [ ] A function can be triggered when a specific field in a Firestore document is changed.
> * [ ] A function can only be triggered on changes to an individual Firestore document.

#### Quiz 2.

> [!important]
> **What are two methods of making a secret available to a cloud function?**
>
> * [ ] Mount the secret as a volume so that the function can access the secret from a file.
> * [ ] Provide the secret name and value as query parameters to the function.
> * [ ] Provide the secret as an environment variable when deploying the function.
> * [ ] Secrets cannot be accessed from Cloud Run functions.

#### Quiz 3.

> [!important]
> **Which three statements about using environment variables with Cloud Run functions are correct?Environment variables:**
>
> * [ ] Cannot be added, updated, or removed.
> * [ ] Can be shared and used by multiple functions.
> * [ ] Can be stored in a YAML file, whose filename can be provided during function deployment.
> * [ ] Are key-value pairs that are accessed by the function code at runtime.
> * [ ] Are provided during function deployment.

### Video - [Module review](https://www.cloudskillsboost.google/course_templates/505/video/513281)

* [YouTube: Module review](https://www.youtube.com/watch?v=hWdVc8DvWdU)

Let’s review the topics that were discussed in this module. In this module, you learned how to connect Cloud Run functions to cloud databases. We discussed how Cloud Run functions can use environment variables, and access secrets stored in Secret Manager. You also completed a lab on integrating Cloud Run functions with Firestore. In this module, you learned how to connect Cloud Run functions to Memorystore, Google Cloud’s in-memory cache service. We discussed the ways in which you can provide environment variable key-value pairs to Cloud Run functions during deployment. We also discussed how you can use event-driven functions to integrate Firestore database events with Cloud Run functions, and how Cloud Run functions can access sensitive values stored as secrets in Google Cloud. You also completed a lab to integrate Cloud Run functions with Firestore.

## Best Practices for Functions

Learn how to use best practices with functions.

### Video - [Best practices for functions](https://www.cloudskillsboost.google/course_templates/505/video/513282)

* [YouTube: Best practices for functions](https://www.youtube.com/watch?v=SCL3hOpe_BY)

In this module, we discuss some of the best practices that you can use when writing functions. In this module, you learn about some of the best practices that are used to implement functions, tips to improve performance and networking, and how to retry functions on failure. We’ll discuss how to configure your functions, including configuration to scale and split traffic between Cloud Run function revisions. Finally, we review what was discussed in this module. Let’s start by first reviewing some of the best practices when implementing functions. Write your functions to be idempotent so that they produce the same result when called multiple times. This lets you retry a function invocation if the previous invocation partially fails for some reason. An HTTP function must always return an HTTP response, otherwise the function may continue executing until timeout and incur charges for the entire time till then. You should not have any activities running in the background after your function invocation terminates because the CPU is not accessible and the code will not continue to execute. A subsequent invocation that is executed in the same environment will cause the background activity to resume and interfere with the current invocation that may lead to errors and unexpected behavior. Ensure that all asynchronous operations in your function code finish before you terminate the function. When developing functions, you write to files in a temporary directory which is part of an in-memory file system. These files consume memory that is available to your function, and sometimes persist between invocations. To avoid eventually running out of memory and a subsequent cold start of your function, ensure that you explicitly delete any files that are created by your function code. To test your function code, you must first deploy it and wait for the deployment to complete and for log entries to become available. Developing and testing your function locally in your development environment makes the development and testing process significantly faster. To comply with data locality restrictions in geographical or network boundaries that are not accessible to your functions, you can run your functions on a platform that complies with these restrictions and is compatible with the open source abstraction layers used in Cloud Run functions. In languages that support exception handling, do not throw uncaught exceptions because they force cold starts in future function invocations. Manually exiting from functions using process.exit() (in Node.js), or using sys.exit() (in Python), may cause unexpected behavior. Instead, return implicitly or explicitly from event-driven functions, and return HTTP responses from HTTP functions. You must always handle runtime errors and exceptions in your function code, because exceptions that are not caught may terminate the function and result in cold starts for future invocations. Runtime exceptions that are emitted from your function are sent to Error Reporting. You can aggregate and view these errors in the Google Cloud console, be notified when they occur, and take steps to troubleshoot and resolve them as quickly as possible. Cloud Run functions includes simple runtime logging by default. Logs written to stdout or stderr will appear automatically in the Google Cloud console. HTTP functions should report the error and respond with an appropriate HTTP status code based on the type of error encountered. Event-driven functions should report and return an error message when an exception occurs. You should report exceptions and errors that may occur during function execution to Google Cloud’s Error Reporting service. Let’s now review some practices to improve performance and networking for functions. A cold start creates and initializes the execution environment of a function. During a cold start, any dependencies that your function imports are loaded, adding to the function’s invocation latency. You can reduce this latency and the time needed to deploy your function, by not loading dependencies that your function doesn't use. The execution environment of a function's previous invocation is often recycled. If you declare a variable in global scope, its value can be reused in subsequent invocations to a function instance without having to be recomputed resulting in significant performance improvements. You can use this approach to cache objects like API client objects and network connections that may be expensive to recreate on each function invocation. Initialization of global variables always increases a function’s latency during cold start invocations. If some of these global variables are not used in all of your function’s code paths, you should consider initializing the variables lazily on demand. Function instances are scaled based on the number of incoming requests. By setting a minimum number of function instances to be kept ready to serve requests, you can reduce cold starts of your function and improve your application’s overall performance. When accessing URLs from your functions, you should create persistent HTTP connections to those URLs. By creating persistent connections and caching them in your function’s global scope, you can reduce the CPU time spent to establish a new connection with each function invocation. You can also reduce the likelihood of exhausting your connection quota. Similarly, to avoid unnecessary connections and DNS queries when communicating with Google APIs from your function, create the Google service client object in global scope. Use Serverless VPC Access connectors to send requests and receive responses to and from your VPC network using internal DNS and internal IP addresses, so that traffic to internal resources is not exposed to the internet. Let’s discuss how you can retry functions on failure. Automatic retry is available for event-driven functions only, and is disabled by default. You can enable automatic retries for a function with the –retry flag using the gcloud functions deploy CLI command, or select the Retry on failure option in Google Cloud console when you deploy the function. To disable retries, you must redeploy the function without the –retry flag or clear the Retry on failure option in Google Cloud console. Some reasons for function failure are: A bug causes the runtime to throw an exception that is not handled. A service endpoint is not reachable from the function which times out. The function code intentionally throws an unhandled exception when certain conditions occur. A Node.js function returns a rejected promise or passes a non-null value to a callback. In these situations, the function stops executing and the event is discarded. With retry enabled, the event is retried repeatedly for up to seven days by default until the function executes successfully, or the maximum retry period has elapsed. Retries are best used to handle intermittent or transient failures such as failing to connect to a service endpoint or timing out while waiting for the connection to succeed. These kinds of failures have a high likelihood of resolution upon retrying. Because your function is retried continuously until successful execution, any bugs that cause function failure should be discovered and fixed in your code through testing before enabling retries. Ensure that your function code handles any exceptions that should not result in a function retry. When failures are persistent, prevent infinite retry loops by including an end condition in your function before the function processing code executes. One approach is to use timestamps to discard events that are older than a specified time. Let’s discuss some best practices on function configuration, and using IAM with functions. Following the principle of least privilege, ensure that you limit access to your functions to the minimum number of users and service accounts, and allocate the minimum set of permissions required to develop and use your functions. When building services that connect multiple functions, ensure that each function can only send requests to a specific subset of your other functions. For example, a login function should be able to access a user profiles function, but probably not be able to a ccess a search function. Unless you specify a different runtime service account when deploying a function, a default service account is used for the function's identity. For production use, you should give each function a dedicated identity by assigning it a user-managed service account. User-managed service accounts let you control access by granting a minimal set of permissions using Identity and Access Management. You can provision Cloud Run functions with different amounts of memory and control the amount of memory a function can use. The amount of allocated memory you choose corresponds to an amount of allocated CPU for your function. To limit the amount of memory allocated to a function, use the –memory flag with the gcloud functions deploy command or use the memory settings in the Google Cloud console. For more details, see the documentation on memory limits for Cloud Run functions. To prevent your function from timing out, specify your function’s timeout duration to be slightly higher than the function’s execution time. Use the –timeout flag with the gcloud functions deploy command or the Timeout settings in Google Cloud console. For more details, see the documentation on function timeout. By default, function instances handle only one request at a time. You can change this behavior for Cloud Run functions, so that they can handle multiple concurrent requests to a single function instance. This helps to reduce overall latency by preventing cold starts as an already warmed instance can process additional requests to the function. To enable concurrency, set a concurrency value per function through the function's underlying Cloud Run service. The concurrency value represents the maximum number of concurrent requests that a single instance of the function can handle. With concurrency enabled, your function code must be safe to execute concurrently as Cloud Run functions does not provide isolation. Let’s review how functions scale and how you can split traffic between revisions of your Cloud Run functions. Scaling is implemented by creating new instances of your function based on the volume of requests to your function. You can control the scaling behavior of your function by setting the minimum and maximum number of function instances during deployment. Functions scale independently of each other with each function having its own scaling configuration. To avoid cold starts for your application and reduce application latency set a minimum number of instances for your function. To limit requests to throughput-constrained downstream resources (for example databases), set the maximum number of instances for your function. To handle spikes in traffic, more than the specified maximum instances might be created for a short period. Also, because instances limits are set for each revision of your function independently, the specified limit might be temporarily exceeded during the period after deployment. This happens so that existing requests are processed uninterrupted by the previous instances, and any new requests are handled by the new instances. Each time you deploy a Cloud Run function, a new revision of the function and the underlying Cloud Run service is automatically created. Revisions are immutable and cannot be modified once they are deployed. To change a function, you must redeploy it. By default, all traffic to a function is routed to its latest revision. You can change this behavior by setting a custom traffic configuration, enabling you to split traffic between different revisions or roll your function back to a prior revision.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/505/quizzes/513283)

#### Quiz 1.

> [!important]
> **How can you control the scaling behavior of functions?**
>
> * [ ] Function scaling is handled automatically and cannot be controlled.
> * [ ] Because there are no servers to manage, functions cannot be scaled.
> * [ ] Set the minimum and maximum number of function instances during deployment.
> * [ ] Use a common configuration to control the scaling behavior of all of your functions.

#### Quiz 2.

> [!important]
> **To improve the performance of your function, what are three best practices to follow?**
>
> * [ ] Set a minimum number of instances when deploying your function.
> * [ ] Remove any unused dependencies from the function source.
> * [ ] Initialize global variables in your function code eagerly.
> * [ ] In your function code, reuse objects with global variables.

#### Quiz 3.

> [!important]
> **To optimize networking for your function, which two approaches should you use?**
>
> * [ ] Serverless VPC Access connectors to connect your cloud function to project resources.
> * [ ] Local scope to initialize and store network connections and API client objects.
> * [ ] Persistent HTTP connections.

#### Quiz 4.

> [!important]
> **Which statement regarding revisions of Cloud Run functions is correct?**
>
> * [ ] You cannot roll back a function to a prior revision.
> * [ ] You can change an existing revision of a deployed function.
> * [ ] You can split traffic between different revisions of a function.
> * [ ] When a function is deployed, a new revision is not automatically created.

#### Quiz 5.

> [!important]
> **Which two statements about retrying of functions are correct?Function retry:**
>
> * [ ] Is supported for both HTTP and event-driven functions.
> * [ ] Is enabled by default.
> * [ ] Can be enabled or disabled in Google Cloud console or with the gcloud CLI.
> * [ ] If enabled, causes the function to be retried on failure for up to 7 days.

#### Quiz 6.

> [!important]
> **What are three best practices to use when implementing IAM policies for functions?**
>
> * [ ] In production environments, use the default runtime service account for a function's identity.
> * [ ] Ensure that a function sends requests only to a subset of your other functions that are needed to perform its job.
> * [ ] Limit the number of user and service accounts that can access the function.
> * [ ] Allocate the minimum set of permissions required to develop and use your functions.

### Video - [Module review](https://www.cloudskillsboost.google/course_templates/505/video/513284)

* [YouTube: Module review](https://www.youtube.com/watch?v=hjigWJuyoJQ)

In this module, we discussed some of the best practices when writing functions, and how to optimize them for performance and networking. We discussed how to enable and optimize function retry, and the error conditions that trigger the retrying of functions. You learned about best practices when implementing IAM policies for your functions, and to configure functions to control the amount of memory used, and avoid function timeouts. Finally, we discussed how functions are scaled and how you can control the scaling behavior with configuration, and you learned how to split traffic between different revisions of a Cloud Run function.

## Course Review

Review of course content.

### Video - [Course Review](https://www.cloudskillsboost.google/course_templates/505/video/513285)

* [YouTube: Course Review](https://www.youtube.com/watch?v=ioPKIckpPLQ)

Congratulations on completing this course on Developing Applications with Cloud Run Functions on Google Cloud. Let’s review the topics that were discussed and the skills you gained in this course. By completing this course, you can now develop and test functions locally, and deploy them to Cloud Run functions using the Google Cloud console, or the gcloud CLI. You can use HTTP or event triggers to invoke and trigger your Cloud Run functions based on your application requirements. You have the knowledge and skills to connect Cloud Run functions with Workflows, and to project resources with Serverless VPC Access. You learned how to secure access to Cloud Run functions with authentication and authorization, and how to protect functions with customer-managed encryption keys. You now have the skills to provide environment variable key-value pairs to Cloud Run functions during deployment, and enable Cloud Run functions to access sensitive values stored as secrets in Google Cloud. You also learned how to use event-driven functions to integrate Firestore database events with Cloud Run functions, and how to connect Cloud Run functions to Memorystore, Google Cloud’s in-memory cache service. By completing this course, you have the knowledge to implement best practices when developing and configuring Cloud Run functions for optimal performance. Now that you’ve completed this course on developing applications with Cloud Run functions, you might consider learning about other services such as Cloud Run, Google Kubernetes Engine, and about Service Orchestration and Choreography on Google Cloud. Some of these courses are part of a set of courses in the Cloud Developer learning path that you can subscribe to, and expand your knowledge and skills on Google Cloud.

## Course Resources

Student PDF links to all modules.

### Document - [Course Resources](https://www.cloudskillsboost.google/course_templates/505/documents/513286)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
