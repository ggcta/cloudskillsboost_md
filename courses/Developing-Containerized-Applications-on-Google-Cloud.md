---
id: 530
name: 'Developing Containerized Applications on Google Cloud'
type: Course
url: https://www.cloudskillsboost.google/course_templates/530
date_published: 2023-03-22
topics:
  - GKE
---

# [Developing Containerized Applications on Google Cloud](https://www.cloudskillsboost.google/course_templates/530)

**Description:**

In this course, you learn about containers and how to build, and package container images.

The content in this course includes best practices for creating and securing containers, and

provides an introduction to Cloud Run and Google Kubernetes Engine for application developers.

**Objectives:**

* Define containers and container images.
* Build and package applications into container images.
* Identify best practices used to create, test, and secure  containers.
* Understand the basics of Cloud Run and Google Kubernetes  Engine.

## Course Introduction

A brief introduction to the course structure, and it's contents.

### Document - [Course Introduction](https://www.cloudskillsboost.google/course_templates/530/documents/370140)

## Introduction to Containers

This module discusses the basics of containers and container images. You'll learn how to build and package applications into container images with Docker and Buildpacks, and learn about some of the continous integration and delivery tools to build container images. The module also reviews some of the best practices to create, test, and secure containers.

### Document - [Containers and container images](https://www.cloudskillsboost.google/course_templates/530/documents/370141)

### Document - [Building container images with Docker](https://www.cloudskillsboost.google/course_templates/530/documents/370142)

### Lab - [Creating and Running Docker Containers](https://www.cloudskillsboost.google/course_templates/530/labs/370143)

In this lab, you create Docker containers and run them locally in Cloud Shell. You also publish a container image to Artifact Registry.

* [ ] [Creating and Running Docker Containers](../labs/Creating-and-Running-Docker-Containers.md)

### Document - [Building container images with Buildpacks](https://www.cloudskillsboost.google/course_templates/530/documents/370144)

### Lab - [Creating a Containerized Application with Buildpacks](https://www.cloudskillsboost.google/course_templates/530/labs/370145)

In this lab, you build a containerized application with the CLI tool pack, and the Google Cloud Buildpacks builder.

* [ ] [Creating a Containerized Application with Buildpacks](../labs/Creating-a-Containerized-Application-with-Buildpacks.md)

### Document - [Continuous integration and delivery tools](https://www.cloudskillsboost.google/course_templates/530/documents/370146)

### Document - [Best Practices](https://www.cloudskillsboost.google/course_templates/530/documents/370147)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/530/quizzes/370148)

#### Quiz 1.

> [!important]
> **A container image is:**
>
> * [ ] A base runtime system that you can use to bootstrap your application.
> * [ ] A script that is used to deploy source code to a container platform.
> * [ ] A manifest that is used to build a virtual machine.
> * [ ] A package with your application and everything that the application needs to run.

#### Quiz 2.

> [!important]
> **Which of the following statements about using Docker are correct? Select three.**
>
> * [ ] You must pre-build your application from source files before using Docker.
> * [ ] A Dockerfile contains a set of instructions that is used to build a container image.
> * [ ] Dockerfiles provide a powerful, and flexible mechanism to create container images.
> * [ ] A multi-stage build is used to create optimized and secure container images.
> * [ ] When building a container image, if you try to use a base image that is not available in the local image repository, the Docker build fails.

#### Quiz 3.

> [!important]
> **Which of the following statements about Buildpacks are correct? Select three.**
>
> * [ ] Buildpacks are distributed and executed in OCI images called builders, where each builder can support a single source code language.
> * [ ] To create a container image with Buildpacks, you must first develop your own builder.
> * [ ] Google Cloud's buildpacks are built into Cloud Run.
> * [ ] When processing a source directory, a builder executes two phases of a buildpack: the detect phase and the build phase.
> * [ ] Buildpacks are a way to turn your application source code into a container image without writing a Dockerfile.

#### Quiz 4.

