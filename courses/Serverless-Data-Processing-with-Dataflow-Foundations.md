---
id: 218
name: 'Serverless Data Processing with Dataflow: Foundations'
datePublished: 2025-01-10
topics:
- IAM
- Batch Processing
- Data Processing
type: Course
url: https://www.cloudskillsboost.google/course_templates/218
---

# [Serverless Data Processing with Dataflow: Foundations](https://www.cloudskillsboost.google/course_templates/218)

**Description:**

This course is part 1 of a 3-course series on Serverless Data Processing with Dataflow. In this first course, we start with a refresher of what Apache Beam is and its relationship with Dataflow. Next, we talk about the Apache Beam vision and the benefits of the Beam Portability framework. The Beam Portability framework achieves the vision that a developer can use their favorite programming language with their preferred execution backend. We then show you how Dataflow allows you to separate compute and storage while saving money, and how identity, access, and management tools interact with your Dataflow pipelines. Lastly, we look at how to implement the right security model for your use case on Dataflow.

**Objectives:**

- Demonstrate how Apache Beam and Dataflow work together to fulfill your organization’s data processing needs
- Summarize the benefits of the Beam Portability Framework and enable it for your Dataflow pipelines
- Enable Shuffle & Streaming Engine for batch & streaming pipelines respectively for maximum performance
- Enable Flexible Resource Scheduling for more cost efficient performance
- Select the right combination of IAM permissions for your Dataflow job
- Implement best practices for a secure data processing environment

## Introduction

This module covers the course outline and does a quick refresh on the Apache Beam programming model and Google's Dataflow managed service.

### Video - [Course Introduction](https://www.cloudskillsboost.google/course_templates/218/video/520329)

