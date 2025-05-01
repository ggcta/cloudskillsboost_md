---
id: 525
name: 'Google Cloud Compute and Scalability for Azure Professionals'
type: Course
url: https://www.cloudskillsboost.google/course_templates/525
date_published: 2023-09-25
topics:
  - Networking
  - Compute Instances
  - Managed Instance Groups
---

# [Google Cloud Compute and Scalability for Azure Professionals](https://www.cloudskillsboost.google/course_templates/525)

**Description:**

This is the second course of a four-course series for cloud architects and engineers with existing Azure knowledge. It aims to compare Google Cloud and Azure solutions and guide professionals on their use.

This course focuses on compute resources and load balancing in Google Cloud. The learner will apply the knowledge of using virtual machines and load balancers in Azure to explore the similarities and differences with configuring and managing compute resources and load balancers in Google Cloud. Learners will get hands-on practice building and managing Google Cloud resources.

**Objectives:**

* Create and configure a Compute Engine instance in Google Cloud.
* Explain the difference between Google Cloud images and Azure Custom Images.
* Compare and contrast Cloud Load Balancing with Azure Load Balancers.
* Explain the best use case for each specific type of load balancer (HTTP, TCP, SSL, Network, and Internal).
* Describe managed instance groups (MIGs) and how to use them.

## Virtual Machines in Google Cloud

In this module, you will apply your knowledge of working with virtual machines in Azure to explore the similarities and differences with virtual machines in Google Cloud. You will learn about Google Virtual Private Cloud (VPC), routing and firewalls in Google Cloud, and the variety of options Google Cloud offers for connecting networks.

### Link - [Virtual Machines in Google Cloud](https://www.cloudskillsboost.google/course_templates/525/documents/411222)

* [Virtual Machines in Google Cloud](https://storage.googleapis.com/cloud-training/T-INFRAZR2-I/1.0.1/od/en/web/MODULE01/content/index.html)

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/525/quizzes/411223)

#### Quiz 1.

> [!important]
> **You store data from Azure virtual machines in an Azure zone-redundant storage, which distributes data over different zones in the same region. You need to reimplement this scenario using Google Compute Engine. What should you use?**
>
> * [ ] Local SSD
> * [ ] Zonal persistent disks
> * [ ] Regional persistent disks
> * [ ] Spot VMs

#### Quiz 2.

> [!important]
> **You have been asked to train a junior team member who is familiar with Azure in the lifecycle of a Google Cloud virtual machine (VM). How can you describe the equivalent of the Azure VM's deallocating state in Google Cloud?**
>
> * [ ] Deallocating
> * [ ] Terminating
> * [ ] Preemption
> * [ ] Delete

#### Quiz 3.

> [!important]
> **You need to take your existing Azure Virtual Machine Resource Manager templates and reimplement them for a Google Cloud solution. Which Google Cloud tool can you use?**
>
> * [ ] Managed instance groups
> * [ ] Instance Templates
> * [ ] Differential backup
> * [ ] Spot VM

#### Quiz 4.

> [!important]
> **You need to create virtual machines that are optimized for high-end remote visualization, deep learning, and predictive analytics. What machine family in Compute Engine should you use?**
>
> * [ ] A2 series
> * [ ] M series
> * [ ] E series
> * [ ] C series

#### Quiz 5.

> [!important]
> **You have a Virtual Machine that is running data pipeline batch Extract, Transform, and Load (ETL) jobs. If the VM fails, the ETL package will gracefully recover the data pipeline and it will restart at the point of failure. You want to choose the most cost-effective solution in Google Cloud. What should you do?**
>
> * [ ] Create a managed instance group.
> * [ ] Set up a VM and put it into sole tenancy.
> * [ ] Use a Spot VM to deliver the batch data pipeline job.
> * [ ] Set up a Compute Engine instance with GPUs.

### Lab - [Google Cloud Fundamentals: Getting Started with Compute Engine (Azure)](https://www.cloudskillsboost.google/course_templates/525/labs/411224)

