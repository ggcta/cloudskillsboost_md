---
id: 660
name: 'Configure Google Kubernetes Engine Networking'
datePublished: 2023-09-14
topics:
- Networking
- GKE
- Ingress
type: Course
url: https://www.cloudskillsboost.google/course_templates/660
---

# [Configure Google Kubernetes Engine Networking](https://www.cloudskillsboost.google/course_templates/660)

**Description:**

This course teaches you some basic Google Kubernetes Engine (GKE) networking. With written lectures, hands-on lab exercises, and quizzes, you learn how to set up services, facilitate communication, and configure secure access to your GKE applications.

**Objectives:**

- Create and use an ingress resource.
- Manage traffic to and between GKE clusters.
- Configure Anthos Service Mesh to communicate with and between GKE resources.
- Configure Cloud NAT to provide external communication to GKE private clusters.

## GKE Networking Overview

In this module, you learn about services in GKE, particularly ingress.

### Document - [Introduction](https://www.cloudskillsboost.google/course_templates/660/documents/405088)

### Document - [Clusters and services](https://www.cloudskillsboost.google/course_templates/660/documents/405089)

### Lab - [Creating Services and Ingress Resources](https://www.cloudskillsboost.google/course_templates/660/labs/405090)

Architecting with Google Kubernetes Engine: Creating Services and Ingress Resources

- [ ] [Creating Services and Ingress Resources](../labs/Creating-Services-and-Ingress-Resources.md)

### Document - [Pod DNS](https://www.cloudskillsboost.google/course_templates/660/documents/405091)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/660/quizzes/405092)

#### Quiz 1.

> [!important]
> **Sasha checked the VPC flow logs and observed that traffic ingresses and egresses through a load balancer. Sasha wants egress traffic to bypass the load balancer. What can they do?**
>
> - [ ] Create an external passthrough Network Load Balancer for use with your Ingress.
> - [ ] Create a new cluster using Dataplane V2, and deploy your applications to the new cluster.
> - [ ] Edit the cluster to use Dataplane V2; the nodes will automatically use the change.
> - [ ] Edit the cluster to use Dataplane V2 and the node pool.

#### Quiz 2.

> [!important]
> **(Choose all that apply) Which statements about GKE standard mode clusters are true?**
>
> - [ ] Google configures the node pool scaling for you.
> - [ ] An Alias IP range is used to assign IP addresses to pods.
> - [ ] Standard mode clusters use Dataplane V2 by default.
> - [ ] Standard mode clusters support more  pods than autopilot mode.

#### Quiz 3.

> [!important]
> **(Choose all that apply) For a cluster in autopilot mode, you can set:**
>
> - [ ] Network tags
> - [ ] The GKE version
> - [ ] The dataplane to use
> - [ ] The service address range
> - [ ] The node subnet

## Anthos Service Mesh

In this module, you learn how to set up and use Anthos Service Mesh.

### Document - [Introduction to Anthos Service Mesh](https://www.cloudskillsboost.google/course_templates/660/documents/405093)

### Lab - [Installing Cloud Service Mesh on Google Kubernetes Engine](https://www.cloudskillsboost.google/course_templates/660/labs/405094)

In this lab you will install the Cloud Service Mesh, and use it with the Bookinfo microservices application, all on a GKE cluster.

- [ ] [Installing Cloud Service Mesh on Google Kubernetes Engine](../labs/Installing-Cloud-Service-Mesh-on-Google-Kubernetes-Engine.md)

### Document - [Lab Review](https://www.cloudskillsboost.google/course_templates/660/documents/405095)

### Document - [Architecture](https://www.cloudskillsboost.google/course_templates/660/documents/405096)

### Document - [Installation](https://www.cloudskillsboost.google/course_templates/660/documents/405097)

### Document - [Life of a request in the mesh](https://www.cloudskillsboost.google/course_templates/660/documents/405098)

### Document - [Mesh telemetry and instrumentation](https://www.cloudskillsboost.google/course_templates/660/documents/405099)

### Document - [Anthos Service Mesh dashboards](https://www.cloudskillsboost.google/course_templates/660/documents/405100)

