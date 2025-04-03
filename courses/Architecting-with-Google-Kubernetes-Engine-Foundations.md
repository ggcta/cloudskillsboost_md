---
id: 32
name: 'Architecting with Google Kubernetes Engine: Foundations'
type: Course
url: https://www.cloudskillsboost.google/course_templates/32
date: 2025-04-03
datePublished: 2024-01-25
topics:
- Deployment
- GKE
---

# [Architecting with Google Kubernetes Engine: Foundations](https://www.cloudskillsboost.google/course_templates/32)

**Description:**

In this course, "Architecting with Google Kubernetes Engine: Foundations," you get a review of the layout and principles of Google Cloud, followed by an introduction to creating and managing software containers and an introduction to the architecture of Kubernetes.

This is the first course of the Architecting with Google Kubernetes Engine series. After completing this course, enroll in the Architecting with Google Kubernetes Engine: Workloads course.

**Objectives:**

- Understand the difference among Google Cloud compute platforms
- Understand the components and architecture of Kubernetes
- Store container images in Container Registry

## Course Introduction for Course 1

In this module, you'll become familiar with the structure and layout of the course.

### Document - [Welcome and Getting Started Guide](https://www.cloudskillsboost.google/course_templates/32/documents/450873)

### Video - [Course Introduction Foundation](https://www.cloudskillsboost.google/course_templates/32/video/450874)

- [YouTube: Course Introduction Foundation](https://www.youtube.com/watch?v=ZhfA9ppyf0Y)

Hi, I'm Brian. Thanks for taking part in the architecting with Google Kubernetes Engine specialization. You're here because you're interested in Kubernetes, a software layer that sits between your applications and your hardware infrastructure. Because it abstracts away your underlying infrastructure, it's easier to consistently run and manage your applications. Google Kubernetes Engine brings you Kubernetes as a managed service on Google Cloud Platform. The specialization as a whole will teach you how to implement solutions using Google Kubernetes Engine, including, building, scheduling, load balancing, and monitoring workloads, as well as providing for discovery of services, managing role-based access control and security, and providing persistent storage to these applications. In this course, architecting with Google Kubernetes Engine foundation, each module aims to build on your ability to architect with GKE and includes hands-on labs for you to experience functionalities firsthand. In the first module, you'll be introduced to a range of Google Cloud platform services and features with a view to helping you choose the right GCP services to create your own Cloud solution. You'll learn about creating a container using Cloud Build and storing a container in Container Registry. You'll also compare and contrast the features of Kubernetes and Google Kubernetes Engine, also referred to as GKE. In addition to conceptualizing the Kubernetes architecture, you will deploy a Kubernetes cluster using GKE, deploy pods to a GKE cluster and view and managed Kubernetes objects.

## Introduction to Google Cloud

This module helps you start off with the right framework of concepts. After a review of fundamentals cloud computing, you will learn about how Google Cloud's resources around the world are organized into regions and zones. You'll also learn how you can organize the resources you use in Google Cloud, so that you can manage them. Finally, you'll meet the tools that let you connect to Google Cloud and allocate, change, and release resources.

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/32/video/450875)

