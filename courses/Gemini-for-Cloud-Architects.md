---
id: 878
name: 'Gemini for Cloud Architects'
type: Course
url: https://www.cloudskillsboost.google/course_templates/878
date_published: 2024-05-10
topics:
  - GKE
---

# [Gemini for Cloud Architects](https://www.cloudskillsboost.google/course_templates/878)

**Description:**

In this course, you learn how Gemini, a generative AI-powered collaborator from Google Cloud, helps administrators provision infrastructure. You learn how to prompt Gemini to explain infrastructure, deploy GKE clusters and update existing infrastructure. Using a hands-on lab, you experience how Gemini improves the GKE deployment workflow.

Duet AI was renamed to Gemini, our next-generation model.

**Objectives:**

* Prompt Gemini to provide commands that you can use to deploy a basic app to a GKE cluster.
* Create, explore, and modify a GKE cluster by using Gemini to explain and generate shell commands.

## Gemini for Cloud Architects

Learn how to provision infrastructure with help from Gemini.

### Video - [Introducing Gemini for cloud architects](https://www.cloudskillsboost.google/course_templates/878/video/475984)

* [YouTube: Introducing Gemini for cloud architects](https://www.youtube.com/watch?v=DKlUYcdpks0)

[MUSIC] This is a cloud architect. Let's learn how to use Gemini to build and deploy web apps in Google Cloud. To do this, we learned to enable Gemini in the Google Cloud console. Create a series of prompts that describe the infrastructure that you want to deploy. Create a series of prompts that helps you select the correct storage option for your infrastructure. Refine our prompts to fine tune the specific settings in our deployment. To do that, the cloud architect asks Gemini for help and looks to pick the right compute option that will be fully managed. After looking at the options suggested, they decide to focus on Cloud Run. But what's the best way to make sure it can scale? Gemini comes to the rescue once more. Being new to Cloud Run, the architect gets more help from Gemini on networking and authentication help. They will also need caching to help with scale, so Gemini can give advice on caching options and manage services like Memorystore. The web app will also need a database layer, and for that there's a few options in cloud. The architect asks for recommendations and settles on Cloud SQL. Finally, it's time to deploy all three tiers. Gemini shares a sample architecture that includes Cloud Run, Memorystore, and Cloud SQL, all working happily together. Delighted with her progress, our cloud architect is ready to test it out, hooray! With all the time they saved getting this architecture spun up, the cloud architect has more time to practice their ballet moves. What will you build? [MUSIC]

### Lab - [Provision Cloud Infrastructure with Gemini](https://www.cloudskillsboost.google/course_templates/878/labs/475985)

In this lab, you will learn how to use Gemini, an AI-powered collaborator in Google Cloud, to navigate and understand different elements of delpoying and maintaining a managed Kubernete cluster in Google Cloud.

* [ ] [Provision Cloud Infrastructure with Gemini](../labs/Provision-Cloud-Infrastructure-with-Gemini.md)

### Video - [Creating GKE clusters with Gemini](https://www.cloudskillsboost.google/course_templates/878/video/475986)

* [YouTube: Creating GKE clusters with Gemini](https://www.youtube.com/watch?v=xirSA_wn1tw)

If someone asks you if you know about Kubernetes, you have no problem saying yes. If they ask you to set up and manage a GKE cluster on Google Cloud, perhaps it's been a while or you are new to Google Cloud. You may not be clear on some of the actions you need to take. Gemini is here to help. Let's start by opening up Gemini from the Google Cloud console toolbar. If you don't see this icon, make sure you've got Gemini activated on your project, and you have the permissions to use it. You could also use Gemini from within your IDE of choice. Let's jump right in and ask how we can run Kubernetes on Google Cloud without having to own management of nodes and the control pane. Here we have Gemini's response. To run Kubernetes on Google Cloud, you can use Google Kubernetes Engine Autopilot mode. You can also use GKE-managed nodes, which are fully managed Kubernetes that are provisioned and maintained by Google. Let's continue our conversation. We'd love to standardize our cluster creation in autopilot using Terraform, so let's ask if we can do that. From the response, we see that we can. We even get a link or three to dive deeper. We could bookmark these for now, as I'd really like to test GKE cluster creation. Gemini chat is an ongoing conversation as long as it stays in this session. We could also reset our chat by clicking the reset icon. For now, we'll continue on. Gemini has recommended GKE in Autopilot mode for running Kubernetes in Google Cloud. However, I'm unfamiliar with how this managed Kubernetes service works, so let's first test GKE in Autopilot mode and have Gemini help us along. We get a response, but there are some placeholder values for cluster name, region, and project ID. Since I'm already in the project and I know the cluster name in region, I'll be more specific with Gemini, so I can just copy and paste the response. Now let's copy this gcloud command into Cloud Shell and get started deploying a sample application. This will take some time. After our cluster has finished provisioning, we can use a test application for further experimentation. Google already has one called hello-app, and we can use Gemini to help us see how it behaves in GKE Autopilot. Let's use Google's test container image to create a deployment called hello-server. After a few moments, Gemini responds and includes the command. Let's run it in Cloud Shell. Now, the web server is created, but in order for anyone to get to it, we'll need to provision a load balancer for it. Let's ask Gemini how to expose this deployment on Port 80 with a load balancer. Look at that. I didn't even tell the deployment name, but it understood from context that I wanted hello-server when I said to expose this deployment. Finally, if we want to see this service in action, we'll need to point our browser to an IP address. Let's ask Gemini to help us find it. We should get a response with a command to run in our terminal. Let's run it, and in a few minutes, we should have an IP address. Plugging the IP address into our browser shows us the hello-server deployment in action. Once again, let's head into chat and ask Gemini how we can configure time periods where GKE Autopilot will not perform maintenance or upgrades. Gemini responds with information on maintenance windows and exclusions. After reading this, you might realize the off hours of 10:00 PM to 2:00 AM are a great time for maintenance to be run, so let's ask how to create a daily maintenance window on our cluster at that time. After a few moments of thinking, voila, Gemini has given us a response. We could input this command in our shell to set this up and feel free, but now you are ready to add Gemini to your infrastructure administration tool belt. You will also use it to aid in deploying and maintaining your Kubernetes clusters on Google Cloud.

### Video - [Architect web apps with Gemini](https://www.cloudskillsboost.google/course_templates/878/video/475987)

* [YouTube: Architect web apps with Gemini](https://www.youtube.com/watch?v=wD_NWnKAPEI)

As a Cloud architect, you might find yourself designing an organization wide golden path for your developers, one in which they can quickly build a web app in Google Cloud. I'll show you a few ways you can use Gemini as your partner to understand the options better. First, we'll open up Gemini using the icon in the Cloud Console toolbar. Here, we'll chat with Gemini as we would another human being in any chat application. You could also use Gemini chat in some popular IDEs like VS Code with our Google Cloud extensions. We'll start telling Gemini that we are designing a multi tier web app on Google Cloud and that we first want information on what to use for the compute tier. It is important to provide as many details as we would provide a subject matter expert. Let's make it clear we are serving traffic over the public Internet and that we would like fully managed services. In just a few moments, Gemini has provided us with quite a bit of information. Let's say that we are creating the fastest path to running smaller web apps in our organization. The description given for Cloud Run seems to meet our requirements. Let's just confirm this by checking which metrics Cloud Run uses for auto scaling. After a moment, Gemini gives us an answer about incoming requests and also provides a link to follow for more information. Since Gemini told us that Cloud Run uses the number of incoming requests for auto scaling. Let's see where those requests might come from by asking how it is exposed to users over the Internet. The response we get back talks about a public load balancer, which is probably fine for our applications. But some apps might need to be available only to users with the correct permissions. Let's ask how easy it is to only allow authenticated users access to an application. Great. It looks like there's an easy way to accomplish that. Gemini also provides a bit of description as to how to accomplish this and what to expect plus, more information is available if we want to read further. Finally, our goal is to make this as simple as possible for our developers. We prefer they didn't need to write any configuration related to infrastructure like Docker files. Also, we've already standardized on Django as our web framework. Let's ask Gemini if we could deploy these types of apps without the need to containerize anything. Again, Gemini responds in the positive and provides even more context to allow us to use it as we need. It looks like Cloud Run is the way we'll go for the compute layer. Now, onto the caching layer, Gemini will use our previous discussion and answer with that discussion in mind. Let's ask how we can introduce a caching layer and ask to prioritize fully managed services for this tier as well. Our response recommends Cloud Memory Store, Cloud CDN and Redis. Cloud Memory store sounds the most reasonable, but a good architect has security concerns. Let's ensure communication between Cloud Run and Cloud memory store is private. Here is the response, and there is a step to take in ensuring private communication, a serverless VPC access connector. I'm glad we asked that question. I'm glad Gemini was able to help us with the caching tier. Apps of any complexity deal with storing and using data. A relational database might be the way you'd like your developers to go. Continuing our conversation with Gemini, let's ask what it recommends and let it know we'd like to continue prioritizing fully managed services. A few moments later, the response lets us know there are a few options for us. But given our previous discussion, tells us about Cloud SQL first. Given our goals and developer expertise with SQL, this seems like a perfect solution. With our three tiers settled upon, how would we go about deploying an app that uses Cloud Run, Cloud Memory Store, and Cloud SQL together. Let's ask Gemini one more time. Of course, Gemini responds with a solution that has already been developed. In a short conversation, we've come up with a multi tiered web app architecture that fits our needs, and we can move forward with testing it to finalize any thoughts we have on using it. Gemini is a great tool to use when you would normally think out loud, but would also like to get answers to those thoughts. As an architect, you are likely to have many questions when deciding on the best solutions, and Gemini can be there for you.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/878/quizzes/475988)

#### Quiz 1.

> [!important]
> **Which of the following is not a resource that Gemini can help you manage in a GKE cluster?**
>
> * [ ] Network policies
> * [ ] Pods
> * [ ] Nodes
> * [ ] Services

### Document - [Next Steps](https://www.cloudskillsboost.google/course_templates/878/documents/475989)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
