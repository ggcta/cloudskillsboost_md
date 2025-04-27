---
id: 526
name: 'Google Cloud Compute and Scalability for AWS Professionals'
datePublished: 2023-09-22
topics:
- Managed Instance Groups
- Load Balancing
- Networking
type: Course
url: https://www.cloudskillsboost.google/course_templates/526
---

# [Google Cloud Compute and Scalability for AWS Professionals](https://www.cloudskillsboost.google/course_templates/526)

**Description:**

This is the second course of a four-course series for cloud architects and engineers with existing AWS knowledge. It aims to compare Google Cloud and AWS solutions and guide professionals on their use.

This course focuses on compute resources and load balancing in Google Cloud. The learner will apply the knowledge of using virtual machines and load balancers in AWS to explore the similarities and differences with configuring and managing compute resources and load balancers in Google Cloud. Learners will get hands-on practice building and managing Google Cloud resources.

**Objectives:**

- Create and configure a Compute Engine instance in Google Cloud.
- Explain the difference between Google Cloud images and AWS AMI.
- Compare and contrast Cloud Load Balancing with AWS Load Balancers.
- Explain the best use case for each specific type of load balancer (HTTP, TCP, SSL, Network, and Internal).
- Describe managed instance groups (MIGs) and how to use them.

## Virtual Machines in Google Cloud

In this module, you will apply your knowledge of working with virtual machines in AWS to explore the similarities and differences with virtual machines in Google Cloud. You will learn about Google Virtual Private Cloud (VPC), routing and firewalls in Google Cloud, and the variety of options Google Cloud offers for connecting networks.

### Document - [Course Introduction](https://www.cloudskillsboost.google/course_templates/526/documents/410908)

### Link - [Virtual Machines in Google Cloud](https://www.cloudskillsboost.google/course_templates/526/documents/410909)

- [Virtual Machines in Google Cloud](https://storage.googleapis.com/cloud-training/T-INFRAWS2-I/1.0.1/od/en/web/MODULE01/content/index.html)

### Lab - [Google Cloud Fundamentals: Getting Started with Compute Engine (AWS)](https://www.cloudskillsboost.google/course_templates/526/labs/410910)

In this lab, you will create virtual machines (VMs) and connect to them.  You will also create connections between the instances.

- [ ] [Google Cloud Fundamentals: Getting Started with Compute Engine (AWS)](../labs/Google-Cloud-Fundamentals-Getting-Started-with-Compute-Engine-(AWS).md)

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/526/quizzes/410911)

#### Quiz 1.

> [!important]
> **You need to create virtual machines that are optimized for high-end remote visualization, deep learning, and predictive analytics. What machine family in Compute Engine should you use?**
>
> - [ ] C series
> - [ ] E series
> - [ ] M series
> - [ ] A2 series

#### Quiz 2.

> [!important]
> **You need to take your existing Amazon EC2 launch templates and reimplement them for a Google Cloud solution. Which Google Cloud tool can you use?**
>
> - [ ] Spot VM
> - [ ] Instance Templates
> - [ ] Managed instance groups
> - [ ] Differential backup

#### Quiz 3.

> [!important]
> **You have been asked to train a junior team member who is familiar with AWS in the lifecycle of a Google Cloud virtual machine (VM). How can you describe the equivalent of the Amazon EC2 instance shutting-down state in Google Cloud?**
>
> - [ ] Terminating
> - [ ] Delete
> - [ ] Pending
> - [ ] Preemption

#### Quiz 4.

> [!important]
> **You currently store data from Amazon EC2 instances in an EBS volume with automated snapshots providing availability across availability zones. You need to reimplement this scenario using Google Compute Engine. What should you use?**
>
> - [ ] Spot VMs
> - [ ] Zonal persistent disks
> - [ ] Local SSD
> - [ ] Regional persistent disks

#### Quiz 5.

> [!important]
> **You have a Virtual Machine that is running data pipeline batch Extract, Transform, and Load (ETL) jobs. If the VM fails, the ETL package should gracefully recover the data pipeline and it will restart at the point of failure. You want to choose the most cost-effective solution in Google Cloud. What should you do?**
>
> - [ ] Set up a Compute Engine instance with GPUs.
> - [ ] Set up a VM and put it into sole tenancy.
> - [ ] Create a managed instance group.
> - [ ] Use a Spot VM to deliver the batch data pipeline job.