- [YouTube: Introduction](https://www.youtube.com/watch?v=H5hKCNhhIFs)

Hi, I'm Evan. Welcome to introduction to Google Cloud platform. The first module of this course. I'm excited to share with you the stuff that you need to know, to use Google Kubernetes engine. And the other services that make up Google Cloud platform. In this first module, I'll share a simple explanation of what cloud computing is, so that we start off with the right framework of concepts. So here's a quick preview. Cloud computing entails resources being provided to you, as a service. GCP offers several services that let you run general purpose compute workloads on Google's hardware. And we're going to meet them. Google cloud platform as a global footprint. I'll explain how GCP's resources around the world, are organized into regions and zones. You can then use these resources. But of course it's your job to define the policies for what you want to use. GCP offers a hierarchical structure for organizing your use of cloud resources, and we'll meet it in this module. Finally, you'll meet the tools that let you connect to GCP, and allocate change in the listed resources.

### Video - [Cloud Computing and Google Cloud](https://www.cloudskillsboost.google/course_templates/32/video/450876)

- [YouTube: Cloud Computing and Google Cloud](https://www.youtube.com/watch?v=LTO1DbM-fAs)



### Quiz - [Cloud Computing and Google Cloud](https://www.cloudskillsboost.google/course_templates/32/quizzes/450877)

#### Quiz 1.

> [!important]
> **Which statements are true about cloud computing? Mark all that are true (2 correct answers).**
>
> - [ ] Cloud computing providers dedicate particular physical resources to particular customers.
> - [ ] Customers pay for the resources they use or reserve.
> - [ ] Customers who need more resources can get them rapidly
> - [ ] Human intervention is required to stop using cloud resources once reserved, and payment continues until the change is confirmed.

#### Quiz 2.

> [!important]
> **Which of these Google Cloud compute services provides environments for execution of code, in which users don't have to worry about infrastructure management? Choose all that are correct (2 correct answers).**
>
> - [ ] Compute Engine
> - [ ] Google Kubernetes Engine
> - [ ] Cloud Functions
> - [ ] App Engine

### Video - [Resource Management](https://www.cloudskillsboost.google/course_templates/32/video/450878)

- [YouTube: Resource Management](https://www.youtube.com/watch?v=k9HQKihnBVI)



### Quiz - [Resource Management](https://www.cloudskillsboost.google/course_templates/32/quizzes/450879)

#### Quiz 1.

> [!important]
> **What type of resource is a Compute Engine virtual machine?**
>
> - [ ] Multi-regional
> - [ ] Regional
> - [ ] Zonal
> - [ ] Global

#### Quiz 2.

> [!important]
> **Within which of these Google Cloud geographic scopes are network latencies generally less than 1 millisecond? Choose all that are correct (2 correct answers).**
>
> - [ ] Global
> - [ ] Multi-Region
> - [ ] Zone
> - [ ] Region

#### Quiz 3.

> [!important]
> **What is the base-level organizing entity for creating and using Google Cloud resources and services?**
>
> - [ ] Folder
> - [ ] Region
> - [ ] Project
> - [ ] Cluster

### Video - [Billing](https://www.cloudskillsboost.google/course_templates/32/video/450880)

- [YouTube: Billing](https://www.youtube.com/watch?v=RlCOzjhH484)

Billing! It's no fun but a fact of life. Let's learn more about it. Billing in Google Cloud is set up at the project level. When you define a Google Cloud project, you link a billing account to it. This billing account is where you will configure all your billing information, including your payment option. You can link your billing account to one or more projects. Projects that you don't link to any billing account can only use free Google Cloud services. Your billing account can be charged automatically and invoiced every month, or at every threshold limit. You can separate project billings by setting up billing subaccounts. Some Google Cloud customers who resell Google Cloud services use subaccounts for each of their own clients. You're probably thinking, "How can I make sure I don't accidentally run up a big Google Cloud bill?" Google Cloud provides three tools to help: Budgets and alerts, Billing export, and, Reports. You can define budgets at the billing account level or at the project level. To be notified when costs approach your budget limit, you can create an alert. For example, with a budget limit of $20,000 and an alert set at 90%, you'll receive a notification alert when your expenses reach $18,000. You can also set up a webhook to be called in response to an alert. This webhook can control automation based on billing alerts. For example, you could trigger a script to shut down resources when a billing alert occurs. Or you could use this webhook to file a trouble ticket for your team. Cloud Billing export to BigQuery enables you to export detailed Google Cloud billing data (such as usage, cost estimates, and pricing data) automatically throughout the day to a BigQuery dataset that you specify. Then you can access your Cloud Billing data from BigQuery for detailed analysis, or use a tool like Google Data Studio to visualize your data. Note that the exporting of Cloud Billing data to a file is now deprecated and available only to existing customers using this feature. And Reports is a visual tool in the Console that allows you to monitor expenditure based on a project or services. Google Cloud also implements quotas, which limit unforeseen extra billing charges. Quotas are designed to prevent the over-consumption of resources because of an error or a malicious attack. Quotas apply at the level of the Google Cloud project. There are two types of quotas: rate quotas and allocation quotas. Rate quotas reset after a specific time. For example, by default, the GKE service implements a quota of 3,000 calls to its API from each Google Cloud project per min. This doesn't limit the rate of calls to your applications running in GKE, but, rather, calls to the administrative configuration of your GKE clusters themselves. It would be very unusual to make that many calls in such a short period of time. The quota might well catch and stop erroneous behavior. Allocation quotas govern the number of resources you can have in your projects. This count doesn't reset at intervals; instead you need to free up resources to stay within them. For example, by default, each Google Cloud project has a quota allowing it no more than 15 Virtual Private Cloud networks. These quotas are not the same for all projects. Although projects start with the same quotas, you can change some of them by requesting an increase from Google Cloud Support. Some quotas may increase automatically, based on your use of a product. And you can use the Google Cloud console to explicitly lower some of them for your own projects, say, if you want to put a more stringent cap on your consumption. Finally, some quotas are fixed for all Google Cloud customers. Regardless, in addition to their benefits to customers, Google Cloud quotas also protect the community of Google Cloud users by reducing the risk of unforeseen spikes in usage.

### Quiz - [Billing](https://www.cloudskillsboost.google/course_templates/32/quizzes/450881)

#### Quiz 1.

> [!important]
> **At what level in the Google Cloud resource hierarchy is billing set up?**
>
> - [ ] Folder
> - [ ] Individual users
> - [ ] Project
> - [ ] Organization

#### Quiz 2.

> [!important]
> **Which type of quota resets at regular intervals?**
>
> - [ ] Rate quotas
> - [ ] Allocation quotas

### Video - [Interacting with Google Cloud](https://www.cloudskillsboost.google/course_templates/32/video/450882)

- [YouTube: Interacting with Google Cloud](https://www.youtube.com/watch?v=t3yx6rVd774)

This next video looks at how you interact with GCP. You learn about the Google tools and interfaces that allow you to manage and configure your GCP resources. There are four ways to interact with GCP; the Google Cloud Platform Console, the Cloud Shell and Cloud SDK, the Cloud Console Mobile App, and REST-based APIs. Now, we're not going to focus very much on APIs in this specialization. Developers use them to build applications that allocate and manage GCP resources, but our present focus is on letting Kubernetes manage those resources for us. The GCP Console is a web-based graphical user interface from where you manage your GCP resources. It allows you to execute common tasks using simple mouse clicks with no need to remember commands and avoiding typos. It also provides visibility into your GCP project and its resources. Now, you can sign into the GCP Console from a web browser at console.cloud.google.com. All GCP services are accessible through the simple menu button in the top left-hand corner. You can pin frequently used services to this menu. You'll learn how to use the GCP Console during an upcoming lab. Alternatively, you can download and install the Google Cloud SDK onto a computer of your choice. The Cloud SDK contains a set of command-line tools for the Google Cloud Platform. Most notably for us, it contains the 'gcloud' and the 'kubectl' commands, which we will use a lot of in this course. It also contains the 'gsutil' and 'bq' utilities. You can run these tools interactively or in your automated scripts. The Cloud SDK contains client libraries for various programming languages too. But what if it isn't convenient to install the Cloud SDK in the machine that you're working with? Cloud Shell provides command-line access to your cloud resources directly from within your web browser. Using Cloud Shell, you can manage your projects and resources easily without having to install the Cloud SDK or other tools locally. The Cloud SDK, gcloud, and kubectl command-line tools, and other utilities are always available up-to-date and fully authenticated. How does Cloud Shell do that? It's built using a Compute Engine virtual machine instance that you're not billed for. Each GCP user has one. Your Cloud Shell virtual machine is ephemeral, which means it'll be stopped whenever you stop using interactively and it'll be restarted for you every time you re-enter Cloud Shell. You wouldn't want to run a production web server in your Cloud Shell for example. You'll also get five gigabytes of persistent disk storage that is reattached for you every time a new Cloud Shell session is started. It also provides a web preview functionality and built-in authorization process for access to GCP Console projects and resources including your GKE resources. The Cloud Shell code editor is a tool for editing files inside of your Cloud Shell environment in real-time within your web browser. You can also use text editors from within Cloud Shell command prompt. This tool is extremely convenient working with code-first applications or container-based workloads because you can easily edit files without the needed download and upload changes. But is the easy way always the best way? Of course not. Later on, in this specialization, we'll talk about the best management practices for these code files. Here's a screenshot of the GCP consoles, GKE area showing you its web-based interface for administering your GKE resources. The bottom third of the screenshot is your Cloud Shell and operation where you can launch commands to administer those resources as well. Some of those commands are from the Google Cloud SDK and the others will be specific to your workload. Later in this course, we'll learn about the Kubectl command and you can see it being launched from Cloud Shell here. Finally, there's the Cloud Console Mobile App available for iOS and Android. It offers many capabilities like managing virtual machines and viewing their logs, getting up-to-date billing information for your projects, getting billing alerts for projects that are going over budget and setting up customizable graphs, showing key metrics such as CPU usage, network usage, requests per second and any server errors. We'll not use it in this course but it's a resource you might find convenient and of course it's at no additional charge.

### Quiz - [Interacting with Google Cloud](https://www.cloudskillsboost.google/course_templates/32/quizzes/450883)

#### Quiz 1.

> [!important]
> **Which of these ways to interact with  give you access to the gcloud and kubectl commands? Choose all that are correct (2 correct answers).**
>
> - [ ] Cloud Console mobile app
> - [ ] Cloud SDK
> - [ ] Console
> - [ ] Cloud Shell

### Document - [Computing Options](https://www.cloudskillsboost.google/course_templates/32/documents/450884)

### Video - [Lab Intro](https://www.cloudskillsboost.google/course_templates/32/video/450885)

- [YouTube: Lab Intro](https://www.youtube.com/watch?v=HLAEFHPBIhg)

In this lab, you'll access and become familiar with the GCP Console. You also become familiar with the features of Cloud Shell, including the Cloud Shell code editor. You'll create buckets, VMs, and service accounts using the GCP Console and Cloud Shell and execute several other commands using Cloud Shell as well. You have multiple attempts at doing this lab inside of Qwiklabs. Once you're satisfied, comeback and you'll watch the solution video, we'll walk through each of these steps that you just performed.

### Lab - [Accessing the Google Cloud Console and Cloud Shell](https://www.cloudskillsboost.google/course_templates/32/labs/450886)

Architecting with Google Kubernetes Engine: Introduction to Google Cloud

- [ ] [Accessing the Google Cloud Console and Cloud Shell](../labs/Accessing-the-Google-Cloud-Console-and-Cloud-Shell.md)

### Video - [Lab solution](https://www.cloudskillsboost.google/course_templates/32/video/450887)

- [YouTube: Lab solution](https://www.youtube.com/watch?v=hbsQxbeXTAA)

Now, we'll start off in the GCP console. Let's go to the home screen and select our project name. We'll use this later. Now, let's go to the storage browser and create a new bucket. We're going to name this bucket after our GCP project. We'll accept all the defaults. Now, let's create a Virtual Machine Instance. We'll click the Create Instance button, and we're going to change the name of the VM to first-vm. Let's run it in the us-central1-c zone. Let's compare some of the prices of machine types. The micro type is very inexpensive. We'll take almost all the other defaults except, we're going to configure the firewall to allow HTTP traffic through. Now we click Create. It takes a few minutes to create the virtual machine. Once the virtual machine has been created, let's perform a different task. We're going to make a service account. We click create service account and give the account name. When we click Create, we get the opportunity to define a role for the account. We'll give this one the editor role. A key allows actors to authenticate as the service account. It's downloaded to our local computer. We'll upload it later in the lab. Now that the account has been created, it shows up in the list. Next, let's explore Cloud Shell. Cloud Shell gives us an environment where we can use the G-Cloud command and other cloud commands from the G-Cloud SDK. We're already authenticated. Our first task is to define some environment variables for convenience. It's not required, but it helps us avoid error. We're defining my bucket name one to be the same as our GCS bucket that we created earlier which is named after our project. We'll create another name for a bucket by using that name with a dash two appended to it. We'll echo the contents of that environment variable to make sure it works. I'm going to full-screen the Cloud Shell window and upload the JSON credentials file. It's underneath the three-dot menu. Let's check to make sure it worked. There it is, the file's been successfully uploaded. We'll use it later in the lab. Let's use the gsutil command to make a second cloud storage bucket. Gsutil mb does the job. It's created. When we go back to the storage browser, we will see both the new bucket and the old one in the list. The older one first and then the new one. Let's return to Cloud Shell and make a second virtual machine instance, this time using the command line. Again, to save ourselves the risk of error, we're going to use environment variables. We'll define an environment variable to contain our chosen region. Now let's search for the zones in that region. Looks like the us-central1 region has four zones. With this VM, we're going to choose the a zone. We'll use the G-Cloud command to define our preferred zone, and we'll put our preferred name for our virtual machine into another environment variable for tidiness. Here's the G-Cloud command to create a virtual machine from the command line. As always, it takes a moment to complete. Now that it's done, we can see it in the output of the G-Cloud compute instances list command as well as in the GCP Console. In the Compute Engine VM instances list, we see first VM and second VM. There's also VM here that is an artifact of the Quick Labs environment, that you won't see in your own projects. Let's see how to create a service account from the command line. Let's go to the GCP console now, and see our newly created service account in the list. Under IAM & admin, you go to service accounts and scroll down. There it is. Now we're going to use the command line to give the second service account the project viewer role. Done. We can go into the GCP Console and confirm the effective or action. You click on "IAM" and scroll down in the list of members to find the newly created service account. Its last in alphabetical order. We click the pencil icon and that reveals that it has the viewer role. Now let's work with Cloud Shell. This command copies a picture of a cat out of the publicly available Cloud storage bucket into our Cloud Shell folder. Now we're going to copy that file into our first storage bucket. Now we're going to copy it from one storage bucket to another. All of these were done using the gsutil cp command. Now each of our two bucket has a copy of this picture of a cat. Using the gsutil acl command, we're going to configure the first bucket so that it is private to only its owner. We can see the effect of this change by changing who we are authenticated as. The gcloud config list command shows us that presently the account we're authenticated as is gcpstaging57838_studentqwiklabs.net. Let's change that. Now we're going to assume the role of a service account. The first one we created. Notice that we use the credentials file that we previously uploaded. The gcloud config list command confirms the change is effect. Notice the account now is shown as our service account. Now when we try to copy the cat picture into the first storage bucket, we get an access denied exception because it is private to the owner and we are in the service account now instead of the owner. We can copy the image into the second bucket because we didn't change its permissions. Let's change who we're authenticated as back to our GCP account. We will use the gcloud config command just like before. Now let's repeat our attempt to copy the cat picture into the bucket. It succeeds because we own the bucket. Now let's configure that bucket so that its contents are public. Now when we look at the bucket using the storage browser of the GCP console, we'll notice something new. We'll drill into that bucket and there we will see that there's a public link for the cat picture. We'll open in new tab and we see a picture of a cat. We will use this in a web page. Remember, we configured a virtual machine earlier and opened its firewall port for HTTP. We'll create the web page using the Cloud Shell code editor which you can launch by clicking the pencil icon. Let's explore the Cloud Shell editor first. First, let's experiment with what happens when we change the contents of our Cloud Shell home directory. We're going to clone a Git repository. Notice that the change is immediately reflected in the file display. When I create a directory from the command line, that change is reflected immediately too. Let's open up one of these directories and open a file. Here's the file, cleanup.sh. I'm going to add a new line at the very end of this file. The change is immediately visible from the command line. I'm going to cap the file and there's the line I added. Now let's go make that HTML page. I'm going to return to the home directory and my HL prompt and I'm going to go to the File menu of the editor and create a file called index.html. I'm going to paste in some web page text and I'm going to replace the URL with the actual URL of the copy of the cat picture that I put into my public Cloud storage bucket. Now I'm going to copy that file out of Cloud Shell into my virtual machine. We need to install web server software into our virtual machine. So we're going to SSH to it using the link that's provided for us in the VM instances display. We'll use the standard Debian Linux commands to install the Nginx web server. Now that that's done let's return to Cloud Shell and move our HTML file in using SCP. I know why that didn't work. I put the file into the wrong directory. I'm going to use Cloud Shell's editor to drag it into the right place, into my home directory. Now the command will work. The file is copied to my virtual machine. To return to my SSH window on the VM and move that HTML file from the home directory to Nginx's document root. Now I can go to the VM Instances screen and click the link and I get the web page that I created.

### Video - [Summary](https://www.cloudskillsboost.google/course_templates/32/video/450888)

- [YouTube: Summary](https://www.youtube.com/watch?v=cCwkE65YDz0)

That concludes the Introduction to Google Cloud Platform module. Let me remind you of what you've learned. Cloud computing is a way to organize your use of IT, in which a provider gives you on-demand access over the network to resources from a pool that they maintain. You pay for what you use or reserve. The provider maintains the infrastructure for you, and you can turn it off when you're done. Google Cloud Platform offers lots of different kinds of cloud computing resources, including four that run your code for you on Google hardware. In this course. We're focusing on Kubernetes Engine. All the resources offered by GCP are organized into regions and zones. You can use resources in several zones in a region to increase your application's resiliency. GCP is a shared security model. You're responsible for defining security policies for your GCP resources, and the cloud resource management hierarchy helps you do that in a manageable way. Two important tools that you can use to manage your use of GCP resources are the GCP Console and Cloud Shell. We'll be using both of those throughout the rest of this specialization

### Quiz - [Introduction to Google Cloud](https://www.cloudskillsboost.google/course_templates/32/quizzes/450889)

#### Quiz 1.

> [!important]
> **You need to write some automated scripts to run periodic updates to the resources in your Google Cloud environment. What tools can you install in your own computers to allow you to run those scripts?**
>
> - [ ] The Cloud SDK
> - [ ] The Cloud Console Mobile app
> - [ ] The Cloud Shell
> - [ ] The Google Cloud Console

#### Quiz 2.

> [!important]
> **You are developing a new product for a customer and need to implement control structures in Google Cloud to help manage the Google Cloud resources consumed by the product and the billing for the customer account. What steps should you take to manage costs for this product and customer?**
>
> - [ ] Configure quotas and limits for the product folders.
> - [ ] Configure the billing account at the product folder level in the resource hierarchy.
> - [ ] Set up budgets and alerts at the project level for the product.
> - [ ] Configure the billing account for each project associated with the product.

#### Quiz 3.

> [!important]
> **You are considering deploying a solution using containers on Google Cloud. What Google Cloud solutions are available to you that will provide a managed compute platform with native support for containers?**
>
> - [ ] Compute Engine Autoscaling Groups
> - [ ] Cloud Functions
> - [ ] Container Registry
> - [ ] Google Kubernetes Engine Clusters

#### Quiz 4.

> [!important]
> **One of the key characteristics of cloud computing is the concept of measured service. What is the primary customer benefit of the measured service aspect of cloud computing?**
>
> - [ ] You can get more resources as quickly as you need them.
> - [ ] You share resources from a large pool enabling economies of scale.
> - [ ] Resources can be allocated automatically.
> - [ ] You pay only for the resources you consume.

#### Quiz 5.

> [!important]
> **You are ready to start work building an application in Google Cloud. What IAM hierarchy should you implement for this project?**
>
> - [ ] Create a new folder inside your organization and create projects inside that folder for the resources.
> - [ ] Create new projects and resources inside departmental folders for the resources needed by the component applications.
> - [ ] Create new projects for each of the component applications and create folders inside those for the resources.
> - [ ] Create a new organization for the project and create all projects and resources inside the new organization.

## Introduction to Containers and Kubernetes

In this module you will learn about software containers and their benefits are for application deployment. You'll configure and build containers. You'll also learn about the functions container that management solutions like Kubernetes provide. You'll encounter the advantages of Google Kubernetes Engine compared to building your own container-management infrastructure.

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/32/video/450890)

- [YouTube: Introduction](https://www.youtube.com/watch?v=o9zZmlWy3Ng)

Welcome to the introduction to containers and kubernetes module. In this module, you'll learn what containers are, what their benefits are for application deployment, how containers are configured in built, what functions container management solutions like kubernetes provide, and what the advantage of Google kubernetes engine are, compared to building your own container management infrastructure. In this module, you'll learn how to create a container using Cloud Build and store the container and get in a container registry, and then compare and contrast kubernetes using Google kubernetes engine features.

### Video - [Introduction to Containers](https://www.cloudskillsboost.google/course_templates/32/video/450891)

- [YouTube: Introduction to Containers](https://www.youtube.com/watch?v=7ZXkUZKGb2M)

Let's start by introducing containers. In this video, you'll learn about the key features of containers and the advantages of using containers for application deployment compared to alternatives such as deploying apps directly to virtual machines. You'll learn about Google's Cloud Build, and then you can see how you can use it to build and manage your application images. It's now not very long ago, the default way to deploy an application was on its own physical computer. To set one up, you'd find some physical space, power, cooling, network connectivity for it, and then install an operating system, any software dependencies, and then finally the application itself. If you need more processing power, redundancy, security, or scalability, what'd you do? Well you'd have to simply add more computers. It was very common for each computer to have a single-purpose. For example, a database, web server, or content delivery. This practice as you might imagine, wasted resources and it took a lot of time to deploy and maintain and scale. It also wasn't very portable at all. Applications were built for a specific operating system and sometimes even for specific hardware as well. In comes the dawn of virtualization. Virtualization helped by making it possible to run multiple virtual servers and operating systems on the same physical computer. A hypervisor is the software layer that breaks the dependencies of an operating system with its underlying hardware, and allow several virtual machines to share that same hardware. KVM is one well-known hypervisor. Today you can use virtualization to deploy new servers fairly quickly. Now adopting virtualization means that it takes us less time to deploy new solutions, we waste less of the resources on those physical computers that we're using, and we get some improved portability because virtual machines can be imaged and then moved around. However, the application, all of its dependencies and operating system are still bundled together and it's not very easy to move from a VM from one hypervisor product to another. Every time you start up a VM, it's operating system still takes time to boot up. Running multiple applications within a single VM also creates another tricky problem, applications that share dependencies are not isolated from each other, the resource requirements from one application, can starve out other applications of the resources that they need. Also, a dependency upgrade for one application might cause another to simply stop working. You can try to solve this problem with rigorous software engineering policies. For example, you could lock down the dependencies that no application is allowed to make changes, but this leads to new problems because dependencies do need to be upgraded occasionally. You can add integration tests to ensure that applications work. Integration tests are great, but dependency problems can cause new failure modes that are harder to troubleshoot, and it really slows down development if you have to rely on integration tests to simply just perform basic integrity checks of your application environment. Now, the VM-centric way to solve this problem is to run a dedicated virtual machine for each application. Each application maintains its own dependencies, and the kernel is isolated. So one application won't affect the performance of another. One you can get as you can see here, is two complete copies of the kernel that are running. But here too we can run into issues as you're probably thinking. Scale this approach to hundreds of thousands of applications, and you can quickly see the limitation. Just imagine trying to do a simple kernel update. So for large systems, dedicated VMs are redundant and wasteful. VMs are also relatively slow to start up because the entire operating system has to boot. A more efficient way to resolve the dependency problem is to implement abstraction at the level of the application and its dependencies. You don't have to virtualize the entire machine or even the entire operating system, but just the user space. Again, the user space is all the code that resides above the kernel, and includes the applications and their dependencies. This is what it means to create containers. Containers are isolated user spaces for running application code. Containers are lightweight because they don't carry a full operating system, they can be scheduled or packed tightly onto the underlying system, which is very efficient. They can be created and shut down very quickly because you're just starting and stopping the processes that make up the application and not booting up an entire VM and initializing an operating system for each application. Developers appreciate this level of abstraction because they don't want to worry about the rest of the system. Containerization is the next step in the evolution of managing code. You now understand containers as delivery vehicles for application code, they're lightweight, stand-alone, resource efficient, portable execution packages. You develop application code in the usual way, on desktops, laptops, and servers. The container allows you to execute your final code on VMs without worrying about software dependencies like application run times, system tools, system libraries, and other settings. You package your code with all the dependencies it needs, and the engine that executes your container, is responsible for making them available at runtime. Containers appeal to developers because they're an application-centric way to deliver high performance and scalable applications. Containers also allow developers to safely make assumptions about the underlying hardware and software. With a Linux kernel underneath, you no longer have code that works in your laptop but doesn't work in production, the container's the same and runs the same anywhere. You make incremental changes to a container based on a production image, you can deploy it very quickly with a single file copy, this speeds up your development process. Finally, containers make it easier to build applications that use the microservices design pattern. That is, loosely coupled, fine-grained components. This modular design pattern allows the operating system to scale and also upgrade components of an application without affecting the application as a whole.

### Quiz - [Introduction to Containers](https://www.cloudskillsboost.google/course_templates/32/quizzes/450892)

#### Quiz 1.

> [!important]
> **Which of these problems are containers intended to solve? Mark all that are correct (3 correct answers).**
>
> - [ ] Packaging applications in virtual machines can be wasteful.
> - [ ] Large monolithic applications that need to be run in the cloud.
> - [ ] It's difficult to troubleshoot applications when they work on a developer's laptop but fail in production.
> - [ ] Applications need a way to isolate their dependencies from one another.

### Video - [Containers and Container Images](https://www.cloudskillsboost.google/course_templates/32/video/450893)

- [YouTube: Containers and Container Images](https://www.youtube.com/watch?v=i1Q0d-V0ILw)

An application and its dependencies are called an image. A container is simply a running instance of an image. By building software into container images, developers can easily package and ship an application without worrying about the system it will be running on. You need software to build container images and to run them. Docker is one tool that does both. Docker is an open-source technology that allows you to create and run applications in containers, but it doesn't offer a way to orchestrate those containers at scale as Kubernetes does. In this course, we will use Google's Cloud Build to create Docker-formatted container images. Containers are not an intrinsic, primitive feature of Linux. Instead, their power to isolate workloads is derived from the composition of several technologies. One foundation is the Linux process. Each Linux process has its own virtual memory address space, separate from all others, and Linux processes are rapidly created and destroyed. Containers use Linux namespaces to control what an application can see: process ID numbers, directory trees, IP addresses, and more. By the way, Linux namespaces are not the same thing as Kubernetes namespaces, which you will learn about later in this course. Containers use cgroups to control what an application can use: its maximum consumption of CPU time, memory, I/O bandwidth, and other resources. Finally, containers use union file systems to efficiently encapsulate applications and their dependencies into a set of clean, minimal layers. Now let's see how this works. A container image is structured in layers. The tool you use to build the image reads instructions from a file called the "container manifest." In the case of Docker-formatted container images, that's called a Dockerfile. Each instruction in the Dockerfile specifies a layer inside the container image. Each layer is read-only. (When a container runs from this image, it will also have a writable, ephemeral topmost layer.) Let's look at a simple Dockerfile. This Dockerfile will contain four commands, each of which creates a layer. (At the end of this discussion, I'll explain why this Dockerfile is a little oversimplified for modern use.) The FROM statement starts out by creating a base layer, pulled from a public repository. This one happens to be the Ubuntu Linux runtime environment of a specific version. The COPY command adds a new layer, containing some files copied in from your build tool's current directory. The RUN command builds your application using the "make" command and puts the results of the build into a third layer. And finally, the last layer specifies what command to run within the container when it is launched. Each layer is only a set of differences from the layer before it. When you write a Dockerfile, you should organize from the layers likely to change, through to the layers most likely to change. By the way, I promised that I would explain how this Dockerfile example is oversimplified. These days, the best practice is not to build your application in the very same container that you ship and run. After all, your build tools are at best just clutter in a deployed container, and at worst they are an additional attack surface. Today, application packaging relies on a multi-stage build process, in which one container builds the final executable image, and a separate container receives only what is needed to run the application. Fortunately for us, the tools we use support this practice. When you launch a new container from an image, the container runtime adds a new writable layer on top of the underlying layers. This layer is often called the container layer. All changes made to the running container, such as writing new files, modifying existing files, and deleting files, are written to this thin writable container layer. And they're ephemeral: When the container is deleted, the contents of this writable layer are lost forever. The underlying container image remains unchanged. This fact about containers has an implication for your application design: whenever you want to store data permanently, you must do so somewhere other than a running container image. You will learn about several choices in this specialization. Because each container has its own writable container layer, and all changes are stored in this layer, multiple containers can share access to the same underlying image and yet have their own data state. The diagram shows multiple containers sharing the same Ubuntu image. Because each layer is only a set of differences from the layer before it, you get smaller images. For example, your base application image may be 200 MB, but the difference to the next point release might only be 200 KB. When you build a container, instead of copying the whole image, it creates a layer with just the difference. When you run a container, the container runtime pulls down the layers it needs. When you update, you only need to copy the difference. This is much faster than running a new virtual machine. It's very common to use publicly available open-source container images as the base for your own images, or for unmodified use. For example, you've already seen the "ubuntu" container image, which provides a Ubuntu Linux environment inside a container. "Alpine" is a popular Linux environment in a container, noted for being very small. The nginx web server is frequently used in its container packaging. Artifact Registry is the single place to store container images as well as language and OS packages. You can use Artifact Registry with other Google Cloud services namely IAM for access control, KMS for customer managed encryption keys, Cloud Build for CI/CD and scan for container vulnerabilities with Container Analysis. You can also find container images in other public repositories: Docker Hub Registry, GitLab, and others. The open-source docker command is a popular way to build your own container images. It's widely known and widely available. One downside of building containers with the docker command is that you must trust the computer that you do your builds on. Google provides a managed service for building containers that's integrated with IAM. This service is called Cloud Build, and we'll use it in this course. Cloud Build can retrieve the source code for your builds from many code repositories, including Cloud Source Repositories, or git-compatible repositories like GitHub and Bitbucket. To generate a build with Cloud Build, you define a series of steps. For example, you can configure build steps to fetch dependencies, compile source code, run integration tests, or use tools such as Docker, Gradle, and Maven. Each build step in Cloud Build runs in a Docker container. Then Cloud Build can deliver your newly built images to various execution environments: not only GKE, but also App Engine and Cloud Functions.

### Quiz - [Containers and Container Images](https://www.cloudskillsboost.google/course_templates/32/quizzes/450894)

#### Quiz 1.

> [!important]
> **What is significant about the topmost layer in a container? Choose all that are true (2 correct answers).**
>
> - [ ] An application running in a container can only modify the topmost layer.
> - [ ] Reading from or writing to the topmost layer requires special software libraries.
> - [ ] Reading from or writing to the topmost layer requires special privileges.
> - [ ] The topmost layer's contents are ephemeral. When the container is deleted the contents will be lost.

#### Quiz 2.

> [!important]
> **Why do Linux containers use union file systems?**
>
> - [ ] To give a container its own virtual memory address space
> - [ ] To efficiently encapsulate applications and their dependencies into a set of clean, minimal layers
> - [ ] To control an application's ability to see parts of the directory tree and IP addresses
> - [ ] To control an application's maximum consumption of CPU time and memory

### Video - [Lab Intro](https://www.cloudskillsboost.google/course_templates/32/video/450895)

- [YouTube: Lab Intro](https://www.youtube.com/watch?v=Dh7ZcHCife8)

In this lab, you'll build a Docker container image from provided source code and a Dockerfile using Cloud Build. You'll then upload the container to Container Registry. The tasks that you'll perform include: using Cloud Build to build and push containers and then using Container Registry to store and deploy containers. Remember that you have multiple tries to complete the lab, so don't worry if your lab timer runs out. You can always start again. Now, try out the lab and come back and watch the solution walkthrough video where we'll highlight each of the critical points you just practiced.

### Lab - [Working with Cloud Build](https://www.cloudskillsboost.google/course_templates/32/labs/450896)

Architecting with Google Kubernetes Engine: Working with Cloud Build

- [ ] [Working with Cloud Build](../labs/Working-with-Cloud-Build.md)

### Video - [Lab Solution](https://www.cloudskillsboost.google/course_templates/32/video/450897)

- [YouTube: Lab Solution](https://www.youtube.com/watch?v=lBsa4fV3lIg)

Let's start by making sure that the needed APIs are enabled. In the GCP console, we go to APIs & Services. The API usage graphs are empty because this is a new project. We click "Enable APIs & Services", and type in the name of the API we need. First, we need to check Cloud Build. It says API enabled, that's great. Now, let's go back and try the other API we need for this activity, the Container Registry API. It's also enabled. We would have otherwise been shown a button to enable the API. Now let's launch Cloud Shell. We'll use the simple nano text editor to create a short shell script. This will be the useful payload of the container we build. This shell script simply prints a message whenever it is run. You press Command X to exit and save. Now we create a simple Dockerfile. The base layer of our container will be Alpine Linux. We'll place our shell script into the root directory of the container, and it will arrange for it to be run when the container is launched. We press Command X to exit. We'll set the permissions of the container so that it is executable. Now we'll call Cloud Build to build the container image. The build succeeded, so let's go look at it in Google Container Registry. Here's our container; its name is what we called it on the G Cloud Build command line. Now we'll work with two variations on this pattern. Their sources are stored in a Git repository to save your typing. We clone them in using git clone. Here's a YAML file that describes our build. We're going to create an image with the same name as before. Notice that the Dockerfile and the shell script are here just like before. We submit the YAML file to Cloud Build. The build succeeded. Now let's go see how this is reflected in Google Container Registry. We refresh the display. Still an image by the name quickstart-image, but when we click on it, we see that there's an older version and a newer version. Cloud Build History records the process of building this container images. A powerful capability of Cloud Build is its ability to include logic in the build. Let's take a look at a different YAML file. This YAML file runs the just built container image. You could use this capability to run a test suite that's embedded in your container image. In this example, we have a simulated test suite that always fails. We launch the build once again. The test suite fails, so the build fails. The status is reported to the calling shell.

### Video - [Introduction to Kubernetes](https://www.cloudskillsboost.google/course_templates/32/video/450898)

- [YouTube: Introduction to Kubernetes](https://www.youtube.com/watch?v=rr3Lo07gFBw)

Now, let's introduce a popular container management and orchestration solution called Kubernetes. Let's say your organization has really embraced the idea of containers. Because containers are so lean, your coworkers are creating them in numbers far exceeding the counts of virtual machines you used to have, and the applications running in them need to communicate over the network. But you don't have a network fabric that lets containers find each other. You need help. How can you manage your container infrastructure better? Kubernetes is an open source platform that helps you orchestrate and manage your container infrastructure on-premises or in the Cloud. So what is Kubernetes? It's a container-centric management environment. Google originated it and then donated it to the open source community. Now it's a project of the vendor-neutral Cloud Native Computing Foundation. It automates the deployment, scaling, load balancing, logging, monitoring, and other management features of containerized applications. These are the features that are characteristic of a typical platform as service solutions. Kubernetes also facilitates the features of an infrastructure as a service, such as allowing a wide range of user preferences and configuration flexibility. Kubernetes supports declarative configurations. When you administer your infrastructure declaratively, you describe the desired state you want to achieve instead of issuing a series of commands to achieve that desired state. Kubernetes' job is to make the deployed system conform to your desired state and then keep it there in spite of failures. Declarative configuration saves you work. Because the system's desired state is always documented, it also reduces the risk of error. Kubernetes also allows imperative configuration in which you issue commands to change the system state. But administering Kubernetes as scale imperatively, will be a big missed opportunity. One of the primary strengths of Kubernetes is its ability to automatically keep a system in a state that you declare. Experienced Kubernetes administrators use imperative configuration only for quick temporary fixes and as a tool in building a declarative configuration. Now that you know what Kubernetes is, let's talk about some of its features. Kubernetes supports different workload types. It supports stateless applications such as an Nginx or Apache web server, and stateful applications, where user and session data can be stored persistently. It also supports batched jobs and daemon tasks. Kubernetes can automatically scale in and out containerized applications based on resource utilization. You can specify resource request levels and resource limits for your workloads and Kubernetes will obey them. These resource controls let Kubernetes improve overall workload performance within the cluster. Developers extend Kubernetes through a rich ecosystem of plugins and add-ons. For example, there's a lot of creativity going on currently with Kubernetes custom resource definitions, which bring the Kubernetes declarative management model to amazing variety of other things that need to be managed. The primary focus of this specialization though, is architecting with Kubernetes because it's provided as a service by Google Cloud. So extending Kubernetes is not within our scope. Because it's open source, Kubernetes also supports workload portability across on-premises or multiple Cloud service providers such as GCP and others. This allows Kubernetes to be deployed anywhere. You can move Kubernetes workloads freely without a vendor lock-in.

### Quiz - [Introduction to Kubernetes](https://www.cloudskillsboost.google/course_templates/32/quizzes/450899)

#### Quiz 1.

> [!important]
> **When you use Kubernetes, you describe the desired state you want, and Kubernetes's job is to make the deployed system conform to your desired state and to keep it there in spite of failures. What is the name for this management approach?**
>
> - [ ] Containerization
> - [ ] Imperative configuration
> - [ ] Declarative configuration
> - [ ] Virtualization

#### Quiz 2.

> [!important]
> **What is a stateful application?**
>
> - [ ] A web front end
> - [ ] An application that requires user and session data to be stored persistently
> - [ ] An application that is not containerized

### Video - [Introduction to Google Kubernetes Engine](https://www.cloudskillsboost.google/course_templates/32/video/450900)

- [YouTube: Introduction to Google Kubernetes Engine](https://www.youtube.com/watch?v=rxLkv0F80p4)

Google Cloud's managed services offering for Kubernetes is called Google Kubernetes Engine, or GKE. Why do people choose it? What if you have begun using Kubernetes in your environment, but the infrastructure has become a burden to maintain? Is there anything within Google Cloud that can help you? Absolutely yes. Google Cloud offers a managed Kubernetes solution called Google Kubernetes Engine. Google Kubernetes Engine is a managed Kubernetes service on Google infrastructure. GKE helps you to deploy, manage, and scale Kubernetes environments for your containerized applications on Google Cloud. More specifically, GKE is a component of the Google Cloud compute offerings. It makes it easy to bring your Kubernetes workloads into the cloud. GKE is fully managed, which means you don't have to provision the underlying resources. GKE uses a container-optimized operating system to run your workloads. These operating systems are maintained by Google and are optimized to scale quickly with a minimal resource footprint. The container-optimized OS is discussed later in this course. GKE Autopilot is a mode of operation in GKE in which Google manages your cluster configuration, including your nodes, scaling, security, and other preconfigured settings. The virtual machines that host your containers in a GKE cluster are called nodes. If you enable GKE's auto-repair feature, the service will repair unhealthy nodes for you. It'll make periodic health checks on each node of the cluster. If a node is determined to be unhealthy and require repair, GKE will drain the node (in other words, cause its workloads to gracefully exit) and recreate the node. When you use GKE, you start by directing the service to instantiate a Kubernetes system for you. This system is called a cluster. GKE's auto-upgrade feature can be enabled to ensure that your clusters are always automatically upgraded with the latest stable version of Kubernetes. Just as Kubernetes supports scaling workloads, GKE supports scaling the cluster itself. GKE also integrates with Google's Identity and Access Management, which allows you to control access through the use of accounts and role permissions. Google Cloud's operations suite is a system for monitoring and managing services, containers, applications, and infrastructure. GKE integrates with Cloud Monitoring to help you understand your applications' performance. GKE is integrated with Google Virtual Private Clouds and makes use of Google Cloud's networking features. GKE seamlessly integrates with Google's Cloud Build and Artifact Registry. This allows you to automate deployment using private container images that you have securely stored in Artifact Registry. And finally the Google Cloud console provides insights into GKE clusters and their resources and allows you to view, inspect and delete resources in those clusters. You might be aware that open-source Kubernetes contains a dashboard, but it takes a lot of work to set it up securely. But the Google Cloud console is a dashboard for your GKE clusters and workloads that you don't have to manage, and it's more powerful than the Kubernetes dashboard.

### Quiz - [Introduction to Google Kubernetes Engine](https://www.cloudskillsboost.google/course_templates/32/quizzes/450901)

#### Quiz 1.

> [!important]
> **What is the relationship between Kubernetes and Google Kubernetes Engine?**
>
> - [ ] Google Kubernetes Engine is Kubernetes as a managed service.
> - [ ] Google Kubernetes Engine is a closed-source variant of Kubernetes.
> - [ ] Kubernetes and Google Kubernetes Engine are two names for the same thing.

#### Quiz 2.

> [!important]
> **What is the name for the computers in a Kubernetes cluster that can run your workloads?**
>
> - [ ] Container images
> - [ ] Nodes
> - [ ] Control Planes
> - [ ] Containers

#### Quiz 3.

> [!important]
> **Which of the following supports scaling a Kubernetes cluster as a whole?**
>
> - [ ] Google Kubernetes Engine
> - [ ] Kubernetes
> - [ ] Compute Engine

### Video - [Compute Options Detail](https://www.cloudskillsboost.google/course_templates/32/video/450902)

- [YouTube: Compute Options Detail](https://www.youtube.com/watch?v=PQ0xSkZ_f9I)

In this last lesson, you'll learn more about the computing options available. In a previous module, I briefly introduced your choices for running compute workloads in GCP. Now that we know more about how containers work, we can compare these choices in more detail. The services are: Compute Engine, GKE, App Engine, Cloud Run, and Cloud Functions. At the end of this lesson, you'll understand why people choose each. Compute Engine offers virtual machines that run on GCP. You can select predefined VM configurations. You can also create customized configurations to precisely match your performance and cost requirements. Virtual machines need block storage. Compute Engine offers you two main choices: persistent disks and local SSDs. Persistent disks offer network storage that can scale up to 64 terabytes and you can easily take snapshots of these discs for backup and mobility. You can also choose local SSDs, which enable very high input output operations per second. You can place your Compute Engine workloads behind global load balancers that support auto scaling. Compute Engine offers a feature called managed instance groups. With these, you can define resources that are automatically deployed to meet demand. GCP enables fine-grain control of costs of Compute Engine resources by providing per second billing. This granularity helps reduce your costs when deploying compute resources for short periods of time, such as batch processing jobs. Compute Engine offers preemptible virtual machines, which provides significantly cheaper pricing for your workloads that can be interrupted safely. So why do people choose Compute Engine? With Compute Engine, you have complete control over your infrastructure. You can customize operating systems and even run applications that rely on a mix of operating systems. You can easily lift and shift your on premises workloads into GCP without rewriting your applications or making any changes. Compute Engine is the best option when other computing options don't support your applications or requirements. App Engine has a completely different orientation from Compute Engine. App Engine is a fully- managed application platform. Using App Engine means zero server management and zero configuration deployments. So if you're a developer, you can focus on building applications and not really worrying about the deployment part. So you can simply use your code, and App Engine will deploy that required infrastructure for you. App Engine supports popular languages like Java and Node.js, Python, PHP, C#, . NET, Ruby, and Go. You can also run container workloads, Stackdriver monitoring, logging and diagnostics, such as error reporting are also tightly integrated with App Engine. Stackdriver integrates with tools such as Cloud SDK, Cloud Source repositories, IntelliJ, Visual Studio and PowerShow. App Engine also supports version control and traffic splitting. App Engine is a good choice, if you simply want to focus on writing code, you don't want to worry about building the highly reliable and scalable infrastructure that it will run on. You can just focus on building applications instead of deploying and managing the environment. Use cases for App Engine include, websites, mobile apps, gaming backends, and as a way to present a RESTful API to the Internet. What's a RESTful API? In short, it's an application program interface that resembles the way a web browser interacts with a web server. RESTful APIs are easy for developers to work with and extend, and App Engine makes them easy to operate. Finally, the main topic of this course, Google Kubernetes Engine. We learned that Kubernetes is an orchestration system for applications in containers. It automates deployment, scaling, load balancing, logging and monitoring, and other management features. Google Kubernetes Engine extends Kubernetes management on GCP by adding features and integrating with other GCP services automatically. GKE supports cluster scaling, persistent disks, automated updates to the latest version of Kubernetes, and auto repair for unhealthy nodes. It has built-in integration with Cloud Build, Container Registry, Stackdriver Monitoring, and Stackdriver Logging. Existing workloads running with an on-premise clusters can easily be moved onto GCP. There's no vendor lock in. Overall, GKE is very well suited for containerized applications, cloud-native distributed systems, and hybrid applications. Kubernetes and GKE are discussed in-depth throughout this course. Cloud Run is a managed compute platform that enables you to run stateless containers via web requests or Cloud Pub/Sub events. Cloud Run is serverless, it abstracts away all the infrastructure management, so you can focus on developing applications. It's built on Knative, an open source Kubernetes-based platform. It builds, deploys, and manages modern serverless workloads. Cloud Run gives you the choice of running your containers either fully-managed or in your own GKE cluster. Cloud Run enables you to run request or event-driven stateless workloads without having to worry about servers. It abstracts away all the infrastructure management, such as provisioning, configuring, managing those servers, so you can focus on just writing code. It automatically scales up and down from zero depending upon traffic almost instantaneously, so you never have to worry about scale configuration. Cloud Run charges you for only the resources that you use calculated down to the nearest 100 milliseconds. So you'll never have to pay for those over-provisioned resources. With Cloud Run, you can choose to deploy your stateless containers with a consistent developer experience to a fully-managed environment or to your own GKE cluster. This common experience is enabled by Knative, an open API and runtime environment built on top of Kubernetes. And it gives you the freedom to move your workloads across different environments and platforms either fully-managed on GCP, on GKE, or anywhere Knative runs. Cloud Run enables you to deploy stateless containers that listen for requests or events delivered via HTTP requests. With Cloud Run, you can build your applications in any language using whatever frameworks and tools you wish and deploy them in seconds without having to manage and maintain that server infrastructure. Cloud Functions is an event-driven serverless compute service for simple, single-purpose functions that are attached to events. In Cloud Functions, you simply upload your code, written in JavaScript or Python or Go and then GCP will automatically deploy the appropriate computing capacity to run that code. These servers are automatically scaled and are deployed from highly available in a fault-tolerant design. You're only charged for the time that your code runs. For each function, invocation, memory and CPU use is measured in the 100 millisecond increments rounded up to the nearest increment. Cloud Functions also provides a perpetual free tier, so many Cloud Functions use cases could be free of charge. With Cloud Functions, your code is triggered within a few milliseconds based on events. For example, a file is uploaded to Google Cloud Storage, or a message is received from Cloud Pub/Sub. Cloud Functions can also be triggered based on HTTP endpoints that you define and events in the Firebase mobile application backend. What are some of the use cases for Cloud Functions? They're generally used as part of a microservices application architecture. You can also build simple, serverless mobile IoT backends or integrate with third-party services and APIs. Files uploaded into your GCS bucket can be processed in real time. Similarly, the data can be extracted, transformed, and loaded for querying and analysis. GCP customers often use Cloud Functions as part of intelligent applications, such as virtual assistance, video or image analysis, and sentiment analysis. So which compute service should you adopt? A lot depends on where you're coming from. If you're running applications on physical server hardware, it'll be the path of least resistance to move into Compute Engine. What if you're running applications in long-lived virtual machines in which each VM is managed and maintained? In this case, you'll also find moving to Compute Engine is the quickest GCP service for getting your applications to the cloud. What if you don't want to think about operations at all? Well, App Engine and Cloud Functions are good choices. You can learn more about the differences between App Engine and Cloud Functions in the courses under Developing Applications with Google Cloud Platform. I hope that this course so far has helped you understand why software containers are so beneficial. Containerization is the most efficient and portable way to package up an application. The popularity of containerization is growing very fast. In fact, both Compute Engine, and App Engine can launch containers for you. Compute Engine will accept the container image from you and launch a virtual machine instance that contains it. You can use Compute Engine technologies to scale and manage the resulting VM. And App Engine flexible environment will accept a container image from you and then run it with the same No-ops environment that App Engine delivers for code. But what if you want more control over your containerized workloads than what App Engine offers. And denser packing than what Compute Engine offers? That increasingly popular use case is what GKE is designed to address. The Kubernetes paradigm of container orchestration is incredibly powerful, and its vendor neutral. And a broad and vibrant community has developed all around it. Using Kubernetes as a managed service from GCP saves you work and lets you benefit from all the other GCP resources too. You can also choose Cloud Run to run stateless containers on a managed compute platform. And of course, if you're already running Kubernetes in your on premises data centers, moving to GKE is a great choice. Because you'll be able to bring along both your workloads and your management approach.

### Video - [Summary](https://www.cloudskillsboost.google/course_templates/32/video/450903)

- [YouTube: Summary](https://www.youtube.com/watch?v=D_SeKQajFuM)

That concludes introduction to containers and Kubernetes. In this module, you learned how to create a container using cloud build, which will build and manage your application images. In your labs, you create a Docker formatted container images and so you could privately store them in container registry. You also learn how to securely manage your builds with the native integration with cloud IM. You review the four compute solutions offered by Google Cloud platform starting with compute engine for those lift and shift workloads, app engine, GKE, and cloud functions. Then you weighed the benefits of each and looked at some common use cases. Lastly, you learn that GKE supports automatic Kubernetes version updates, automatic repair for unhealthy nodes, and even scaling of the cluster itself for you. All of this allows you to focus your time on dreaming up in writing your next great application. This means less time worrying about infrastructure, managing and maintaining deployment environments, worrying about security or building and sharing your containers, and it allows you to focus on building your next idea for scale. In the next module, you'll learn about the architecture of Kubernetes.

### Quiz - [Containers and Kubernetes in Google Cloud](https://www.cloudskillsboost.google/course_templates/32/quizzes/450904)

#### Quiz 1.

> [!important]
> **Google Compute Engine provides fine-grained control of costs. Which Compute Engine features provide this level of control? (2 correct responses)**
>
> - [ ] Billing budgets and alerts
> - [ ] Managed instance groups
> - [ ] Fully customizable virtual machines
> - [ ] Autoscaling groups
> - [ ] Per-second billing

#### Quiz 2.

> [!important]
> **You are classifying a number of your applications into workload types. Select the stateful applications in this list of applications. Choose all responses that are correct (2 correct responses).**
>
> - [ ] Image recognition application that identifies product defects from images.
> - [ ] A shopping application that saves user shopping cart data between sessions.
> - [ ] A gaming application that keeps track of user state persistently.
> - [ ] Web server front end for your inventory system.

#### Quiz 3.

> [!important]
> **You are choosing a technology for deploying applications, and you want to deliver them in lightweight, standalone, resource-efficient, portable packages. Which choice best meets those goals?**
>
> - [ ] Containers
> - [ ] Executable files
> - [ ] Virtual Machines
> - [ ] Hypervisors

#### Quiz 4.

> [!important]
> **You are deploying a containerized application, and you want maximum control over how containers are configured and deployed. You want to avoid the operational management overhead of managing a full container cluster environment yourself. Which Google Cloud compute solution should you choose?**
>
> - [ ] Google Kubernetes Engine
> - [ ] Compute Engine
> - [ ] App Engine
> - [ ] Cloud Functions

## Kubernetes Architecture

In this module you'll learn the components of a Kubernetes cluster and how they work together. You'll deploy a Kubernetes cluster using Google Kubernetes Engine and deploy Pods to a GKE cluster. You'll also view and manage several very useful kinds of Kubernetes objects.

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/32/video/450905)

- [YouTube: Introduction](https://www.youtube.com/watch?v=cNpGJYXsPBY)

Welcome to the Kubernetes Architecture module of our course. It helps to know the parts of Kubernetes and to understand the philosophy it implements. How does Kubernetes expect you to tell it what to do? What choices do you have for describing your workloads? That's the theme of this module. In this module, you'll learn how to, understand how the Kubernetes architecture is laid out, deploy a Kubernetes cluster using Google Kubernetes Engine, deploy pods to a GKE cluster, and view and managed several very useful kinds of Kubernetes objects.

### Video - [Kubernetes Concepts](https://www.cloudskillsboost.google/course_templates/32/video/450906)

- [YouTube: Kubernetes Concepts](https://www.youtube.com/watch?v=6h8ZNLV6twA)

Hi, I'm Eoin. In this lesson, we'll lay out the fundamental components of the Kubernetes operating philosophy. To understand how Kubernetes works, there are two related concepts you need to understand. The first is a Kubernetes object model. Each thing Kubernetes manages is represented by an object, and you can view and change these objects, attributes, and state. The second is the principle of declarative management. Kubernetes expects you to tell it what you want the state of the objects under its management to be, and it will work to bring that state into being and keep it there. How does it do that? By means of its so-called 'watch loop.' Formally, a Kubernetes object is defined as a persistent entity that represent the state of something running in a cluster, it's desired state and its current state. Various kinds of objects represent containerized applications, the resources that are available to them, and the policies that affect their behavior. Kubernetes objects have two important elements. You give Kubernetes an object spec for each object you want to create. With this spec, you define the desired state of the object by providing the characteristics that you want. The object status is simply the current state of the object provided by the Kubernetes control plane. By the way, we use the term Kubernetes control plane to refer to the various system processes that collaborate to make a Kubernetes cluster work. You'll learn more about these processes later in this module. Each object is of a certain type or 'Kind' as Kubernetes calls them. Pods are the basic building block of the standard Kubernetes module, and they are the smallest deployable Kubernetes object. You may be surprised to hear me say that. Maybe you're expecting me to say the smallest Kubernetes object is the container. Not so. Every running container in a Kubernetes system is a Pod. A Pod embodies the environment where containers live and that environment can accommodate one or more containers. If there is more than one container in a Pod, they are tightly coupled and they share resources including networking and storage. Kubernetes assigns each Pod a unique IP address. Every container within a Pod shares the network namespace including IP address and network ports. Containers within the same Pod can communicate through localhost 127.0.0.1. A Pod can also specify a set of storage volumes to be shared amongst it's containers. By the way, later in this specialization, you'll learn how Pods can share storage with one another and not just a single Pod. Let's consider a simple example, where you want three instances of the nginx web server, each in its own container, running all the time. How is this achieved in Kubernetes? Remember that Kubernetes embodies the principle of declarative management. You declare some objects to represent those nginx containers. What kind of object? Perhaps Pods! Now it is Kubernetes' job to launch those Pods and keep them in existence. But be careful, Pods are not self healing. If we want to keep all our nginx web servers not just in existence but also working together as a team, we might want to ask for them using a more sophisticated kind of object. We'll tell you more about this later in the module. Let's suppose we have given Kubernetes a desired state that consists of three nginx Pods, always kept running. We did this by telling Kubernetes to create and maintain one or more objects that represent them. Kubernetes compares the desired state to its current state. Let's imagine that our declaration of three nginx containers is completely new. The current state does not match the desired state, so Kubernetes, specifically it's control plane, will remedy the situation. Because the number of desired Pods running for the object we declared as three, and zero are presently running, three will be launched. The Kubernetes control plane will continuously monitor the state of the cluster, endlessly comparing reality to what has been declared and remedying state as needed.

### Quiz - [Kubernetes Concepts](https://www.cloudskillsboost.google/course_templates/32/quizzes/450907)

#### Quiz 1.

> [!important]
> **What is the difference between a pod and a container?**
>
> - [ ] A container contains one or more pods.
> - [ ] A pod contains one or more containers.
> - [ ] Pods and containers are two names for the same thing.

### Video - [Kubernetes Control Plane](https://www.cloudskillsboost.google/course_templates/32/video/450908)

- [YouTube: Kubernetes Control Plane](https://www.youtube.com/watch?v=f8-rQMvVNmc)

In the previous lesson, I mentioned the Kubernetes control plane, which is the fleet of cooperating processes that make a Kubernetes cluster work. Even though you'll only work directly on a few of these components, it helps to know about them and the role each plays. I'll build up Kubernetes cluster part by part, explaining each piece is I go. After I'm done, I'll show you how a Kubernetes cluster running in GKE is a lot less work to manage the one you provisions yourself. Okay, here we go. First and foremost, your cluster needs computers. Nowadays, the computers to compose your clusters usually are virtual machines. They always are in GKE, but they could be physical computers too. One computer is called the control plane and the others are simply called nodes. The job of the nodes is to run parts. The job of the control plane is to coordinate the entire cluster. We'll meet its control plane components first. Several critical Kubernetes components run under control plane. The single component that you interact with directly is called a kube-APIserver. This components job is to accept commands that view or change the state of the cluster, including launching pods. In this specialization, you'll use the kubectl command frequently. This command's job is to connect to the kube-APIserver and communicate with us using the Kubernetes API. kube-APIserver also authenticates incoming requests, determines whether they are authorized and valid, and manages admission control. But it's not just a kubectl that talks with kube-APIserver, in fact any query or change towards the cluster state must be addressed to the kube-APIserver. Etcd is the clusters database. Its job is to reliably store the state of the cluster. This includes all of the cluster configuration data and more dynamic information, such as what nodes are part of the cluster, what pods should be running and where they should be running. You'll never interact directly with etcd, instead kube-APIserver interacts with the database on behalf of the rest of the system. Kube-scheduler is responsible for scheduling pods onto nodes. To do that, it evaluates the requirements of each individual pod and selecting which note is most suitable. But it doesn't do the work of actually launching the pods on the notes. Instead, whenever it discovers a pod object that doesn't yet have an assignment to a node, it chooses a node and simply writes the name of that node into the pod object. Another component of the system is responsible, then for launching to the pods and you'll see it very soon. But how does kube-scheduler decide where to run a pod? It knows the state of all of the nodes and it will obey constraints that you define on where a pod may run, based on hardware, software and policy. For example, you might specify a certain pod is only allowed to run on nodes with a certain amount of memory. You can also define affinity specifications, which caused groups of pods to prefer running on the same node or anti-affinity specifications, which ensure the pods do not run on the same node. You'll learn more about some of these tools in later modules. Kube-controller-manager has a broader job. It continuously monitors the state of the cluster through kubeAPIserver. Whenever the current state of the cluster doesn't match the desired state, kube-controller-manager will attempt to make changes to achieve the desired state. It's called the controller manager because many Kubernetes objects are managed by loops of code called controllers. These loops of code handle the process of re-mediation. Controllers will be very useful for you. To be specific, you'll learn to use certain kinds of Kubernetes controllers to manage workloads. For example, remember our problem of keeping three engine X pods always running? We can gather them together into a controller object called a deployment. That not only keeps them running, but also let's us scale them and bring together under the front end. We'll meet deployments later in this module. Other kinds of controllers have system level responsibilities. For example, node comptroller's job is to monitor and respond when a node is offline. Kube-cloud manager manages controllers that interact with the underlying cloud providers. For example, if you manually launched a Kubernetes cluster on Google compute engine, kube-cloud manager would be responsible for bringing in Google cloud features like load balancers and storage volumes when you needed them. Each node runs a small family of control plane components too. For example, each node runs a kubelet. You can think of a kubelet as Kubernetes agent on each node. When the kube-APIserver wants to start a pod on a node, it connects to that nodes kubelet. Kubelet uses the container runtime to start the pod and monitors its life cycle, including readiness and liveliness probes and reports back to kube-APIserver. Do you remember our use of the term container runtime in the previous module? This is the software that knows how to launch a container from a container image. The world of Kubernetes offers several choices for container runtimes. But the Linux distribution that GKE uses for its node launches containers using Containerd, the runtime component of Docker. Kube-proxy's job is to maintain the network connectivity among the pods in the cluster. In open source Kubernetes, it does so using the firewall capabilities of IP tables, which are built into the. Later in the specialization, we will learn how GKE handles pod networking.

### Quiz - [Kubernetes Control Plane](https://www.cloudskillsboost.google/course_templates/32/quizzes/450909)

#### Quiz 1.

> [!important]
> **Which control plane component is the cluster's database?**
>
> - [ ] kube-controller-manager
> - [ ] etcd
> - [ ] kube-scheduler
> - [ ] kube-apiserver

#### Quiz 2.

> [!important]
> **What is the role of the kubelet?**
>
> - [ ] To serve as Kubernetes's agent on each node
> - [ ] To maintain network connectivity among the Pods in a cluster
> - [ ] To interact with underlying cloud providers

#### Quiz 3.

> [!important]
> **Which control plane component is the only one with which clients interact directly?**
>
> - [ ] kube-apiserver
> - [ ] etcd
> - [ ] kube-controller-manager
> - [ ] kube-scheduler

### Video - [Google Kubernetes Engine Concepts](https://www.cloudskillsboost.google/course_templates/32/video/450910)

- [YouTube: Google Kubernetes Engine Concepts](https://www.youtube.com/watch?v=tZXcgXFDDTQ)

Next, we'll introduce concepts specific to Google Kubernetes Engine. That diagram of the Kubernetes control plane had a lot of components, didn't it? Setting up a Kubernetes cluster by hand is a lot of work. Fortunately, there is an open-source command called kubeadm that can automate much of the initial setup of a cluster. But if a node fails or needs maintenance, a human administrator has to respond manually. I suspect you can see why many people like the idea of a managed service for Kubernetes! GKE is available in two modes of operation, Autopilot and Standard mode. Autopilot is a new mode of operation in GKE that manages the entire cluster's infrastructure, including control plane, node-pools and nodes. By managing the entire cluster, Google monitors and manages all operational aspects of the cluster, including the control plane, worker nodes and core Kubernetes system components, ensuring your workloads always as a place to run. Autopilot is a fully managed Kubernetes cluster bringing together the best of GKE advances in scaling, security and Day 2 operations into a Google SRE managed and optimized kubernetes cluster. Standard mode has all of the same functionality as Autopilot but you are responsible for the configuration, management, and optimization of the cluster to your requirements. Google Cloud advises that unless you have a specific reason you need the level of configuration control that standard offers, you should always use Autopilot mode. Here is how our Kubernetes diagram differs for GKE. From the user's perspective, it's a lot simpler. GKE manages all the control plane components for us. It still exposes an IP address to which we send all of our Kubernetes API requests, but GKE takes responsibility for provisioning and managing all the control plane infrastructure behind it. It also abstracts away having a separate control plane. For the nodes configuration and management, it depends on the type of GKE mode that you are using. Google recommends using Autopilot mode. GKE manages the underlying infrastructure such as node configuration, autoscaling, auto-upgrades, baseline security configurations, and baseline networking configuration. If you're using Standard mode, you manage the underlying infrastructure, including configuring the individual nodes. Now let's talk about nodes. In any Kubernetes environment, nodes are created externally by cluster administrators, not by Kubernetes itself. GKE automates this process for you. It launches Compute Engine virtual machine instances and registers them as nodes. You can manage node settings directly from the Google Cloud console. You pay per hour of life of your nodes (not counting the control plane). Because nodes run on Compute Engine, you choose your node machine type when you create your cluster. By default, the node machine type is e2-medium, which provides 2vCPU, and 4 gigabytes of memory. Google Cloud offers a wide variety of Compute Engine options. At the time this course was developed, the generally available maximum was 416 vCPU cores. That's a moderately big virtual machine. You can customize your nodes' number of cores and their memory capacity. You can select a CPU platform. You can choose a baseline minimum CPU platform for the nodes or node pool. This allows you to improve node performance. GKE will never use a platform that is older than the CPU platform you specify, and if it picks a newer platform, the cost will be the same as the specified platform. You can also select multiple node machine types by creating multiple node pools. A node pool is a subset of nodes within a cluster that share a configuration, such as their amount of memory, or their CPU generation. Node pools also provide an easy way to ensure that workloads run on the right hardware within your cluster: you just label them with a desired node pool. By the way, node pools are a GKE feature rather than a Kubernetes feature. You can build an analogous mechanism within open-source Kubernetes, but you would have to maintain it yourself. You can enable automatic node upgrades, automatic node repairs, and cluster autoscaling at this node pool level. Here's a word of caution. Some of each node's CPU and memory are needed to run the GKE and Kubernetes components that let it work as part of your cluster. So, for example, if you allocate nodes with 15 gigabytes of memory, not quite all of that 15 gigabytes will be available for use by Pods. This module has a documentation link that explains how much CPU and memory are reserved. By default, a cluster launches in a single Google Cloud compute zone with three identical nodes, all in one node pool. The number of nodes can be changed during or after the creation of the cluster. Adding more nodes and deploying multiple replicas of an application will improve an application's availability. But only up to a point! What happens if the entire compute zone goes down? You can address this concern by using a GKE regional cluster. Regional clusters have a single API endpoint for the cluster. However, its control planes and nodes are spread across multiple Compute Engine zones within a region. Regional clusters ensure that the availability of the application is maintained across multiple zones in a single region. In addition, the availability of the control plane is also maintained so that both the application and management functionality can withstand the loss of one or more, but not all, zones. By default, a regional cluster is spread across 3 zones, each containing 1 control plane and 3 nodes. These numbers can be increased or decreased. For example, if you have five nodes in Zone 1, you will have exactly the same number of nodes in each of the other zones, for a total of 15 nodes. Once you build a zonal cluster, you can't convert it into a regional cluster, or vice versa. A regional or zonal GKE cluster can also be set up as a private cluster. The entire cluster (that is, the control plane and its nodes) are hidden from the public internet. Cluster control planes can be accessed by Google Cloud products, such as Cloud Logging or Cloud Monitoring, through an internal IP address. They can also be accessed by authorized networks through an external IP address. Authorized networks are basically IP address ranges that are trusted to access the control plane. In addition, nodes can have limited outbound access through Private Google Access, which allows them to communicate with other Google Cloud services. For example, nodes can pull container images from Google Container Registry without needing external IP addresses.

### Quiz - [Google Kubernetes Engine Concepts](https://www.cloudskillsboost.google/course_templates/32/quizzes/450911)

#### Quiz 1.

> [!important]
> **What is the purpose of configuring a regional cluster in GKE?**
>
> - [ ] To ensure that the cluster's workloads are isolated from the public Internet
> - [ ] To allow applications running in the cluster to withstand the loss of a zone

#### Quiz 2.

> [!important]
> **In GKE, how are control planes provisioned?**
>
> - [ ] As abstract parts of the GKE service that are not exposed to Google Cloud customers
> - [ ] As Compute Engine virtual machines

#### Quiz 3.

> [!important]
> **In GKE clusters, how are nodes provisioned?**
>
> - [ ] As abstract parts of the GKE service that are not exposed to Google Cloud customers
> - [ ] As Compute Engine virtual machines

### Video - [Kubernetes Object Management](https://www.cloudskillsboost.google/course_templates/32/video/450912)

- [YouTube: Kubernetes Object Management](https://www.youtube.com/watch?v=sA84ei7vUB8)

Now we'll discuss Kubernetes Object Management. All Kubernetes objects are identified by a unique name and a unique identifier. Let's return once again to our example in which we want three nginx web servers running all the time. Well, the simplest way would be to declare three Pod objects and specify their state: for each, a Pod must be created and an nginx container image must be used. Let's see how we declare this. You define the objects you want Kubernetes to create and maintain with manifest files. These are ordinary text files. You may write them in YAML or JSON format. YAML is more human-readable and less tedious to edit, and we will use it throughout this specialization. This YAML file defines a desired state for a Pod: its name and a specific container image for it to run. Your manifest files have certain required fields. 'apiVersion' describes which Kubernetes Api version is used to create the object. The Kubernetes protocol is versioned so as to help maintain backwards compatibility. 'Kind' defines the object you want, in this case a Pod, and 'metadata' helps identify the object using name, unique ID, and an optional namespace. You can define several related objects in the same YAML file and it is a best practice to do so. One file is often easier to manage than several. Another even more important tip: You should save your YAML files in version-controlled repositories. This practice makes it easier to track and manage changes and to back-out those changes when necessary. It's also a big help when you need to recreate or restore a cluster. Many GCP customers use Cloud Source Repositories for this purpose, because that service lets them control the permissions of those files in the same way as their other GCP resources. When you create a Kubernetes object, you name it with a string. Names must be unique. Only one object of a particular kind can have a particular name at the same time in a Kubernetes namespace. However, if an object is deleted, its name can be reused. Alphanumeric characters, hyphens, and periods are allowed in the names, with a maximum character length of 253. Each object generated throughout the life of a cluster has a unique ID generated by Kubernetes. This means that no two objects will have the same UID throughout the life of a cluster. 'Labels' are key-value pairs with which you tag your objects during or after their creation. Labels help you identify and organize objects and subsets of objects. For example, you could create a label called 'app' and give as its value the application of which this object is a part. In this simple example, a Deployment object is labeled with three different key values: its application, its environment, and which stack it forms a part of. Various contexts offer ways to select Kubernetes resources by their labels. In this specialization, you will spend plenty of time with the kubectl command. Here's an example of using it to show all the Pods that contain a label called 'app' with a value of 'nginx'. Label selectors are very expressive. You can ask for all the resources that have a certain value for a label, all those that don't have a certain value, or even all those that have a value in a set you supply. So one way to bring three nginx web servers into being would be to declare three Pod objects, each with its own section of YAML. Kubernetes' default scheduling algorithm prefers to spread the workload evenly across the nodes available to it. So we'd get a situation like this one. Looks good, doesn't it? Maybe not. Suppose I want 200 more nginx instances. Managing 200 more sections of YAML sounds very inconvenient. Here's another problem. Pods don't heal or repair themselves, and they're not meant to run forever. They are designed to be ephemeral and disposable. For these reasons, there are better ways to manage what you run in Kubernetes than specifying individual Pods. You need a setup like this to maintain an application's high availability along with horizontal scaling. So, how do you tell Kubernetes to maintain the desired state of three nginx containers? We can instead declare a controller object whose job is to manage the state of the Pods. Some examples of these objects: Deployments, StatefulSets, DaemonSets, and Jobs. We'll meet all of these in our specialization. Deployments are a great choice for long-lived software components like web servers, especially when we want to manage them as a group. In our example, when kube-scheduler schedules Pods for a Deployment, it notifies the kube-APIserver. These changes are constantly monitored by controllers, especially by the Deployment controller. The Deployment controller will monitor and maintain three nginx Pods. If one of those Pods fails, the Deployment controller will recognize the difference between the current state and the desired state, and will try to fix it by launching a new Pod. Instead of using multiple YAML manifests or files for each Pod, you used a single Deployment YAML to launch three replicas of the same container. A Deployment insures that a defined set of Pods is running at any given time. Within its object spec, you specify how many replica Pods you want, how Pods should run, which containers should run within these Pods, and which Volumes should be mounted. Based on these templates, controllers maintain the Pod's desired state within a cluster. Deployments can also do a lot more than this, which you will see later in the course. When Kubernetes schedules a Pod, it's important that the containers have enough resources to actually run. If you schedule a large application on a node with limited resources, it is possible for the node to run out of memory or CPU resources and for things to stop working! It's also possible for applications to take up more resources than they should. This could be caused by a team spinning up more replicas than they need, possibly to artificially decrease latency, or to a bad configuration change that causes a program to go out of control and use 100% of the available CPU. Regardless of whether the issue is caused by a bad developer, bad code, or bad luck, what's important is that you are in control. When you specify a Pod, you can optionally specify how much of each resource a container needs. The most common resources to specify are CPU and memory (RAM); however, there are others. Let's take a look at the mechanisms Kubernetes uses to control these resources. So how do you keep everybody's work on your cluster tidy and organized? Kubernetes allows you to abstract a single physical cluster into multiple clusters known as 'namespaces'. Namespaces provide scope for naming resources such as Pods, Deployments, and controllers. As you can see in this example, there are three namespaces in this cluster: Test, Stage, and Prod. Remember that you cannot have duplicate object names in the same namespace. You can create three Pods with the same name, nginx in this case, but only if they don't share the same namespace. If you attempt to create another Pod with the same name 'nginx Pod' in namespace 'test', you won't be allowed. Object names need only be unique within a namespace, not across all namespaces. Namespaces also let you implement resource quotas across the cluster. These quotas define limits for resource consumption within a namespace. They're not the same as your GCP quotas, which we discussed in an earlier module. These quotas apply specifically to the Kubernetes cluster they're defined on. You're not required to use namespaces for your day-to-day management. You can also use labels. Still, namespaces are a valuable tool. Suppose you want to spin up a copy of a deployment as a quick test. Doing so in a new namespace makes it easy and free of name collisions. There are three initial namespaces in a cluster. The first is a default namespace, for objects with no other namespace defined. Your workload resources will use this namespace by default. Then there is the kube-system namespace for objects created by the Kubernetes system itself. We'll see more of the object kinds in this diagram elsewhere in this specialization. When you use the kubectl command, by default, items in the kube-system namespace are excluded, but you can choose to view its contents explicitly. The third namespace is the kube-public namespace for objects that are publicly readable to all users. kube-public is a tool for disseminating information to everything running in a cluster. You're not required to use it, but it can come in handy, especially when everything running in a cluster is related to the same goal and needs information in common. You can apply a resource to a namespace when creating it using a command-line namespace flag. Or, you can specify a namespace in the YAML file for the resource. Whenever possible, apply namespaces at the command line level. This practice makes your YAML files more flexible. For example, some day you might want to create two completely independent instances of one of your deployments, each in its own namespace. This is difficult if you have chosen to embed namespace names in your YAML files.

### Document - [A note about Deployments and ReplicaSets](https://www.cloudskillsboost.google/course_templates/32/documents/450913)

### Quiz - [Kubernetes Object Management](https://www.cloudskillsboost.google/course_templates/32/quizzes/450914)

#### Quiz 1.

> [!important]
> **In a manifest file for a Pod, in which field do you define a container image for the Pod?**
>
> - [ ] metadata
> - [ ] kind
> - [ ] spec
> - [ ] apiVersion

#### Quiz 2.

> [!important]
> **What is the purpose of the Deployment object?**
>
> - [ ] To launch one or more Pods on a time-based schedule.
> - [ ] To ensure that a defined set of Pods is running at any given time.
> - [ ] To launch one or more Pods and ensure that a specified number of them successfully run to completion and exit.

#### Quiz 3.

> [!important]
> **What are Kubernetes namespaces useful for? Choose all that are correct (2 correct answers).**
>
> - [ ] Namespaces let you implement resource quotas across your cluster.
> - [ ] Namespaces allow you to use object names that would otherwise be duplicates of one another.
> - [ ] Namespaces make resources more secure,
> - [ ] Namespaces partition Linux kernel resources.

### Document - [A note about Services](https://www.cloudskillsboost.google/course_templates/32/documents/450915)

### Document - [Controller objects to know about](https://www.cloudskillsboost.google/course_templates/32/documents/450916)

### Quiz - [Kubernetes Controller Objects](https://www.cloudskillsboost.google/course_templates/32/quizzes/450917)

#### Quiz 1.

> [!important]
> **What is the purpose of a Service? Choose all that are true (2 correct answers)**
>
> - [ ] To provide a way to inspect and diagnose code running in a Pod
> - [ ] To allow you to choose how Pods are exposed
> - [ ] To provide a load-balancing network endpoint for Pods
> - [ ] To allow you to put constraints on Pods' resource consumption

#### Quiz 2.

> [!important]
> **If you are deploying applications in your Pods that need persistent storage, which controller type should you use?**
>
> - [ ] DaemonSet
> - [ ] ReplicaSet
> - [ ] Deployment
> - [ ] StatefulSet

### Video - [Lab Intro](https://www.cloudskillsboost.google/course_templates/32/video/450918)

- [YouTube: Lab Intro](https://www.youtube.com/watch?v=9WirU2JVRFU)

In this lab, you'll build and use GKE clusters and deploy a sample pod. The tasks that you'll learn to perform include using the GCP Console to build and manipulate GKE clusters, deploy a pod, and examine the cluster and pods. Now, go ahead and try the quick lab. You have multiple attempts to complete it, so don't worry if you need more time or want to practice more. Afterward, come back here and we'll walk through the lab solution and key learning points together.

### Lab - [Deploying Google Kubernetes Engine](https://www.cloudskillsboost.google/course_templates/32/labs/450919)

Architecting with Google Kubernetes Engine: Creating a GKE Cluster via Google Cloud Console

- [ ] [Deploying Google Kubernetes Engine](../labs/Deploying-Google-Kubernetes-Engine.md)

### Video - [Migrate for Anthos introduction](https://www.cloudskillsboost.google/course_templates/32/video/450920)

- [YouTube: Migrate for Anthos introduction](https://www.youtube.com/watch?v=JeOff4C2MxY)

Hi, I'm Eoin. So you've heard a bit about Kubernetes and it sounds pretty great. But what if you've got existing applications, that are not in containers, or perhaps not even in the cloud? Well, don't worry, because Google Cloud is the solution for this. Migrate for Anthos, is our tool for getting workloads into containerized deployments on Google Cloud. Let's look at what Migrate for Anthos does. Migrate for Anthos, moves your existing applications into a Kubernetes environment. And the best thing about this, is the process is automated. Your workloads can be on premises, or in other cloud providers. I've already mentioned that Migrate for Anthos are automated, but it's also very fast. Most migrations are completed in less than 10 minutes. And, you have the choice of migrating your applications data in one move, or stream it to the cloud until the application is live. That sounds pretty amazing. Let's have a quick overview of what happens in a migration.

### Video - [Migrate for Anthos Architecture](https://www.cloudskillsboost.google/course_templates/32/video/450921)

- [YouTube: Migrate for Anthos Architecture](https://www.youtube.com/watch?v=mTpimfN7Rnc)

First, let's inspect the architecture required for a migration. The first step is to allow Migrate for Compute Engine to create a pipeline for streaming or migrating the data from on premises or another cloud provider into Google Cloud. Migrate for Compute Engine is a tool that allows you to bring your existing applications into VMs on Google Cloud. Migrate for Anthos is then installed on a GKE processing cluster and is composed of many Kubernetes resources. Migrate for Anthos is used to generate deployment artifacts. Some of these artifacts, like your Kubernetes configurations and the dockerfile are used to create the VM wrapping container. This container goes into Cloud Storage. The container images themselves are stored in the Container Registry. After the deployment assets are created, they can be used to deploy your application into a target cluster. You simply apply the generated configuration and it creates all the necessary Kubernetes elements on the target cluster.

### Video - [Migration Path](https://www.cloudskillsboost.google/course_templates/32/video/450922)

- [YouTube: Migration Path](https://www.youtube.com/watch?v=7rZQZeM-jxA)

Now that you've seen the architecture required from migration, let's look at what happens when you migration application using Migrate For Anthos. First you need to create the processing cluster. After that you install the Migrate For Anthos components onto that cluster. Next you need to add a migration source. You can migrate from VMware, AWS, Azure or Google cloud. You will need to create a migration object with the details of the migration that you're performing. This will generate a plan template for you in a YAML file. You may need to alter this configuration file to create the level of customization that you desire. When the plan is ready, you will need to generate the artifacts for the migration. This means generation that container images of your applications on the YAML files required for the deployment. After your migration artifacts have been generated, they need to be tested. Both the container images and the deployments will be tested at this stage. Finally, if the tests are successful, you can use the generative artifacts to deploy your application in to your production clusters.

### Video - [Migrate for Anthos Installation](https://www.cloudskillsboost.google/course_templates/32/video/450923)

- [YouTube: Migrate for Anthos Installation](https://www.youtube.com/watch?v=6CwTrz2W3TQ)

Okay, we've looked at the infrastructure required for using Migrate for Anthos and the basic path that the migration journey would take. Now let's look at a worked example of installing the necessary tools to perform our migration. Let's go through an example and see what happens at each stage. The first thing you need to do is setup the processing cluster. Before you run the command on screen, you need to make sure that you are a GKE admin to set up the cluster, you also must have firewall rules in place to allow communications between Migrate for Anthos and Migrate for Compute Engine. After all that's done, you can create the processing cluster. The example on screen enables a VPC-native cluster. When the processing cluster is up and running, you need to install Migrate for Anthos using the migctl command. This command installs all of the required Kubernetes resources onto the processing cluster for the migration. The migctl source create command specifies the location of the application to migrate. The example on screen is from migrating from Google Compute Engine. If you're migrating from a VMware backend or another loud provider, you need to install some additional packages. Now that the infrastructure elements are set up, the next step is to create a migration plan. The migctl migration create command will create the migration plan. This command will define the migration resources to be created on the cluster. You identif the source VM on what data to exclude from the migration. You can also specify what migration intents you want. You can specify the following intents: image, image and data, data, or PV-based container. The output of this command is a YAML file that can be further customized. After creating a migration plan, you will need to generate the artifacts for the migration. The migctl migration generate- artifacts command on screen will start this process. This process will first copy files and directories representing the VM to a Container Image Registry as images. Migrate for Anthos creates two images, a runnable image for deployment into another cluster, and a non-runnable image layer that can be used to update the container image in the future. Next, Migrate for Anthos will generate configuration YAML files that you can use to deploy the VM to another GKE cluster. These are copied into a Cloud Storage bucket as an intermediate location. You run the migctl migration get-artifacts command to download the YAML configuration files generated in the last step. The YAML configuration defines the resources to deploy, such as, are you creating a deployment or a stateful set? Is the deployment a headless service? Are you using persistent volumes or persistent volume claims? You can edit the YAML file to customize your deployment. Examples of customizations include enabling load balancing, allowing ingress, or defining disk size. Finally, you run the kubectl apply command to deploy the defined specification.

### Video - [Summary](https://www.cloudskillsboost.google/course_templates/32/video/450924)

- [YouTube: Summary](https://www.youtube.com/watch?v=hp17ZVavM4g)

This concludes the Kubernetes Architecture module. In this module, you learned about the Kubernetes operating philosophy. Every item under Kubernetes control is represented by an object. Kubernetes tries to keep the state of its cluster matching the state that you have declared that you want. You learned about the control plane components that make up Kubernetes. You learned to make a kube-APIserver, which is the point of control for your Kubernetes cluster. And you learned about kubelet, which is your cluster's agent in each node. You also learned that a GKE-managed cluster implements the control plane for you behind the scenes, and that you are not charged separately for it. To tell Kubernetes what you want the state of your cluster to be, create manifest files. Typically, you build these files in a YAML format. These files name and describe the objects that you want Kubernetes to keep alive and healthy. They also document the desired state of your cluster, so you should keep these files in a source control system.

### Quiz - [Kubernetes Architecture](https://www.cloudskillsboost.google/course_templates/32/quizzes/450925)

#### Quiz 1.

> [!important]
> **You want to deploy multiple copies of your application, so that you can load balance traffic across them. How should you deploy this application's Pods to the production Namespace in your cluster?**
>
> - [ ] Deploy the Pod manifest multiple times until you have achieved the number of replicas required.
> - [ ] Create separate named Pod manifests for each instance of the application and deploy as many as you need.
> - [ ] Create a Service manifest for the LoadBalancer that specifies the number of replicas you want to run.
> - [ ] Create a Deployment manifest that specifies the number of replicas that you want to run.

#### Quiz 2.

> [!important]
> **When configuring storage for stateful applications, what steps must you take to provide file system storage inside your containers for data from your applications that will not be lost or deleted if your Pods fail or are deleted for any reason?**
>
> - [ ] You must create Volumes using network based storage to provide durable storage remote to the Pods and specify these in the Pods.
> - [ ] You must export the data from your applications to a remote service that preserves your data.
> - [ ] You must create Volumes using local Storage on the Nodes and mount the Volumes inside your containers to provide durable storage.
> - [ ] You must mount NFS Volumes on each container in the Pod that requires durable storage.

#### Quiz 3.

> [!important]
> **You are designing an application, and you want to ensure that the containers are located as close to each other as possible, in order to minimize latency. Which design decision helps meet this requirement?**
>
> - [ ] Place the containers in the same Pod.
> - [ ] Place the containers in the same Namespace.
> - [ ] Give the containers the same labels.
> - [ ] Place the containers in the same cluster.

#### Quiz 4.

> [!important]
> **You have deployed a new Google Kubernetes Engine regional cluster with four machines in the default pool for the first zone and left the number of zones at the default. How many Compute Engine machines are deployed and billed against your account?**
>
> - [ ] Sixteen. (Four nodes are deployed in primary and secondary zones in two regions, for a total of 4 zones and 16 nodes. A control plane node is deployed in each zone but it is not billed to your account.)
> - [ ] Twelve. (Four nodes are deployed in each of three zones. A control plane node is deployed in each zone which is indirectly billed against your account through the cluster management fee.)
> - [ ] Fifteen. (Four nodes and a single control plane are deployed to each of the three zones. A control plane node is deployed in each zone and it is billed against your account.)
> - [ ] Ten. (Four nodes are deployed in the first zone and three nodes are deployed in two other zones because you selected the defaults.)

#### Quiz 5.

> [!important]
> **You need to ensure that the production applications running on your Kubernetes cluster are not impacted by test and staging deployments. Which features should you implement and configure to ensure that the resources for your production applications can be prioritized?**
>
> - [ ] Configure resource requests for Test, Staging and Production and configure specific Kubernetes resource quotas for the Production Namespace.
> - [ ] Configure labels for Test, Staging and Production and configure specific Kubernetes resource quotas for the Production Namespace.
> - [ ] Configure Namespaces for Test, Staging and Production and configure specific Kubernetes resource quotas for the test and staging Namespaces.
> - [ ] Configure Namespaces for Test, Staging and Production and configure specific Kubernetes resource quotas for the Production Namespace.

#### Quiz 6.

> [!important]
> **Which Kubernetes component does the kubectl command connect to in order to carry out operations on a cluster?**
>
> - [ ] kube-scheduler
> - [ ] kube-dns
> - [ ] kube-controller-manager
> - [ ] kube-apiserver

### Document - [Next steps](https://www.cloudskillsboost.google/course_templates/32/documents/450926)

## Course Resources

PDF links to all modules

### Document - [Foundations Course Resources](https://www.cloudskillsboost.google/course_templates/32/documents/450927)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