> [!important]
> **Which of the following statements about Cloud Build are correct? Select two.**
>
> * [ ] You can only run builds manually when using Cloud Build.
> * [ ] With Cloud Build, you can continuously build, test, and deploy your application on Google Cloud.
> * [ ] You cannot use a Dockerfile when building container images with Cloud Build.
> * [ ] In addition to Cloud Source Repositories, Cloud Build integrates with different source code repositories such as GitHub, Bitbucket, and GitLab.

#### Quiz 5.

> [!important]
> **What are three best practices to use when working with containers or container images?**
>
> * [ ] Remove unnecessary files and tools from the container image.
> * [ ] Run your application as the root user in the container.
> * [ ] Launch the container process with the CMD or ENTRYPOINT instruction in your Dockerfile.
> * [ ] Scan your container images for software vulnerabilities.
> * [ ] When building a Docker container image, the instruction to add your source code should be placed as early as possible near the top of the Dockerfile.

### Document - [Module review](https://www.cloudskillsboost.google/course_templates/530/documents/370149)

## Introduction to Cloud Run and Google Kubernetes Engine

This module introduces Cloud Run, it's features, and use cases for developing and running containerized applications. It also provided an introduction to Google Kubernetes Engine.

### Document - [Introduction to Cloud Run](https://www.cloudskillsboost.google/course_templates/530/documents/370150)

### Lab - [Deploying a Containerized Application on Cloud Run](https://www.cloudskillsboost.google/course_templates/530/labs/370151)

In this lab, you create and deploy a containerized application on Cloud Run.

* [ ] [Deploying a Containerized Application on Cloud Run](../labs/Deploying-a-Containerized-Application-on-Cloud-Run.md)

### Document - [Features and use cases of Cloud Run](https://www.cloudskillsboost.google/course_templates/530/documents/370152)

### Document - [Introduction to Google Kubernetes Engine](https://www.cloudskillsboost.google/course_templates/530/documents/370153)

### Document - [Container-Optimized OS](https://www.cloudskillsboost.google/course_templates/530/documents/370154)

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/530/quizzes/370155)

#### Quiz 1.

> [!important]
> **In Kubernetes, a pod is:**
>
> * [ ] A set of nodes that run your application workloads.
> * [ ] Another name for a Deployment.
> * [ ] A group of one or more containers.
> * [ ] A collection of services.

#### Quiz 2.

> [!important]
> **Which two pricing models are supported by Cloud Run?**
>
> * [ ] CPU always allocated
> * [ ] Based on the number of containers deployed
> * [ ] Fixed fee per service
> * [ ] Pay per use

#### Quiz 3.

> [!important]
> **Which of the following statements about Kubernetes and Google Kubernetes Engine are correct? Select three.**
>
> * [ ] A Kubernetes cluster consists of a control plane and machines called nodes.
> * [ ] In Kubernetes, you can create and configure various kinds of resources in the API either imperatively or declaratively.
> * [ ] Google Kubernetes Engine is a fully managed Kubernetes service that runs on Google Cloud.
> * [ ] A cluster running on Google Kubernetes Engine can only contain a single control plane.

#### Quiz 4.

> [!important]
> **Which of the following statements about Cloud Run are correct? Select three.**
>
> * [ ] Cloud Run runs and autoscales containers on-demand.
> * [ ] To receive requests to your service on Cloud Run, you must manually provision an HTTPS endpoint URL.
> * [ ] To deploy your container to Cloud Run, you can use the Google Cloud console, gcloud CLI, YAML configuration file, or Terraform.
> * [ ] You can use Cloud Run to execute scheduled tasks or jobs.
> * [ ] Before deploying a container to Cloud Run, you must first build your container image outside of Cloud Run.

#### Quiz 5.

> [!important]
> **From which of these container registries can Cloud Run pull container images? Select three.**
>
> * [ ] GitHub
> * [ ] Docker Hub
> * [ ] Other public or private registries
> * [ ] Container Registry
> * [ ] Artifact Registry

### Document - [Module review](https://www.cloudskillsboost.google/course_templates/530/documents/370156)

## Course Review

Brief review of what was discussed in the course.

### Document - [Course review](https://www.cloudskillsboost.google/course_templates/530/documents/370157)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