- [YouTube: Course Introduction](https://www.youtube.com/watch?v=iCILVzFonR4)

Hi, and welcome to the first installment of the Serverless Data Processing with Dataflow series, Dataflow Foundations, My name is Mehran Nazir, and I am a product manager with Dataflow. The Serverless Data Processing with Dataflow Course Series builds on the concepts covered in the Data Engineering specialization. We introduced core Dataflow principles when exploring how to build batch data pipelines on Google Cloud. We also covered streaming basics concepts like windowing, triggers, and watermarks while learning how to build resilient streaming systems using Dataflow. This course series expands on those concepts with three additional courses: Foundations, which will cover the fundamentals of the Apache Beam and Dataflow model. Developing Pipelines, which will provide a comprehensive review of the Apache Beam SDK. And Operations, which will equip learners with the tools to run your Dataflow pipelines at scale. In this course, we will do a deep dive on Foundations. Let’s review the outline for the Dataflow Foundations course. First, we will do a quick refresh on the Apache Beam programming model and Google’s Dataflow managed service. Next, we will learn about the Beam Portability Framework, which allows users to write pipelines in their preferred programming language and run on their desired execution engine. In the next module, we will learn about Dataflow’s premium backends that separate compute and storage for maximum performance. We will then explore how IAM, quotas, and permissions work together to enable Dataflow pipelines. Finally, we will review the main security features that are available with Dataflow and how to implement them. To conclude, we will summarize the main concepts covered in the Foundations course.

### Video - [Beam and Dataflow Refresher](https://www.cloudskillsboost.google/course_templates/218/video/520330)

- [YouTube: Beam and Dataflow Refresher](https://www.youtube.com/watch?v=7k3NJfGXpoE)

Federico: Hi, I'm Federico Patota, a cloud consultant here at Google. In this section, we will revisit some concepts on the relationship between Apache Beam and Dataflow, and we will see why customers value Dataflow so much. Apache Beam is an open source unified programming model to define both batch and streaming processing pipelines. To create a pipeline, you can use the Beam SDK of the language of your choice to build a program that defines your data-processing pipeline. Beam SDKs use the same classes to represent both batch and streaming data sources, and the same run forms to operate on that data. We will talk more about this in the next course on developing pipelines. A pipeline can be run locally on your computer, remotely on a virtual machine in a data center, or by using the services of a cloud provider. To decide which will be the engine powering your pipeline, you need to specify a runner. Each runner has its own configuration, and it is associated with a backend service. As you might now already, Dataflow is one of the runners available in Apache Beam. It is a fully-managed data processing service with automated provisioning and management of processing resources. Dataflow includes resource autoscaling and dynamic work rebalancing to maximize resource usage and automatically optimize your pipeline execution. It is part of the Google Cloud ecosystem and uses horizontal service like logging and monitoring. Dataflow allows you to separate computing storage resources. We will cover this more in detail in another module of this course.

## Beam Portability

In this module we are going to learn about four sections, Beam Portablity, Runner v2, Container Environments, and Cross-Language Transforms. 

### Video - [Beam Portability](https://www.cloudskillsboost.google/course_templates/218/video/520331)

- [YouTube: Beam Portability](https://www.youtube.com/watch?v=mEt-T951mUY)

Federico: Hi and welcome back. Now you will learn about Beam portability. This module is made up of four sections. In this video, we talk about the Beam portability framework. To better understand the purpose of Beam portability, we can start with the vision behind it. The Beam vision is to provide a comprehensive portability framework for data processing pipelines, one that allows you to write your pipeline once in the programming language of your choice and run it with minimal effort on the execution engine of your choice. With Apache Beam, you can define your pipeline in popular languages like Java, Python, Go, SQL. With Beam, you also have the flexibility to move your data processing pipeline from your own premise environment to Dataflow on Google Cloud or any other clouds. There is no vendor lock-in. At the same time, we believe that Dataflow offers the most compelling experience across all of the runners. The portability framework is a language-agnostic way of representing and executing Beam pipelines. It introduces well-defined, language neutral data structures and protocols between the SDKs and the runners. This interoperability layer is called Portability API and enables you to use the language of your choice with the runner of your choice, thus ensuring that SDKs and runners can work with each other uniformly. Moreover, because docker containerization is used, you can customize the execution environment running on the worker nodes of the back end service. Portability brings several additional benefits. Let's review them together. With portability, every runner can work with every supported language. Containerization allows us a configurable, hermetic worker environment. You can have multi-language pipelines and cross-language transforms because of the language-agnostic representation of pipelines and the isolated environment of each operation. And all of this will bring you a faster delivery of new features available in the SDKs because, with portability, every time a new functionality is added to a supported language, it will automatically be available to all DRs.

### Video - [Runner v2](https://www.cloudskillsboost.google/course_templates/218/video/520332)

- [YouTube: Runner v2](https://www.youtube.com/watch?v=T_zvtYU09n0)

person: Let's talk about Dataflow Runner v2. To use the portability features mentioned earlier, you must use the Dataflow Runner v2. This new version of the Dataflow Runner uses a more efficient and portable work architecture, based on the Apache Beam portability framework. As we will discuss in detail in a moment, it supports custom containers, multi-language pipelines and cross-language transforms. This runner is packaged together with the Dataflow Shuffle service and Streaming Engine that you will see more in depth in the next module. To enable it, please refer to Dataflow official documentation.

### Video - [Container Environments](https://www.cloudskillsboost.google/course_templates/218/video/520333)

- [YouTube: Container Environments](https://www.youtube.com/watch?v=oazNZHmB6_Y)

Federico: In this video, we'll look at container environments. The Beam SDK runtime environment can be containerized with Docker to isolate it from other runtime systems. Each user operation has an associated environment in which to execute. Typically, supported SDKs provide a default environment that you can further customize. Because of containerization, you can benefit from ahead-of-time installation. You can include arbitrary dependencies, and even further customization is possible. Now, let's see how you can run your pipeline with custom containers. To use this feature, you need to have the Apache Beam SDK version 2.25.0 or later installed. If you want to test your pipeline locally, you will also need to have Docker installed. To create a custom container image, create a Docker file in which you specify the Apache Beam image as the parent image. Then add your own customizations. After creating your custom Docker file, you need to build the image and push it to a container registry. To do so, you need to specify your project, the name of the image repository, the tag that you want to associate with your image, and the image registry host name. Then you can use either Cloud Build or Docker to build the image and push it to a container registry like GCR.IO. Finally, you can launch your Dataflow job by referencing the regular parameters and the location of the custom container image.

### Video - [Cross-Language Transforms](https://www.cloudskillsboost.google/course_templates/218/video/520334)

- [YouTube: Cross-Language Transforms](https://www.youtube.com/watch?v=yZw9gVpCm6g)

Person: In this video, we look at cross-language transforms. With a language agnostic representation of pipelines and the possibility to specify the environment of each operation, you are no longer limited to a single language in a given pipeline. Portability makes it possible for you to run multi-language pipelines that leverage the respective benefits of the individualized case. For example, you can now write a Python pipeline while using I/O connectors that were only available in Java, or if you want to use a TensorFlow extended block of code for a machine learning model in your Java pipeline, you can now use a cross-language transform. Let's go through an example together. The code you see represents a part of a Python streaming pipeline. The ReadFromKafka transform imported from the apache_beam.io.kafka module is a cross-language transform implemented using the Beam Java SDK. Under the hood, to make Java transforms available to a dataflow Python pipeline, The Apache Beam Python SDK starts up a local Java service on your computer to create and inject the appropriate Java pipeline fragments into your Python pipeline. Then the SDK downloads in stages the necessary Java dependencies needed to execute these transforms, and at run time, the dataflow workers will execute the Python and Java code simultaneously to run your pipeline.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/218/quizzes/520335)

#### Quiz 1.

> [!important]
> **What is the Beam portability framework?**
>
> - [ ] A set of protocols for executing pipelines
> - [ ] A hermetic worker environment
> - [ ] A set of cross-language transforms
> - [ ] A language-agnostic way to represent pipelines

#### Quiz 2.

> [!important]
> **Which of the following are benefits of Beam portability? (Select ALL that apply.)**
>
> - [ ] Cross-language transforms
> - [ ] Running pipelines authored in any SDK on any runner
> - [ ] Implement new Beam transforms using a language of choice and utilize these transforms from other languages

## Separating Compute and Storage with Dataflow

In this module we discuss how to separate compute and storage with Dataflow. This module contains four sections Dataflow, Dataflow Shuffle Service, Dataflow Streaming Engine, Flexible Resource Scheduling. 

### Video - [Separating Storage and Compute with Dataflow](https://www.cloudskillsboost.google/course_templates/218/video/520336)

- [YouTube: Separating Storage and Compute with Dataflow](https://www.youtube.com/watch?v=v0D8x62w4Zo)

Federico: Now, let's discuss how to separate compute and storage with Dataflow. This module contains four sections. In this video, we talk about Dataflow. Dataflow allows you to execute your VM pipelines on Google Cloud. There are several reasons why customers love Dataflow so much. First, it's because it is fully managed and autoconfigured. Second, Dataflow optimizes the graph execution by fusing operations efficiently and by not waiting for previous steps to finish before starting a new one unless there is a dependency involved. Third, autoscaling happens step by step in the middle of a pipeline job. As a job needs more resources, it receives them automatically. You don't have to manually scale resources to match job needs, and you don't pay for VM resources that aren't being used. Dataflow will turn down the workers as the job demand decreases. All of this happens while maintaining strong streaming semantics Aggregations like sums and counts are correct, even if the input source sends duplicate records. As we mentioned in a previous course, Dataflow can also handle later-arriving records with intelligent watermarking. Now, let's talk about how to separate compute and storage and save money and time with Dataflow shuffle service, Dataflow streaming engine, and flexible resource scheduling.

### Video - [Dataflow Shuffle Service](https://www.cloudskillsboost.google/course_templates/218/video/520337)

- [YouTube: Dataflow Shuffle Service](https://www.youtube.com/watch?v=dV9RkG-3nh0)

person: In this video, we look at the Dataflow Shuffle service. A shuffle is a Dataflow-based operation behind transforms such as GroupByKey, CoGroupByKey, and Combine. The Dataflow Shuffle operation partitions and groups data by key in a scalable, efficient, fault-tolerant manner. Currently, Dataflow uses a shuffle implementation that runs entirely on worker virtual machines and consumes worker CPU, memory, and persistent disk storage. The service-based Dataflow Shuffle feature available for batch pipelines only moves the shuffle operations out of the worker VMs and into the Dataflow service backend. With the Dataflow Shuffle service, you will have faster execution time of batch pipelines for the majority of the job types. The worker nodes will benefit from a reduction in consumed CPU, memory, and persistent disk storage resources, and your pipelines will have better autoscaling because the worker nodes VMs no longer hold any shuffle data, and can therefore be scaled down earlier. Also, because of the service, you will get better fault tolerance. An unhealthy VM holding Dataflow Shuffle data will not cause the entire job to fail, which would happen without the feature. See the Dataflow official documentation to learn how to enable the Dataflow Shuffle service for your batch pipelines.

### Video - [Dataflow Streaming Engine](https://www.cloudskillsboost.google/course_templates/218/video/520338)

- [YouTube: Dataflow Streaming Engine](https://www.youtube.com/watch?v=t_aWDwOYcwQ)

person: In this video, we look at the dataflow streaming engine. Just like shuffle component in batch, the streaming engine offloads the window state storage from the persistent disks attached to worker VMs to a back-end service. It also implements an efficient shuffle for streaming cases. Luckily, no code changes are required. Worker nodes continue running your user code and implements data transforms and transparently communicate with a streaming engine to source state. With the dataflow streaming engine, you will have a reduction in consumed CPU, memory, and persistent disk storage resources on the worker VMs. Streaming engine works best with smaller worker machine types like n1-standard-2, and does not require persistent disks beyond a smaller worker boot disk. This leads to a lower resource and quota consumption. With streaming engine, your pipeline will be more responsive to variations to incoming data volume. Finally, you will have improved supportability, since you don't need to redeploy your pipelines to applied service updates. To activate dataflow streaming engine, see dataflow official documentation.

### Video - [Flexible Resource Scheduling](https://www.cloudskillsboost.google/course_templates/218/video/520339)

- [YouTube: Flexible Resource Scheduling](https://www.youtube.com/watch?v=MJNXqM7ie7Y)

person: Now let's talk about Flexible Resource Scheduling, or in short, FlexRS. FlexRS helps you reduce the cost of your batch processing pipelines because you can use advanced scheduling techniques in the Dataflow Shuffle Service and leverage a mix of preemptible and normal virtual machines. When you submit a FlexRS job, the Dataflow service places the job into a queue and submits it for execution within six hours from job creation. This makes FlexRS suitable for workloads that are not time-critical, such as daily or weekly jobs that can be completed within a certain time window. As soon as you submit your FlexRS job, Dataflow records a job ID and performs an early validation run to verify execution parameters, configurations, quota and permissions. In case of failure, the error is reported immediately, and you don't have to wait for a delayed execution. To enable FlexRS, please refer to Dataflow official documentation.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/218/quizzes/520340)

#### Quiz 1.

> [!important]
> **What are the benefits of Dataflow Streaming Engine? (Select ALL that apply.)**
>
> - [ ] More responsive autoscaling for incoming data variations
> - [ ] Lower resource and quota consumption
> - [ ] Reduced consumption of worker CPU, memory, and storage

#### Quiz 2.

> [!important]
> **Which of the following are TRUE about Flexible Resource Scheduling? (Select ALL that apply.)**
>
> - [ ] FlexRS leverages a mix of preemptible and normal VMs.
> - [ ] FlexRS is most suitable for workloads that are time-critical.
> - [ ] FlexRS helps to reduce batch processing costs by using advanced scheduling techniques.
> - [ ] When you submit a FlexRS job, the Dataflow service places the job into a queue and submits it for execution within 6 hours from job creation.

#### Quiz 3.

> [!important]
> **The Dataflow Shuffle service is available only for batch jobs.**
>
> - [ ] False
> - [ ] True

## IAM, Quotas, and Permissions

In this module, we talk about the different IAM roles, quotas, and permissions required to run Dataflow

### Video - [IAM](https://www.cloudskillsboost.google/course_templates/218/video/520341)

- [YouTube: IAM](https://www.youtube.com/watch?v=vCJEJ7BL4BU)

Omar: Hello, there. My name is Omar Ismail, a solutions developer at Google Cloud. In this module, we talk about the different IAM roles, quotas, and permissions required to run Dataflow, Google's batch and streaming analytic service based on Apache Beam. In this video, we learn how IAM provides access to the different Dataflow resources. You have your Beam code, and now you want to run it on Dataflow. Let us look at what happens when your Beam code is submitted. When the pipeline is submitted, it is sent to two places. The SDK uploads your code to Cloud storage and sends it to the Dataflow service. The Dataflow service does a few things. It validates and optimizes the pipeline, it creates the Compute Engine virtual machines in your projects to run your code, it deploys the code to the VMs, and it starts to gather monitoring information for display. When all that is done, the VMs will start running your code. At each of the stages we mentioned-- user submission of code, Dataflow validating the pipeline, and the VM running-- IAM plays a role in determining whether to continue the process. We will briefly explain how IAM comes into play at each stage. Three credentials determine whether a Dataflow job can be launched. The first credential that is checked is the user role. When you submit a code, whether you are allowed to submit it is determined by the IAM role set to your account. On Google Cloud, your account is represented by your email address. For example, when I submit a Dataflow job, it is done via Omar@mysuccessfulcompany.com. Three user roles can be assigned to each user or group. Each role is made up of a set of permissions that determine how much access each user or group has to the different Dataflow resources. The first role you can assign to a user or group is the Dataflow viewer role. If you want a user or group to be able to only view Dataflow jobs, assign them the Dataflow viewer role. This role prevents submitting, updating, and cancelling jobs. It allows users who have the role to only view Dataflow jobs either in the UI or by using the command line interface. The next role you can assign to a user or group is the Dataflow developer role. This role is ideal for a person who is responsible for managing pipelines that are running. For a job to run on Dataflow, the user must be able to submit the job to Dataflow, stage files to cloud storage, and view the available Compute Engine quota. If a user only has the Dataflow developer role, they can view and cancel jobs that are currently running, but they cannot create jobs because the role does not have permissions to stage the files and view the Compute Engine quota. You can use the Dataflow developer role as a building block to compose custom roles. For example, if you also want to be able to create pipelines, you can create a role that has the permissions from the Dataflow developer role plus the permissions required to stage files to a bucket and to view the Compute Engine quota. The last role you can assign to a user or group is the Dataflow admin role. Use this role to provide a user or group with the minimum set of permissions that allow both creating and managing Dataflow jobs. The Dataflow admin role allows a user or group to interact with Dataflow and stage files in an existing Cloud storage bucket and view the Compute Engine quota. The second credential Dataflow uses is the Dataflow service account. Dataflow uses the Dataflow service account to interact between your project and Dataflow. For example, to check project quota, to create worker instances on your behalf, and to manage the job during job execution. When you run your pipeline on Dataflow, it uses the service account service- @dataflow-service-producer-prod . iam.gserviceaccount.com. This account is automatically created when the Dataflow API is enabled. It is assigned the Dataflow service agent role and has the necessary permissions to run a Dataflow job in your project. In our job overview diagram, the Dataflow service account is responsible for the interaction happening here between your project and Dataflow. The last credential used to run Dataflow jobs is the controller service account. The controller service account is assigned to the Compute Engine VMs to run your Dataflow pipeline. By default, workers use your project's Compute Engine default service account as the controller service account. This service account, <project-number>-compute @developer.gservices.com, is automatically created when you enable the Compute Engine API for your project from the API's page in the Google Cloud console. The Compute Engine default service account has broad access to your project's resources, which makes it easy to get started with Dataflow. However, for production workloads, we recommend that you create a new service account with only the roles and permissions that you need. At a minimum, your service account must have the Dataflow worker role and can be used by adding the service account email flag when launching a Dataflow pipeline. When using your own service account, you might also need to add additional roles to access different Google Cloud resources. For example, if your job reads from BigQuery, your service account must also have a role like the BigQuery Data Viewer role. Let us review. In our job overview diagram, where would the controller service account be? Here.

### Video - [Quotas](https://www.cloudskillsboost.google/course_templates/218/video/520342)

- [YouTube: Quotas](https://www.youtube.com/watch?v=MZN1Jfm-w8U)

In the second section of this module, we look at the quotas to consider when running Dataflow. Let’s get started! One of the quotas that Dataflow consumes is CPU. CPU quota is the total number of virtual CPUs across all of your VM instances in a region or zone. Any Google Cloud product that creates a Compute Engine VM, such as Dataproc, GKE, or AI Notebooks, consumes this quota. CPU quota can be viewed in the UI on the IAM Quota page. For example, right now, I am consuming 219 CPUs in the northmaerica-northeast1 region. Say you want to start a Dataflow job with 100 workers. If the VM size selected is n1-standard-1, meaning 1 CPU core per VM, the CPU usage will be 100. If the VM size selected is n1-standard-8, that would mean 800 CPUs are needed. If the limit is 600, the job will display an error because the CPU limit has been exceeded. Another quota to consider is the number of in-use IP addresses in each region. The in-use IP address quota limits the number of VMs that can be launched with an external IP address for each region in your project. Like the CPU quota, this quota is shared across all Google Cloud products that create VMs with an external IP address. When you launch a Dataflow job, the default setting is for the VM to launch with an external IP address. Jobs that access APIs and services outside Google Cloud require internet access. However, if your job does not need to access any external APIs or services, you can launch the Dataflow job using internal IPs only, which saves money and conserves the In-use IP address quota. In our next module, we will show you how to launch VMs with internal IPs only. Unlike the CPU quota, the in-use IP address quota is independent of the machine type; there is no difference between launching 150 n1-standard-1s vs 150 n1-standard-8s. In the slide image here, the In-use IP address limit for a few regions is 575. In the previous slide for CPU quota, the maximum number of CPUs per region was 600. When you launch a Dataflow job, the more restrictive quota takes precedence. Let us look at quotas for persistent disks. You can choose between two different types of Persistent Disks when running Dataflow jobs. You can launch jobs with either legacy Hard Disk Drives or modern Solid State Drives. Each disk type has a limit per region that can be used. For example, in the image shown here, Google Cloud products in my project that use HDDs in northamerica-northeast1 are consuming 23.5 TB of disk space out of the available 102.4TB To specify the disk type, set the worker_disk_type flag to the prefix shown in the image, and end it with either pd-ssd or pd-standard. Use Pd-standard for Hard Disk Drives and pd-ssd for Solid State Drives. In the slide example, we set the disk type to SSD using both Python and Java. When you launch a batch pipeline, the ratio of VMs to PDs is 1:1. For each VM, only one persistent disk is attached. For jobs running shuffle on worker VMs, the default size of each persistent disk is 250 GB. If the Batch job is running using Shuffle Service, the default PD size is 25 GB. Recall that Dataflow Shuffle moves the shuffle operation out of the worker VMs and into the Dataflow service backend, which is why the default persistent disk size attached to the VM is smaller. Note that you can use the disk_size_gb flag to override the default persistent disk size for batch pipelines using either shuffle on VM or Dataflow Shuffle. Streaming pipelines, however, are deployed with a fixed pool of Persistent Disks. Each worker must have at least 1 persistent disk attached to it, while the maximum is 15 persistent disks per worker instance. As with Batch jobs, Streaming jobs can be run either on the worker VMs or on the Dataflow backend. When you run a job using the Dataflow backend, the feature that is used is Dataflow's Streaming Engine. Streaming Engine moves pipeline execution out of the worker VMs and into the Dataflow service backend. For jobs launched to execute in the worker VMs, the default persistent disk size is 400 GB. Jobs launched using Streaming Engine have a persistent disk size of 30 GB. Just like with Batch pipelines, these default persistent disk limits can be overridden using the disk_size_gb flag. It is important to note that the amount of disk allocated in a streaming pipeline is equal to the max_num_workers flag. For example, if you launch a job with 3 workers initially and set the maximum number of workers to 25, 25 disks will count against your quota, not 3. To set the maximum number of workers that a pipeline can use, use the --max_num_workers flag. This cannot be above 1000. When you launch a streaming job that does not use Streaming Engine, the flag --max_num_workers is required. For streaming jobs that do use Streaming Engine, the --max_num_workers flag is optional. The default is 100.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/218/quizzes/520343)

#### Quiz 1.

> [!important]
> **Your project's current SSD usage is 100 TB. You want to launch a streaming pipeline with shuffle done on the VM. You set the initial number of workers to 5 and the maximum number of workers to 100. What will be your project's SSD usage when the job launches?**
>
> - [ ] 500 TB
> - [ ] 140 TB
> - [ ] 102 TB
> - [ ] 103 TB

#### Quiz 2.

> [!important]
> **You want to run the following command:gcloud dataflow jobs cancel 2021-01-31_14_30_00-9098096469011826084--region=$REGIONWhich of these roles can be assigned to you for the command to work?**
>
> - [ ] Composer Worker
> - [ ] Dataflow Developer
> - [ ] Dataflow Viewer
> - [ ] Dataflow Admin

## Security

In this module, we will look at how to implement the right security model for your use case on Dataflow.

### Video - [Data Locality](https://www.cloudskillsboost.google/course_templates/218/video/520344)

- [YouTube: Data Locality](https://www.youtube.com/watch?v=fFn2mf1TIrc)

Omar: Hey there. My name is Omar Ismail, a solutions developer at Google Cloud. In this module, we talk about the different ways you can enhance security while running Dataflow. We discuss four security features in this module. Let us get started with data locality. Data locality ensures that all data and metadata stay in one region. When you launch a Dataflow job, a backend exists in a Google-managed project that deploys and controls your pipeline. As we discussed in the IAM module, the Dataflow service account communicates between your project and the Dataflow backend. The Dataflow backend exists in a few regions across the globe and can be different from the region in which your workers run. What metadata is transferred between your project and the regional endpoint? There are regular health checks from the workers, workers requesting a work item and the regional endpoint responding with a work item, the worker item status, and autoscaling events. Unexpected events are also transferred to the regional endpoint. For example, unhandled exceptions in user code, jobs that fail to launch because of permissions, worker item failures, and errors from another related system, such as Compute Engine. These items are stored at the regional endpoint and are visible to you on the Dataflow UI, along with any other info you see in the UI, such as pipeline parameter values, job name, job ID, and start time. There are a couple of reasons for specifying a regional endpoint. The first is to support your project's security and compliance needs. For example, if you work for a bank in certain countries, regulatory rules mandate that data does not leave the country of operation. These rules can be met by specifying the regional endpoint. You can also specify a regional endpoint to minimize network latency and network transport costs. If your pipeline sources, syncs, and staging locations are all in the same region, you will not be charged for network egress because all the info remains in the same region. If you have a pipeline with workers in northamerica-northeast and its regional endpoint is set to us-central1, your network egress charge will increase because of the metadata that is transferred between your project and the regional endpoint. In the next couple of slides, we will show you how to specify the regional endpoint you want the Dataflow service to run in. If you want to use a supported regional endpoint and have no zone preference within the region, specify the regional flag only. In this case, the regional endpoint automatically selects the best zone based on available capacity. In Apache Beam 2.15 and greater, specifying this flag is mandatory. If you need worker processing to occur in a specific zone of a region that has a regional endpoint, specify both region and worker zone flags. Use the region flag to specify the regional endpoint, and use the worker zone flag to specify the specific zone within that region. If you need worker processing to occur in a specific region that does not have a regional endpoint, specify both region and worker region flags. Use the region flag to specify the supported regional endpoint that is closest to the region where the worker processing must occur. Use worker region flag to specify a region where worker processing must occur. Compared to the scenarios on the two previous slides, specifying a different region for the regional endpoint and the worker has the protentional to create greater latency. It is important to note that even if no regional endpoint exists in a region you want your data to be kept in, only metadata is transferred. Your application data stays in that region.

### Video - [Shared VPC](https://www.cloudskillsboost.google/course_templates/218/video/520345)

- [YouTube: Shared VPC](https://www.youtube.com/watch?v=9Rhs482l8vU)

person: Another security feature you can use with Dataflow is shared VPC. Dataflow can run in networks that are either in the same project or in a separate project which we call the host project. When a network exists in a host project, we call the networking setup shared VPC. Shared VPC lets organization admins delegate administrative responsibilities, such as creating and managing instances, to others while maintaining centralized control over network resources like subnets, routes, and firewalls. When set to run in a shared VPC, Dataflow works in either a default or a custom network. The default network is the one automatically set by Google Cloud when you create a project. A custom network is one where you create the network and define the regions and the subnets in the network. When setting the number of workers to use, remember to have enough IP addresses available. For example, if you have a subnet with a /29 subnet and no other VMs running in it, the maximum number of Dataflow workers that you can launch is four. Finally, the Dataflow service account needs the Compute Network user role in the host project on either a project level or a subnet level. We show the difference between using the network and subnetwork flags here. In the Python example, the Dataflow service account has a compute network role set at the project level, and the user wants to deploy to the default network. In the Java example, the Dataflow service account's permissions are defined at the subnet level, and the user is launching the job in a custom subnet.

### Video - [Private IPs](https://www.cloudskillsboost.google/course_templates/218/video/520346)

- [YouTube: Private IPs](https://www.youtube.com/watch?v=eRxjBww2n8Y)

person: Another security feature you can use with Dataflow is disabling external IP usage. This blocks the workers from accessing the internet, thus securing your data processing infrastructure. By not using public IP addresses for your Dataflow workers, you also lower the number of public IP addresses you consume against your in-use IP address quota. With public IPs turned off, you can still perform administrative and monitoring tasks on Dataflow. By default, the Dataflow service assigns workers both public and private IP addresses. When you turn off public IP addresses, the Dataflow pipeline can access resources only in the following places: another instance in the same VPC network, a shared VPC network, or a network with VPC network peering enabled. If your pipeline is communicating with other Google services and APIs and is in a custom network, Private Google Access must be enabled for the subnetwork your worker will be launched in. If you disable Private Google Access and have no other way of reaching the internet, such as Cloud NAT, the VM instances can no longer reach Google Cloud APIs and services. To use private IPs only, two flags need to be added. The first flag to specify is either the network or subnetwork the workers should run in. The second flag, no_use_public_ips, lets Dataflow know that you want to launch the workers with internal IP addresses only.

### Video - [CMEK](https://www.cloudskillsboost.google/course_templates/218/video/520347)

- [YouTube: CMEK](https://www.youtube.com/watch?v=ebLagAockpo)

person: The last security feature we look at is CMEK. CMEK stands for customer managed encryption key. During a Dataflow job's lifecycle, different storage locations are used to store data. When a Dataflow job is created, a cloud storage bucket is used to store binary files containing pipeline code. A cloud storage bucket is also used to temporarily store export or import data. While the job is running, persistent disks attached to Dataflow workers are used for persistent disk-based shuffle and streaming state storage. If a batch job is using Dataflow Shuffle, the backend stores the batch pipeline state during execution. If a job is using Dataflow Streaming Engine, the backend stores the streaming pipeline state during execution. By default, when data is stored in any of these locations, a Google-managed key is used to encrypt the data. CMEK allows you to encrypt data at rest using one of your symmetric keys stored in Google Cloud key management system. This means that you can use CMEK in any of the data storage locations mentioned. When your pipeline starts and the data is loaded into the worker memory, data keys used in key-based operations, such as windowing, grouping, and joining, will be decrypted using your CMEK keys. For an additional layer of security, you can hash or transform the key. Job metadata is encrypted with Google encryption. Job metadata includes the following: user-supplied data, such as job names, job parameter values, and pipeline graphs, and system generated data, such as job IDs and IP addresses of workers. Using CMEK requires both the Dataflow service account and the Controller Agent service account to have the cloud KMS CryptoKey Encrypter/Decrypter role. To use CMEK, two flags need to be specified. First, specify the cloud storage path for Dataflow to stage temporary files created during the execution of the pipeline using the temp location flag. Second, specify the location of the key in Google's key management service using the Dataflow KMS key flag. When you launch a job that uses CMEK, the region for your key and the regional input for your Dataflow job must be the same. Global or multiregional keys will not work. The bucket selected to temporarily store data must also be in the same region as the key. If you override the pipeline's worker region or zone to a different region than the region associated with your keys, regional keys will not work.

### Lab - [Setup IAM and Networking for your Dataflow Jobs](https://www.cloudskillsboost.google/course_templates/218/labs/520348)

In this lab, you will learn to setup IAM permissions and use private IPs for your Datafow jobs.

- [ ] [Setup IAM and Networking for your Dataflow Jobs](../labs/Setup-IAM-and-Networking-for-your-Dataflow-Jobs.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/218/quizzes/520349)

#### Quiz 1.

> [!important]
> **Your project's current In-use IP address usage is 500/575. You run the following command:
python3 -m apache_beam.examples.wordcount \
--input gs://dataflow-samples/shakespeare/kinglear.txt \
--output gs://$BUCKET/results/outputs --runner DataflowRunner  \
--project $PROJECT  --temp_location gs://$BUCKET/tmp/  --region $REGION \
--subnetwork regions/$REGION/subnetworks/$SUBNETWORK \
--num_workers 20    --machine_type n1-standard-4   --no_use_public_ips
What will be the in-use IP address usage after the job starts?**
>
> - [ ] 520/575
> - [ ] The job will fail to launch.
> - [ ] 500/575

#### Quiz 2.

> [!important]
> **You are a Beam developer for a university in Googleville. Googleville law mandates that all student data is kept within Googleville. Compute Engine resources can be launched in Googleville; the region name is google-world1. Dataflow, however, does not currently have a regional endpoint set up in google-world1. Which flags are needed in the following command to allow you to launch a Dataflow job and to conform with Googleville's law?
python3 -m apache_beam.examples.wordcount \
--input gs://dataflow-samples/shakespeare/kinglear.txt \
 --output gs://$BUCKET/results/outputs --runner DataflowRunner  \
 --project $PROJECT  --temp_location gs://$BUCKET/tmp/  \**
>
> - [ ] --region northamerica-northeast1
> - [ ] --region google-world1  --worker_zone google-world1
> - [ ] --region northamerica-northeast1  --worker_region google-world1

## Summary

In this course, we started with the refresher of what Apache Beam is, and its relationship with Dataflow. 

### Video - [Course Summary](https://www.cloudskillsboost.google/course_templates/218/video/520350)

- [YouTube: Course Summary](https://www.youtube.com/watch?v=ifv7vuTUVeM)

Mehran: Hi, it's Mehran again. Congratulations, you've made it to the end of the foundation's course of serverless data processing. What data flow? Let's recap what you've learned. In this course, we started with the refresher of what Apache Beam is and its relationship with dataflow. Apache Beam is an open source programing model with the unified approach for batch and streaming pipelines so that you don't have to manage multiple data processing architectures, no more land architectures. Data flow is a fully managed, distributed data processing engine for Apache beam pipelines integrated within the Google cloud. Ecosystem data will automates the provisioning and orchestration of worker machines and uses techniques like horizontal auto scaling in dynamic work rebalancing to achieve the lowest total cost of ownership. Next, we talked about the Apache beam vision and the benefits of the beam portability framework. Thanks to the interoperability layer introduced by the Portability API, digital pipelines can leverage new features such as custom containers and multi-language pipelines. The Beam Portability Framework achieves the vision that a developer can use their favorite programing language with the preferred execution backend. Dataflow is runner review to implementation offers this portable architecture on dataflow, it can be enabled via pipeline option without rewriting a single line of code. Another aspect that we looked at is how do you feel allows you to separate, compute and storage while saving money? The shuttle service helps Batz pipelined scale seamlessly to hundreds of terabytes without any testing required by offloading the shuttle operation from worker VMS onto the dataflow service back end. Because operations are carried out on a service back end, pipelines consume less CPU memory and persistent storage. The same principle applies for streaming pipelines with streaming engine, which offloads Windows state storage from the persistent disk attached to workers onto a back end service, this significantly improves auto scaling and data latency and also reduces the resource footprint for your streaming pipeline. We finish this module with flexible resource scheduling or flex hours that can help you save in costs for your pipelines by using a combination of preemptive VMS and our shuffle back end. And the best thing about all these features is that you can enable them for your pipeline to that rewriting a line of code, all you need to do is pass a new parameter when you deploy the pipeline. We reviewed how identity access and management tools interact with your data flow pipelines. We learn about different predefined rules for data flow users and the different service accounts used to run data for pipelines. Then we looked at which quotas apply to data flow jobs. Specifically, VCP use IPS and persistent disks. Every capacity planning exercise it involves data flow. Workloads should involve estimating consumption needs for these resources. Lastly, we looked at how to implement the right security model for your use case on dataflow. We learn how to comply with the locality requirements by specifying the region in zone parameters in your job, and we learn about how to run dataflow jobs with various VPC configurations. We learn how to prevent data exfiltration by disabling public IPS on your dataflow workers. We ended our discussion on security by covering data encryption on data flow. By default, all data is encrypted with Google managed keys, but data integration with cloud key management service allows you to bring your own encryption keys to ensure the maximum level of security. I hope you enjoy this course and you'll be able to put into practice what you've learned.

### Document - [Additional Resources](https://www.cloudskillsboost.google/course_templates/218/documents/520351)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