### Document - [Anthos Service Mesh pricing and support](https://www.cloudskillsboost.google/course_templates/660/documents/405101)

### Lab - [AHYBRID041 Observing Anthos Services](https://www.cloudskillsboost.google/course_templates/660/labs/405102)

Do a custom install of Cloud Service Mesh, evaluate performance with monitoring, logging and tracing, and define and measure SLOs. Optionally, perform similar observability tasks using common OSS tools.

- [ ] [AHYBRID041 Observing Anthos Services](../labs/AHYBRID041-Observing-Anthos-Services.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/660/quizzes/405103)

#### Quiz 1.

> [!important]
> **Which CLI tool is used to install and manage Anthos Service Mesh?**
>
> - [ ] kubectl
> - [ ] asmcli
> - [ ] meshctl
> - [ ] gcloud

#### Quiz 2.

> [!important]
> **Wasm plugins can be used to send telemetry to external backend such as Cloud Monitoring.**
>
> - [ ] True
> - [ ] False

#### Quiz 3.

> [!important]
> **The Anthos Service Mesh control plane interacts with the Envoy proxies to**
>
> - [ ] Check quotas and ACLs as requests flow through the mesh.
> - [ ] Secure requests using mTLS as they flow through the mesh.
> - [ ] Configure them on pod creation.
> - [ ] Route requests as they flow through the mesh.

## Pod Networking

In this module, you learn how to configure pod networking, as well as how to limit traffic to and between the pods.

### Document - [Controlling pod access](https://www.cloudskillsboost.google/course_templates/660/documents/405104)

### Lab - [How to Use a Network Policy on Google Kubernetes Engine](https://www.cloudskillsboost.google/course_templates/660/labs/405105)

In this lab you learn how to improve the security of your Kubernetes Engine by applying fine-grained restrictions to limit intra-cluster network communication.

- [ ] [How to Use a Network Policy on Google Kubernetes Engine](../labs/How-to-Use-a-Network-Policy-on-Google-Kubernetes-Engine.md)

### Document - [Masquerading IP addresses](https://www.cloudskillsboost.google/course_templates/660/documents/405106)

### Document - [Discontiguous multi-pod CIDR](https://www.cloudskillsboost.google/course_templates/660/documents/405107)

### Document - [Configuring Privately Used Public IPs (PUPIs) with GKE](https://www.cloudskillsboost.google/course_templates/660/documents/405108)

### Document - [Cloud NAT and GKE](https://www.cloudskillsboost.google/course_templates/660/documents/405109)

### Lab - [Using a NAT Gateway with Kubernetes Engine](https://www.cloudskillsboost.google/course_templates/660/labs/405110)

This lab shows how to define new node IP address mappings by using network address translation (NAT) gateways.

- [ ] [Using a NAT Gateway with Kubernetes Engine](../labs/Using-a-NAT-Gateway-with-Kubernetes-Engine.md)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/660/quizzes/405111)

#### Quiz 1.

> [!important]
> **Your autopilot mode cluster has run out of IP addresses. What can you do?**
>
> - [ ] Add secondary IP ranges to the cluster.
> - [ ] Add secondary IP ranges to the cluster subnet.
> - [ ] Recreate the cluster and add secondary IP address ranges.
> - [ ] Recreate the cluster with a larger IP address range.

#### Quiz 2.

> [!important]
> **You need to disguise pod addresses in an autopilot mode cluster. What can you do?**
>
> - [ ] Configure a GKE NAT ingress policy.
> - [ ] Configure the masquerade settings on the cluster VPC network.
> - [ ] Configure the masquerade settings on the cluster.
> - [ ] Configure the masquerade settings on the cluster subnet.

#### Quiz 3.

> [!important]
> **(Choose all that apply) To use Cloud NAT with GKE, you**
>
> - [ ] Enables Cloud NAT on the cluster VPC network.
> - [ ] Configure the node pools to use Cloud NAT.
> - [ ] Create a NAT configuration using Cloud Router.
> - [ ] Create firewall policies as needed.
> - [ ] Configure the cluster to use Cloud NAT.

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
