---
id: 882
name: 'Gemini for DevOps Engineers'
type: Course
url: https://www.cloudskillsboost.google/course_templates/882
date_published: 2024-05-14
topics:
  - Large Language Models
  - Continuous Integration
---

# [Gemini for DevOps Engineers](https://www.cloudskillsboost.google/course_templates/882)

**Description:**

In this course, you learn how Gemini, a generative AI-powered collaborator from Google Cloud, helps engineers manage infrastructure. You learn how to prompt Gemini to find and understand application logs, create a GKE cluster, and investigate how to create a build environment. Using a hands-on lab, you experience how Gemini improves the DevOps workflow.

Duet AI was renamed to Gemini, our next-generation model.

**Objectives:**

* Use Gemini to find and explain log entries.
* Plan and implement a build system with assistance from Gemini.

## Gemini for DevOps Engineers

Learn how to manage infrastructure with help from Gemini.

### Video - [Introducing Gemini for DevOps engineers](https://www.cloudskillsboost.google/course_templates/882/video/476336)

* [YouTube: Introducing Gemini for DevOps engineers](https://www.youtube.com/watch?v=aEkcG5CDFTY)

This is a DevOps engineer. Let's learn how Gemini can be used to find and explain log entries. Later, you'll plan and implement a build system with Gemini's assistance. This DevOps engineer needs to find out why their application is throwing errors in production. They have some alerts coming in and want to use Gemini for Google Cloud to help them find the root cause and resolve it. Let's observe this DevOps engineer as they use Gemini to find what's gone wrong and fix it. It all starts with some helpful emails alerting our engineer to an issue with one of their Cloud projects. While useful as alerts, these notifications are not always precise or informative. Some more investigation will be needed. Something is clearly wrong, and today we unravel this mystery faster with the help of AI. They go into the monitoring console to find more details on the incident. Yes, some errors appear. An intermittent spike. But why? To find out the true scope, they will investigate the logs with a Prometheus query. But feeling rusty, they ask Gemini to help. Using a natural language explanation, they can get a query that gives a summary of all services impacted by this error. Awesome. Now they can identify what services are having problems due to this error spike. Next, why is it happening? In the logs explorer, they detect an illegal buffer error, but then it's full of references to code and multiple files. Instead of digging manually, let's use Gemini again. Explain this log entry, gives a new side panel with a handy summary and a conversation opportunity. Of course, they want to fix the problem ASAP. It's time for them to ask Gemini and Plain English for help. Gemini gives context definitions and follow up links and designs a playbook for how to resolve this illegal buffer issue and get the services into a happy state once more. Our engineer has saved hours of investigation in digging thanks to Gemini so they can fix these errors faster. Now they have more time to pursue their true passion, juggling. What will you build?

### Lab - [Implement continuous delivery with Gemini](https://www.cloudskillsboost.google/course_templates/882/labs/476337)

In this lab, you'll use Gemini to implement continuous delivery for an app in Cloud Run.

* [ ] [Implement continuous delivery with Gemini](../labs/Implement-continuous-delivery-with-Gemini.md)

### Video - [Microservices made easy with Gemini](https://www.cloudskillsboost.google/course_templates/882/video/476338)

* [YouTube: Microservices made easy with Gemini](https://www.youtube.com/watch?v=YJAF0M0zfVY)

I'm a DevOps engineer, or at least a developer responsible for making sure containerized workloads are chugging along smoothly, and I want to make sure my micro services are ready to go on top of Google Kubernete's engine. Let's see how Gemini can help. To get a good understanding of the services I'm managing, I want to look at the logs and find out what's going on. I can ask Gemini from inside Google Cloud Console, and with enough context, it gives me back an answer I can copy and paste into cloud logging. Once I've gotten some of the logs results from that search query, I'd like to better understand them. In addition to the chat in the sidebar, Gemini can explain queries to help me see what these results include, and give me better insight into my workloads. To make sure the new test deployment I'm building out stays out of view of the public. I'd like to create a private build environment. Nobody on the Internet should be able to see the half baked stuff I'm testing with, or we might get some bad publicity. Gemini is here to help once more. In addition to documentation about private pools with Cloud Build, it can give me the G Cloud CLI commands I need to create them, and away we go. Not so fast. I need a config file to specify some of those identifiers and parameters. Gemini is ready to help here again, so I'll just make my own file using the guidance I received and double check. Can I skip some of those options because they are default values? Yes, I can. Once that file is done, I'm ready to try the G Cloud CLI literally started to happen, like, over the course of a couple of weekend CLI command once more, using the configuration I just set up. I have a build pool, but what about the packages I want in my private pool? A quick query shows me that I can use Artifact Registry to host my packages, and with a private repo, I'm ready to go. Just follow Gemini with Google Cloud guidance, and I'm set. Almost. Do I need to fill in the KMS key parameter? Nope. Easy Peezy, lemon squeezy. I'll run that command, create the repo, and my workers are ready. This is great. I got help from Gemini on GKE setup, logs analysis, private test deployments, and private package hosting.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/882/quizzes/476339)

### Document - [Next Steps](https://www.cloudskillsboost.google/course_templates/882/documents/476340)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