### Document - [Module 1 Student Guide](https://www.cloudskillsboost.google/course_templates/526/documents/410912)

## Load Balancing and Managed Instance Groups in Google Cloud

In this module, you will apply your knowledge of load balancing and autoscaling instances in AWS to explore the similarities and differences with using load balancers and managed instance groups (MIGs) in Google Cloud. You will learn about the variety of options available in Cloud Load Balancing to distribute external and internal traffic. You will also learn how to create MIGs and use them effectively with load balancing services.

### Link - [Load Balancing and Managed Instance Groups in Google Cloud](https://www.cloudskillsboost.google/course_templates/526/documents/410913)

- [Load Balancing and Managed Instance Groups in Google Cloud](https://storage.googleapis.com/cloud-training/T-INFRAWS2-I/1.0/od/en/web/MODULE02/content/index.html)

### Lab - [Configure an Application Load Balancer with Autoscaling (AWS)](https://www.cloudskillsboost.google/course_templates/526/labs/410914)

In this lab, you configure an Application Load Balancer (HTTP). Then, you stress test the Load Balancer to demonstrate global load balancing and autoscaling.

- [ ] [Configure an Application Load Balancer with Autoscaling (AWS)](../labs/Configure-an-Application-Load-Balancer-with-Autoscaling-(AWS).md)

### Lab - [Configure an Internal Network Load Balancer (AWS)](https://www.cloudskillsboost.google/course_templates/526/labs/410915)

In this lab, you create two managed instance groups in the same region. Then, you configure an Internal Network Load Balancer with the instances groups as the backends.

- [ ] [Configure an Internal Network Load Balancer (AWS)](../labs/Configure-an-Internal-Network-Load-Balancer-(AWS).md)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/526/quizzes/410916)

#### Quiz 1.

> [!important]
> **You need to automatically create virtual machines (VMs) in Google Cloud when demand increases for your application and delete VMs when demand drops. You want to have the VMs grouped together for convenient management. What should you use?**
>
> - [ ] Managed instance group with stateful configuration
> - [ ] A regional managed instance group
> - [ ] A managed instance group that uses preemptible VMs
> - [ ] A managed instance group with autoscaling enabled

#### Quiz 2.

> [!important]
> **You need to set up a load balancer that operates at layer 4 of the Open Systems Interconnection (OSI) model. The load balancer needs to handle SSL layer traffic. What option should you choose in Google Cloud?**
>
> - [ ] External TCP Proxy Load Balancing
> - [ ] External SSL Proxy Load Balancing
> - [ ] Internal TCP Proxy Load Balancing
> - [ ] External TCP/UDP Network Load Balancing

#### Quiz 3.

> [!important]
> **You need to apply load balancing to groups of heterogeneous instances in Google Cloud. Which option can you use?**
>
> - [ ] Unmanaged instance group
> - [ ] Managed instance group in a single zone
> - [ ] Managed instance group
> - [ ] Managed instance group in multiple zones

#### Quiz 4.

> [!important]
> **Which Google Cloud load balancing services support IPv6 clients? (Choose two).**
>
> - [ ] Network load balancing
> - [ ] SSL proxy load balancing
> - [ ] Internal load balancing
> - [ ] Global HTTP(S) load balancing
> - [ ] Regional HTTP(S) load balancing

#### Quiz 5.

> [!important]
> **Your organization uses AWS Application Load Balancer to load balance between your servers in a region at the application layer. You need to implement similar load balancing functionality in Google Cloud. What technology should you use?**
>
> - [ ] Application Capacity Optimizations with Global Load Balancing
> - [ ] Internal TCP Proxy Load Balancing
> - [ ] External SSL Proxy Load Balancing
> - [ ] Internal HTTP(S) Load Balancing

### Document - [Module 2 Student Guide](https://www.cloudskillsboost.google/course_templates/526/documents/410917)

### Document - [What Next](https://www.cloudskillsboost.google/course_templates/526/documents/410918)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
