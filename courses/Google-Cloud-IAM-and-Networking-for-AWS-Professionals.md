---
id: 522
name: 'Google Cloud IAM and Networking for AWS Professionals'
datePublished: 2023-09-20
topics:
- Load Balancing
- IAM
- Networking
type: Course
url: https://www.cloudskillsboost.google/course_templates/522
---

# [Google Cloud IAM and Networking for AWS Professionals](https://www.cloudskillsboost.google/course_templates/522)

**Description:**

This is the first course of a four-course series for cloud architects and engineers with existing AWS knowledge, and it compares Google Cloud and AWS solutions and guides professionals on their use.

This course focuses on Identity and Access Management (IAM) and networking in Google Cloud. The learners apply the knowledge of access management and networking in AWS to explore the similarities and differences with access management and networking in Google Cloud. Learners get hands-on practice building and managing Google Cloud resources.

**Objectives:**

- Explain how Google Cloud’s resource hierarchy differs from AWS
- Explain best practices for Google Cloud’s resource hierarchy, including organizations, folders, and projects.
- Explain the differences between Google Cloud IAM and AWS IAM
- Configure Google Cloud IAM to implement best practices for access control
- Describe the differences in AWS and Google Cloud service accounts

## Resources and Access Management in Google Cloud

In this module, you draw on your knowledge of AWS to discuss how you can set up your resource hierarchy and configure access in Google Cloud. You learn how resources get organized with projects, how Identity and Access Management (IAM) lets you control access to resources, and how to use service accounts in Google Cloud. You'll also explore various ways to interact with Google Cloud.

### Link - [Resources and Access Management in Google Cloud](https://www.cloudskillsboost.google/course_templates/522/documents/410199)

- [Resources and Access Management in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-MODULE01&utm_medium=aRT-clicks&utm_campaign=MODULE01&destination=MODULE01&url=https://storage.googleapis.com/cloud-training/T-INFRAWS1-I/1.0.1/od/en/web/MODULE01/content/index.html)

### Lab - [Working with the Google Cloud Console and Cloud Shell (AWS)](https://www.cloudskillsboost.google/course_templates/522/labs/410200)

In this lab, you will become familiar with the Google Cloud web-based interface including Console, the  GUI (graphical user interface) environment, and Cloud Shell, the CLI (command line interface) environment.

- [ ] [Working with the Google Cloud Console and Cloud Shell (AWS)](../labs/Working-with-the-Google-Cloud-Console-and-Cloud-Shell-(AWS).md)

### Lab - [Exploring IAM (AWS)](https://www.cloudskillsboost.google/course_templates/522/labs/410201)

In this lab you will rehearse several activities associated with Identity and Access Management.

- [ ] [Exploring IAM (AWS)](../labs/Exploring-IAM-(AWS).md)

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/522/quizzes/410202)

#### Quiz 1.

> [!important]
> **In AWS, you have been using AWS CloudShell for writing and running bash scripts to manage your AWS resources without setting up credentials and installing packages on the multiple local machines you use. You need to reimplement your scripts in Google Cloud. Which similar tool could you use?**
>
> - [ ] PowerShell on Google Cloud
> - [ ] Google Cloud Console
> - [ ] Cloud SDK
> - [ ] Cloud Shell

#### Quiz 2.

> [!important]
> **In AWS, you have an admin user, Tamara, who manages the organization with an attached policy that allows all IAM actions on all resources within the organization. How would you grant similar permissions in Google Cloud?**
>
> - [ ] Attach a policy with all IAM permissions to Tamara's user identity.
> - [ ] Add Tamara to an admin group that is assigned the roles/resourcemanager.organizationAdmin on the organization.
> - [ ] Add Tamara to an admin group that is assigned the roles/owner basic role.
> - [ ] Create a custom role with permissions for all IAM permissions and attach to Tamara's user identity.

#### Quiz 3.

> [!important]
> **Alexander is a Storage Administrator, responsible for managing objects in Cloud Storage. He needs to have the right permissions for every project across the organization. What should you do?**
>
> - [ ] Assign Alexander the roles/editor at the organizational level.
> - [ ] Add Alexander to a group that has the roles/storage.objectAdmin role assigned at the organizational level.
> - [ ] Assign Alexander the roles/viewer on each project and the roles/storage.objectCreator for each bucket.
> - [ ] Assign Alexander the roles/storage.objectCreator on every project.

#### Quiz 4.

> [!important]
> **In your current AWS environment, you have an IAM role and instance profiles set up for use by a web application to access other services and resources. You need to set up the equivalent environment in Google. Which type of identity should you use in Google Cloud?**
>
> - [ ] Google Cloud IAM policy
> - [ ] Google Cloud IAM role
> - [ ] Google Cloud IAM service account
> - [ ] Google Cloud IAM user

#### Quiz 5.