In this lab, you will create virtual machines (VMs) and connect to them.  You will also create connections between the instances.

* [ ] [Google Cloud Fundamentals: Getting Started with Compute Engine (Azure)](../labs/Google-Cloud-Fundamentals-Getting-Started-with-Compute-Engine-(Azure).md)

### Document - [Module 1 Student Guide](https://www.cloudskillsboost.google/course_templates/525/documents/411225)

## Load Balancing and Managed Instance Groups in Google Cloud

Compare Cloud Load Balancing with Azure Load Balancer.

### Link - [Load Balancing and Managed Instance Groups in Google Cloud](https://www.cloudskillsboost.google/course_templates/525/documents/411226)

* [Load Balancing and Managed Instance Groups in Google Cloud](https://storage.googleapis.com/cloud-training/T-INFRAZR2-I/1.0/od/en/web/MODULE02/content/index.html)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/525/quizzes/411227)

#### Quiz 1.

> [!important]
> **You need to apply load balancing to groups of heterogeneous instances in Google Cloud. Which option can you use?**
>
> * [ ] Unmanaged instance group
> * [ ] Managed instance group
> * [ ] Managed instance group in a single zone
> * [ ] Managed instance group in multiple zones

#### Quiz 2.

> [!important]
> **You need to set up a load balancer that operates at layer 4 of the Open Systems Interconnection (OSI) model. The load balancer needs to handle SSL layer traffic. What option should you choose in Google Cloud?**
>
> * [ ] Internal TCP Proxy Load Balancing
> * [ ] External SSL Proxy Load Balancing
> * [ ] External TCP Proxy Load Balancing
> * [ ] External TCP/UDP Network Load Balancing

#### Quiz 3.

> [!important]
> **Your organization uses Azure Load Balancer and Azure Application Gateway to load balance between your servers in a region at the application layer. You need to implement similar load balancing functionality in Google Cloud. What technology should you use?**
>
> * [ ] Application Capacity Optimizations with Global Load Balancing
> * [ ] External SSL Proxy Load Balancing
> * [ ] Internal TCP Proxy Load Balancing
> * [ ] Internal HTTP(S) Load Balancing

#### Quiz 4.

> [!important]
> **You need to automatically create virtual machines (VMs) in Google Cloud when demand increases for your application and delete VMs when demand drops. You want to have the VMs grouped together for convenient management. What should you use?**
>
> * [ ] A regional managed instance group
> * [ ] Managed instance group with stateful configuration
> * [ ] A managed instance group with autoscaling enabled
> * [ ] A managed instance group that uses preemptible VMs

#### Quiz 5.

> [!important]
> **Which Google Cloud load balancing services support IPv6 clients? (Choose two).**
>
> * [ ] Regional HTTP(S) load balancing
> * [ ] Internal load balancing
> * [ ] Network load balancing
> * [ ] Global HTTP(S) load balancing
> * [ ] SSL proxy load balancing

### Lab - [Configuring an HTTP Load Balancer with Autoscaling (Azure)](https://www.cloudskillsboost.google/course_templates/525/labs/411228)

In this lab, you configure an HTTP Load Balancer. Then, you stress test the Load Balancer to demonstrate global load balancing and autoscaling.

* [ ] [Configuring an HTTP Load Balancer with Autoscaling (Azure)](../labs/Configuring-an-HTTP-Load-Balancer-with-Autoscaling-(Azure).md)

### Lab - [Configuring an Internal Load Balancer (Azure)](https://www.cloudskillsboost.google/course_templates/525/labs/411229)

In this lab, you create two managed instance groups in the same region. Then, you configure an Internal Load Balancer with the instances groups as the backends.

* [ ] [Configuring an Internal Load Balancer (Azure)](../labs/Configuring-an-Internal-Load-Balancer-(Azure).md)

### Document - [Module 2 Student Guide](https://www.cloudskillsboost.google/course_templates/525/documents/411230)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
