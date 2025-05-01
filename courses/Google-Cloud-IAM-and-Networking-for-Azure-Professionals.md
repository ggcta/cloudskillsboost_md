---
id: 520
name: 'Google Cloud IAM and Networking for Azure Professionals'
type: Course
url: https://www.cloudskillsboost.google/course_templates/520
date_published: 2023-09-22
topics:
  - Networking
  - IAM
---

# [Google Cloud IAM and Networking for Azure Professionals](https://www.cloudskillsboost.google/course_templates/520)

**Description:**

This is the first course of a four-course series for cloud architects and engineers with existing Azure knowledge, and it compares Google Cloud and Azure solutions and guides professionals on their use.

This course focuses on Identity and Access Management (IAM) and networking in Google Cloud. The learners apply the knowledge of access management and networking in Azure to explore the similarities and differences with access management and networking in Google Cloud. Learners get hands-on practice building and managing Google Cloud resources.

**Objectives:**

* Explain how Google Cloud’s resource hierarchy differs from Azure.
* Explain best practices for Google Cloud’s resource hierarchy, including organizations, folders, and projects.
* Describe how to use Google Cloud Directory Sync with Azure Active Directory (AD).
* Explain the differences between Google Cloud’s IAM and Azure AD.
* Navigate through the Google Cloud console and Cloud Shell to perform basic tasks.

## Resources and Access Management in Google Cloud

In this module, you will draw on your knowledge of Azure to discuss how you can set up your resource hierarchy and configure access in Google Cloud. You will learn how resources get organized with projects, how Identity and Access Management (IAM) lets you control access to resources, and how to use service accounts in Google Cloud. You'll also explore various ways to interact with Google Cloud.

### Document - [Course Introduction](https://www.cloudskillsboost.google/course_templates/520/documents/411046)

### Link - [Resources and Access Management in Google Cloud](https://www.cloudskillsboost.google/course_templates/520/documents/411047)

* [Resources and Access Management in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-T-INFRAZR1-I-M1&utm_medium=aRT-clicks&utm_campaign=T-INFRAZR1-I-M1&destination=T-INFRAZR1-I-M1&url=https://storage.googleapis.com/cloud-training/T-INFRAZR1-I/1.0.1/od/en/web/MODULE01/content/index.html)

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/520/quizzes/411048)

#### Quiz 1.

> [!important]
> **Alexander is a Storage Administrator, responsible for managing objects in Cloud Storage. He needs to have the right permissions for every project across the organization. What should you do?**
>
> * [ ] Assign Alexander the roles/viewer on each project and the roles/storage.objectCreator for each bucket.
> * [ ] Assign Alexander the roles/storage.objectCreator on every project.
> * [ ] Assign Alexander the roles/editor at the organizational level.
> * [ ] Add Alexander to a group that has the roles/storage.objectAdmin role assigned at the organizational level.

#### Quiz 2.

> [!important]
> **In Azure, PowerShell can be used to script, automate, and manage the Windows workloads running on Azure Virtual Machines. You need to reimplement your scripts in Google Cloud. Which similar tool could you use to reimplement your scripts in Google Cloud?**
>
> * [ ] Google Cloud Console
> * [ ] Cloud SDK
> * [ ] Cloud Shell
> * [ ] Google Apps Script

#### Quiz 3.

> [!important]
> **The Azure resource hierarchy uses management groups to organize subscriptions. These management groups contain resource groups with resources. How would you create a similar hierarchy in Google Cloud?**
>
> * [ ] Subscriptions, folders, resource groups, resources
> * [ ] Folders, subscriptions, resource groups, resources
> * [ ] Folders, projects, resources
> * [ ] Projects, folders, resources

#### Quiz 4.

> [!important]
> **Consider an Azure environment, where there is an Azure Active Directory Service Principal and an Azure Managed Identity setup for a web application to access other services and resources. You need to set up an equivalent environment at Google. Which type of identity should you use in Google Cloud?**
>
> * [ ] Identity and Access Management user
> * [ ] Identity and Access Management role
> * [ ] Identity and Access Management service account
> * [ ] Identity and Access Management policy

#### Quiz 5.

> [!important]
> **Which option best describes the difference in how user identities are managed between Azure and Google Cloud?**
>
> * [ ] In Azure, user identities are managed using Active Directory; in Google Cloud, user identities are managed using policies in Identity and Access Management.
> * [ ] In Azure, user identities are managed using Active Directory; in Google Cloud, user identities are managed outside IAM.
> * [ ] In Azure, user identities are managed using Active Directory; in Google Cloud, user identities are managed using roles in Identity and Access Management.
> * [ ] In Azure, user identities are managed using Active Directory; in Google Cloud, user identities are managed using Google Groups in Identity and Access Management.

#### Quiz 6.

> [!important]
> **Your organization uses Active Directory as its corporate directory. Which managed service in Google Cloud automates best practices to sync your data and manage authentication and directory operations for Active Directory dependent cloud applications?**
>
> * [ ] Identity and Access Management
> * [ ] Cloud Identity
> * [ ] Google Cloud Directory Sync
> * [ ] Active Directory Federation Services

### Lab - [Working with the Google Cloud Console and Cloud Shell (Azure)](https://www.cloudskillsboost.google/course_templates/520/labs/411049)