> [!important]
> **The AWS resource hierarchy uses organizational units to organize accounts, which then contain resources. How would you create a similar hierarchy in Google Cloud?**
>
> - [ ] Folders, projects, resources
> - [ ] Projects, folders, resources
> - [ ] Folders, organizational units, resources
> - [ ] Accounts, folders, resources

### Document - [Module 1 Student Guide](https://www.cloudskillsboost.google/course_templates/522/documents/410203)

## Networking in Google Cloud

In this module, you apply your knowledge of networking in AWS to explore the similarities and differences with networking in Google Cloud. You learn about Google Virtual Private Cloud (VPC), routing and firewalls in Google Cloud, and the variety of options Google Cloud offers for connecting networks.

### Link - [Networking in Google Cloud](https://www.cloudskillsboost.google/course_templates/522/documents/410204)

- [Networking in Google Cloud](https://art-analytics.appspot.com/r.html?uaid=G-1FVH5QDXEV&utm_source=aRT-MODULE02&utm_medium=aRT-clicks&utm_campaign=MODULE02&destination=MODULE02&url=https://storage.googleapis.com/cloud-training/T-INFRAWS1-I/1.0/od/en/web/MODULE02/content/index.html)

### Lab - [VPC Networking (AWS)](https://www.cloudskillsboost.google/course_templates/522/labs/410205)

In this lab, you create several VPC networks and VM instances and test connectivity across networks.

- [ ] [VPC Networking (AWS)](../labs/VPC-Networking-(AWS).md)

### Lab - [Implement Private Google Access and Cloud NAT (AWS)](https://www.cloudskillsboost.google/course_templates/522/labs/410206)

In this lab, you configure Private Google Access and Cloud NAT for a VM instance that doesn't have an external IP address. Then, you verify access to public IP addresses of Google APIs and services and other connections to the internet.

- [ ] [Implement Private Google Access and Cloud NAT (AWS)](../labs/Implement-Private-Google-Access-and-Cloud-NAT-(AWS).md)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/522/quizzes/410207)

#### Quiz 1.

> [!important]
> **You have an AWS security group that is set up on a VPC, and then associated with instances. You want to replicate this environment in Google Cloud. What technology should you choose?**
>
> - [ ] Cloud Load Balancing
> - [ ] Direct Interconnect
> - [ ] Google firewall rules defined at the network level
> - [ ] Google Cloud Armor with prioritized rules

#### Quiz 2.

> [!important]
> **You want to connect to Google Workspace and YouTube, but your organization cannot meet Google's peering requirements. What network connection service should you choose?**
>
> - [ ] Dedicated Interconnect
> - [ ] Carrier Peering
> - [ ] Partner Interconnect
> - [ ] Direct Peering

#### Quiz 3.

> [!important]
> **You have an AWS EC2 instance without an external IP address assigned, but that connects to AWS services and APIs through an AWS NAT Gateway. You want to configure a similar scenario with a Compute Engine VM. What should you do?**
>
> - [ ] Create a custom mode VPC network to have complete control over its subnets and IP address ranges.
> - [ ] Use Cloud NAT as a Network Address Translation service to manage and scale the service as required.
> - [ ] Use Google APIs and services by enabling Private Google Access on the subnet used by the VM's network interface.
> - [ ] Use a VPC network to list regional virtual subnetworks (subnets) in data centers, all connected by a global wide area network.

#### Quiz 4.

> [!important]
> **What is the key difference and similarity in the scope of AWS VPCs and Google VPC networks?**
>
> - [ ] AWS VPCs are regional and contain Availability Zone subnets; Google Cloud VPCs are global and contain regional subnets.
> - [ ] AWS VPCs and Google Cloud VPCs are both regional and contain zonal subnets.
> - [ ] AWS VPCs are regional and contain Availability Zone subnets; Google Cloud VPCs are regional and contain regional subnets.
> - [ ] AWS VPCs and Google Cloud VPCs are both regional and contain regional subnets.

#### Quiz 5.

> [!important]
> **What is the purpose of a Cloud Router?**
>
> - [ ] A Cloud Router connects VPN on one side to Direct Peering on the other, which is faster than VPN alone.
> - [ ] A Cloud Router is a hardware router, provided by Google but hosted in Google Cloud.
> - [ ] A Cloud Router enables you to perform round-robin switching over multiple VPNs to combine the bandwidth and get better throughput than offered by the internet.
> - [ ] A Cloud Router implements dynamic VPN that allows topology to be discovered and shared automatically, which reduces manual static route maintenance.

#### Quiz 6.

> [!important]
> **Which service in Google Cloud enables you to connect two VPC networks from different organizations?**
>
> - [ ] Shared VPC
> - [ ] Carrier Peering
> - [ ] VPC Peering
> - [ ] Direct Peering

### Document - [Module 2 Student Guide](https://www.cloudskillsboost.google/course_templates/522/documents/410208)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