In this lab, you will become familiar with the Google Cloud web-based interface including Console, the  GUI (graphical user interface) environment, and Cloud Shell, the CLI (command line interface) environment.

* [ ] [Working with the Google Cloud Console and Cloud Shell (Azure)](../labs/Working-with-the-Google-Cloud-Console-and-Cloud-Shell-(Azure).md)

### Lab - [Exploring IAM (Azure)](https://www.cloudskillsboost.google/course_templates/520/labs/411050)

In this lab you will rehearse several activities associated with Identity and Access Management.

* [ ] [Exploring IAM (Azure)](../labs/Exploring-IAM-(Azure).md)

### Document - [Module 1 Student Guide](https://www.cloudskillsboost.google/course_templates/520/documents/411051)

## Networking in Google Cloud

In this module, you will apply your knowledge of networking in Azure to explore the similarities and differences with networking in Google Cloud. You will learn about Google Virtual Private Cloud (VPC), routing and firewalls in Google Cloud, and the variety of options Google Cloud offers for connecting networks.

### Link - [Networking in Google Cloud](https://www.cloudskillsboost.google/course_templates/520/documents/411052)

* [Networking in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-T-INFRAZR1-I-M2&utm_medium=aRT-clicks&utm_campaign=T-INFRAZR1-I-M2&destination=T-INFRAZR1-I-M2&url=https%3A%2F%2Fstorage.googleapis.com%2Fcloud-training%2FT-INFRAZR1-I%2F1.1%2Fod%2Fen%2Fweb%2FMODULE02%2Fcontent%2Findex.html%23%2F)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/520/quizzes/411053)

#### Quiz 1.

> [!important]
> **What is the key difference and similarity in the scope of Azure VNets and Google VPC networks?**
>
> * [ ] Azure VNets are regional and contain regional subnets; Google Cloud VPCs are global and contain regional subnets.
> * [ ] Azure VNets and Google Cloud VPCs are both regional and contain regional subnets.
> * [ ] Azure VNets are global and contain regional subnets; Google Cloud VPCs are regional and contain regional subnets.
> * [ ] Azure VNets and Google Cloud VPCs are both regional and contain zonal subnets.

#### Quiz 2.

> [!important]
> **Which service in Google Cloud enables you to connect two VPC networks from different organizations?**
>
> * [ ] Direct Peering
> * [ ] Carrier Peering
> * [ ] VPC Peering
> * [ ] Shared VPC

#### Quiz 3.

> [!important]
> **You have an Azure Network Security Group that is set up across a region, and then associated with subnets. You want to replicate this environment in Google Cloud. What technology should you choose?**
>
> * [ ] Google Cloud Armor with prioritized rules
> * [ ] Cloud Load Balancing
> * [ ] Direct Interconnect
> * [ ] Google firewall rules defined at the network level

#### Quiz 4.

> [!important]
> **You have an Azure VM without an external IP address assigned to its network interface. The VM connects to a set of external IP addresses used by Azure APIs and services. You want to configure a similar scenario with a Compute Engine VM. What should you do?**
>
> * [ ] Use Google APIs and services by enabling Private Google Access on the subnet used by the VM's network interface.
> * [ ] Use a VPC network to list regional virtual subnetworks (subnets) in data centers, all connected by a global wide area network.
> * [ ] Use Cloud NAT as a Network Address Translation service to manage and scale the service as required.
> * [ ] Create a custom mode VPC network to have complete control over its subnets and IP address ranges.

#### Quiz 5.

> [!important]
> **What is the purpose of a Cloud Router?**
>
> * [ ] A Cloud Router is a hardware router, provided by Google but hosted in Google Cloud.
> * [ ] A Cloud Router implements dynamic VPN that allows topology to be discovered and shared automatically, which reduces manual static route maintenance.
> * [ ] A Cloud Router enables you to perform round-robin switching over multiple VPNs to combine the bandwidth and get better throughput than offered by the internet.
> * [ ] A Cloud Router connects VPN on one side to Direct Peering on the other, which is faster than VPN alone.

#### Quiz 6.

> [!important]
> **You want to connect to Google Workspace and YouTube, but your organization cannot meet Google's peering requirements. What network connection service should you choose?**
>
> * [ ] Dedicated Interconnect
> * [ ] Direct Peering
> * [ ] Partner Interconnect
> * [ ] Carrier Peering

### Lab - [VPC Networking (Azure)](https://www.cloudskillsboost.google/course_templates/520/labs/411054)

In this lab, you create several VPC networks and VM instances and test connectivity across networks.

* [ ] [VPC Networking (Azure)](../labs/VPC-Networking-(Azure).md)

### Lab - [Implement Private Google Access and Cloud NAT (Azure)](https://www.cloudskillsboost.google/course_templates/520/labs/411055)

In this lab, you configure Private Google Access and Cloud NAT for a VM instance that doesn't have an external IP address. Then, you verify access to public IP addresses of Google APIs and services and other connections to the internet.

* [ ] [Implement Private Google Access and Cloud NAT (Azure)](../labs/Implement-Private-Google-Access-and-Cloud-NAT-(Azure).md)

### Document - [Module 2 Student Guide](https://www.cloudskillsboost.google/course_templates/520/documents/411056)

### Document - [What next?](https://www.cloudskillsboost.google/course_templates/520/documents/411057)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
