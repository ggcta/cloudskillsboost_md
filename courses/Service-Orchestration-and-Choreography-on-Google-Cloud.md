---
id: 465
name: 'Service Orchestration and Choreography on Google Cloud'
type: Course
url: https://www.cloudskillsboost.google/course_templates/465
date_published: 2024-10-08
topics:
  - Eventarc
  - Workflows
  - Application Integration
---

# [Service Orchestration and Choreography on Google Cloud](https://www.cloudskillsboost.google/course_templates/465)

**Description:**

This course introduces you to event-based applications and teaches you how to use service orchestration and choreography to coordinate microservices. Using lectures and hands-on labs, you learn how to use Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler to build microservices applications on Google Cloud.

**Objectives:**

* Describe the benefits and challenges of microservices-based architectures.
* Describe the advantages of event-driven applications.
* Identify the strengths of orchestration and choreography.
* Use Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler to coordinate a microservices application on Google Cloud.

## Introduction

Welcome to "Service Orchestration and Choreography on Google Cloud." This course introduces you to microservices, event-driven applications, and the use of service choreography and orchestration on Google Cloud. Through a combination of lectures, hands-on labs, and supplemental materials, you will learn about Google Cloud's services that enable application integration and service communication: Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler.

### Video - [Course introduction](https://www.cloudskillsboost.google/course_templates/465/video/511509)

* [YouTube: Course introduction](https://www.youtube.com/watch?v=rKVfsP5mJgA)

Managing the communication between microservices in your application can be a challenging task, especially as your application scales in size and complexity. An event-based architecture and Google Cloud managed services for application integration can help you address the complexity. In the Service Orchestration and Choreography on Google Cloud course, learn how the orchestration and choreography patterns can be used to coordinate service communication, and how four managed services provided by Google Cloud can streamline the process. Hi, my name is Mike and I’m a Technical Curriculum Developer here at Google Cloud. This course introduces you to the orchestration and choreography patterns and the services in Google Cloud used to coordinate microservices: Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler. This content is for application developers, architects, and cloud engineers who want to build applications with microservices. Through a series of video lectures, quizzes, and hands-on labs, you get an introduction to microservices, event-driven applications, and the use of service choreography and orchestration in Google Cloud. You learn how to describe the benefits and challenges of microservices-based architectures, And the advantages of event-driven applications. In addition, you learn to identify the strengths of orchestration and choreography. And use Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler to coordinate a microservices application on Google Cloud. Let's get started!

## Introduction to Microservices

This module introduces you to microservices and discusses the benefits and challenges of using a microservices architecture for your applications.

### Video - [Module overview](https://www.cloudskillsboost.google/course_templates/465/video/511510)

* [YouTube: Module overview](https://www.youtube.com/watch?v=Ukdc-6BkE6o)

Welcome to module 1 of Service Orchestration and Choreography on Google Cloud: Introduction to Microservices. In this module, you learn about microservices, an architectural style for developing applications. We discuss the benefits you gain by developing your applications using microservices. We also discuss some challenges that a microservices architecture can introduce.

### Video - [What are microservices?](https://www.cloudskillsboost.google/course_templates/465/video/511511)

* [YouTube: What are microservices?](https://www.youtube.com/watch?v=GvA597Fdlws)

Today, many new enterprise applications are being designed using a microservices architecture. What are microservices? First, we should understand how applications were traditionally designed. Early enterprise applications were developed as large, self-contained applications. These applications included the user interface, business logic, and data access code, with data persisted in a large, relational database. These applications were designed to handle many tasks, and the codebase was necessarily complex. Each major change to the application tended to make the codebase even more complex. And, because the code was all in a single application, the application code was often tightly coupled. This interdependent code was hard to maintain, making it difficult to fix bugs without introducing new ones. We now call these monolithic applications, or monoliths. Service-Oriented Architecture, or SOA, was an attempt to solve the challenges of monolithic applications. SOA is an architectural style that focuses on building reusable software components called services. Each service in a service-oriented architecture should execute a discrete business function, ...and communication between services was implemented using messaging over defined service interfaces. SOA was typically implemented at an enterprise level. Organizations would map business activities into services, and mandate interoperability and discoverability standards for their services. SOA did provide tangible benefits, but it typically produced mixed results. One clear benefit was that services were smaller and more loosely coupled than in large monolithic applications. Smaller services often led to smaller development teams focused on a single service and a smaller problem domain, which could improve efficiency. Service reuse was also a large focus of SOA. Applications were created by combining services. The messages between services were handled by a messaging middleware component called the Enterprise Service Bus, or ESB. By managing connectivity, security, and message routing and transformation, the ESB enabled applications to be integrated, even for applications outside the organization. Applications would connect to the ESB, and the ESB would transform protocols, route messages between services, and transform data. Though SOA reduced complexity in the service code, the complexity was typically shifted to ESB integrations. ESB integrations became the bottleneck in successfully launching and updating applications. The ESB was typically managed by a central team, and ESB integration work could face significant delays because all application and service teams needed ESB work. Changing an integration for one application might destabilize other applications using the integration. Even updates to the ESB software itself could break existing integrations, so ESB updates required significant testing. Microservices are an alternative, decentralized approach to decomposing applications into services. Microservices are separate services, limited in scope. In this example, each of the business domains (orders, products, and reviews) is in its own microservice with its own database. A microservice specifies an interface, typically an API, that is used by other services when calling the operations of the microservice. The separation of microservices tends to lead to loose coupling between the microservices. Loosely coupled services are easier to maintain, update, and deploy. When you're starting to design a new application, you may decide to start with microservices instead of a monolith. One of the most difficult parts of architecting a new microservices application is designing the service boundaries. If you're designing an application and do not have expertise in the problem domain, choosing the separate services to create might be difficult. If you start with a monolithic application, you can build your application before you fully understand how to separate the services. You can migrate to a microservices architecture later as you gain more experience with the problem domain. It's easier to deliver microservices in an agile fashion than it is to deliver monoliths. If you require the ability to quickly release changes to your services, it probably makes sense to start with microservices. If you plan to grow the size of your team, microservices allow new team members to focus on smaller parts of the overall application. Team members aren't required to learn a large monolithic codebase. A microservices application provides natural service boundaries that allow for smaller teams, with each team having reduced scope. When starting with a monolith, design your application to be modular so it's easier to migrate to microservices in the future.

### Video - [Benefits of microservices architectures](https://www.cloudskillsboost.google/course_templates/465/video/511512)

* [YouTube: Benefits of microservices architectures](https://www.youtube.com/watch?v=wpJ4DI44QQE)

Developing your applications as microservices has many benefits. One obvious benefit of microservices is that each microservice is simpler than the large, monolithic application. Each microservice has a smaller and simpler codebase, which generally allows for a single, small team to focus on the internal details of that microservice. It's easier for the members of that team to understand the microservice and update it without causing issues in other parts of the application. Microservices are typically easier to unit test, because there are clear boundaries between different services. Microservices are also separately deployable, which allows teams to update their microservices on their own schedules. Other microservices are only affected when a breaking change is made to the interface of a microservice. These traits of microservices lead to more agile development, because microservices can be separately updated and deployed without affecting other services. Another benefit is that microservices can use different programming languages and technologies. Microservices connect using an API interface. The programming languages, frameworks, and technologies used by the microservice code do not affect calling services. A team can choose the languages and technologies that best suit their service. Microservices running on one platform can also connect to microservices running on a different platform. Microservices, which typically connect using HTTP APIs, can call each other without worrying about where the service is located. A third benefit of microservices is the ability to separately scale microservices. Each microservice can be scaled separately, dedicating more resources only to those services that require more capacity. Microservices are typically easy to scale up and down based on fluctuations in traffic. Instead of building the infrastructure required when the load is highest, the infrastructure, and therefore cost, can be optimized based on the current traffic requirements.

### Video - [Challenges of microservices architectures](https://www.cloudskillsboost.google/course_templates/465/video/511513)

* [YouTube: Challenges of microservices architectures](https://www.youtube.com/watch?v=hYDwVrxCvec)

The microservices architecture is a common architecture for new enterprise applications being developed today. However, microservices architectures also provide significant challenges. In a microservices architecture, each microservice tends to be simpler and easier to understand than the monolithic application. Each service can be developed, deployed, and tested separately. However, having more deployable entities causes a greater operational burden for an organization. The operations team must manage tens, hundreds, or thousands of microservices. Automated builds, testing, and deployments are vital to maintaining the health and efficiency of your applications and your operational team. With so many services, it's also important to maintain consistent logging, reporting, security, and authorization for your services. A microservices architecture includes the communication between microservices, which can be complex. If you do not design your systems well, it can be difficult to understand the "spider web" of communication between microservices. Microservices can also introduce communication latency. For a monolith, calls between components are typically in the same process running on the same hardware. With microservices, calls between services happen across the network, which can be thousands of times slower. When a business operation requires many microservice calls, the latency can be significant. While unit testing for each microservice can be straightforward, integration testing is typically more challenging. The distributed nature of microservices often means that testing the entire system requires modeling the entire production deployment. Debugging a microservices architecture can also be difficult. If an application consists of many microservices, and each microservice creates its own logs, tracing calls that span many microservices can be challenging. Building microservices requires a commitment to automation and operational excellence. The benefits of microservices generally outweigh the challenges, and we will see how service orchestration and choreography can reduce the complexity of microservice-based applications.

### Quiz - [Quiz: Introduction to Microservices](https://www.cloudskillsboost.google/course_templates/465/quizzes/511514)

#### Quiz 1.

> [!important]
> **In which situation does it make sense to start developing your application as a monolithic application instead of using microservices?**
>
> * [ ] Agile service delivery is a priority.
> * [ ] Your team does not have expertise in the problem domain.
> * [ ] You plan to grow the team.

#### Quiz 2.

> [!important]
> **Which of the following is a benefit of a microservices architecture?**
>
> * [ ] Microservices are separately deployable.
> * [ ] An application composed of microservices leads to simpler communication patterns.
> * [ ] A microservices architecture typically results in improved communication latency.

### Video - [Module summary](https://www.cloudskillsboost.google/course_templates/465/video/511515)

* [YouTube: Module summary](https://www.youtube.com/watch?v=ikTWV8QzYHY)

This is the end of the first module of the course "Service Orchestration and Choreography in Google Cloud." In this module, "Introduction to Microservices," you learned about microservices, which were compared to monolithic and SOA applications. You also learned about the benefits and challenges of using a microservices architecture.

## Event-Driven Applications

This module introduces events and event-driven applications and discusses the benefits of choosing an event-driven architecture for your microservices applications.

### Video - [Module overview](https://www.cloudskillsboost.google/course_templates/465/video/511516)

* [YouTube: Module overview](https://www.youtube.com/watch?v=Hu74QTMAJEY)

Welcome to module 2 of Service Orchestration and Choreography on Google Cloud: Event-Driven Applications. In this module, you learn about event-driven architecture, a useful pattern for communication when using microservices. You also learn about the benefits of using event-driven architecture for your applications.

### Video - [Event-driven architecture](https://www.cloudskillsboost.google/course_templates/465/video/511517)

* [YouTube: Event-driven architecture](https://www.youtube.com/watch?v=D5i8Oct0umA)

Many applications built using microservices will benefit from an event-driven architecture. Before we discuss event-driven architecture, we must understand events. An event is a record of something that has happened. Examples of events are an employee logging in to an application or a product being added to a shopping cart. That definition may seem obvious. However, when we are discussing event-driven architectures, there are other important attributes of events. First, an event is typically treated as an immutable fact. It's an historical record of an occurrence, and it should not be modified or deleted. Second, an event can be generated even if it's never consumed. Many applications that produce events don't know whether the events they generate are ever consumed. Third, an event can be persisted indefinitely, and can be consumed as many times as necessary. A single event can be consumed by many services, allowing event processing to occur in parallel. As discussed earlier, the "spider web" of point-to-point communication between microservices can be a challenge. Each service must know how to communicate with all downstream services. Point-to-point communication tends to introduce coupling between the microservices. An event-driven architecture inserts an event intermediary between the services. When a service acts as an event producer, it sends events to the intermediary. It isn't necessary for the service to know anything about the services that are consuming the events. A service can also act as an event consumer, receiving events from the intermediary. Event consumers understand how to handle an event. The consumers do not have to know any details about the event producer.

### Video - [Benefits of event-driven applications](https://www.cloudskillsboost.google/course_templates/465/video/511518)

* [YouTube: Benefits of event-driven applications](https://www.youtube.com/watch?v=cuhwzy-DFD0)

There are several benefits of event-driven applications. A centralized event service can simplify the auditing and control for a distributed application. A log of immutable events can be used for auditing purposes. Events can provide a timed, ordered record of every change to the state of an application. A centralized event service can also help you control access to particular services and data. By requiring authentication and authorization at the event service, you can limit access to each of your event-based services. When using an event intermediary, the producer and consumer of an event are decoupled. Services can create an event without having to send direct requests to any services that consume the event. Services can also consume an event without knowing anything about the service that generated the event. This decoupling means that there's no point-to-point spider web of communication. Each event travels through the event intermediary, which routes the event to the correct consumer or consumers. A producer or consumer is only required to know the format of a specific event. An extra benefit of this decoupling is that new event consumers can be added to your application without modifying any existing services. Microservices applications are sometimes designed to use synchronous request/response calls. The health of a service is affected by the health of the services that it calls, directly or indirectly. When a single service fails... ...it can bring down your entire application. With an event-based architecture, events are generated asynchronously, and events are created without waiting for a response. An architecture can be designed to survive the temporary loss of a service. Events sent to the unhealthy service can be replayed or redelivered when the service comes back up. This asynchronous handling of events leads to more resilient applications. When services are asynchronous, push-based messaging allows clients to receive updates without needing to continuously poll remote services. When using a polling model, consumers must continuously poll to determine when there's work to be done. Polling typically leads to increased network I/O and unnecessary delays in processing. A push-based model allows consumers to automatically be notified when there are events to be consumed. Events are efficiently routed to consumers.

### Quiz - [Quiz: Event-Driven Applications](https://www.cloudskillsboost.google/course_templates/465/quizzes/511519)

#### Quiz 1.

> [!important]
> **When using an event-driven architecture, which of the following is true about an event?**
>
> * [ ] An event should be deleted after it has been consumed.
> * [ ] An event should always be consumed at least once.
> * [ ] An event consumer does not need to know which service generated the event.

#### Quiz 2.

> [!important]
> **Which of the following features of event-driven applications causes them to be more resilient than non-event-driven applications?**
>
> * [ ] Multiple services may consume a single event.
> * [ ] Events are created without waiting for a response.
> * [ ] Events may be used for auditing purposes.

### Video - [Module summary](https://www.cloudskillsboost.google/course_templates/465/video/511520)

* [YouTube: Module summary](https://www.youtube.com/watch?v=Rtnc71kfo0k)

This is the end of the second module of the course "Service Orchestration and Choreography in Google Cloud." In this module, "Event-Driven Applications," you learned about event-driven architecture. You also learned about the benefits of building event-driven applications.

## Choreography and Orchestration

This module introduces two effective patterns for inter-service communication: choreography and orchestration. Eventarc uses the choreography pattern, which allows independent services to perform tasks when events are received. Workflows uses orchestration, and acts as a central orchestrator of the interactions between the services. You learn how Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler can be used to build powerful microservices applications on Google Cloud.

### Video - [Module overview](https://www.cloudskillsboost.google/course_templates/465/video/511521)

* [YouTube: Module overview](https://www.youtube.com/watch?v=-IRrZnZH9_E)

Welcome to module 3 of Service Orchestration and Choreography on Google Cloud: Choreography and Orchestration. In this module, you learn about two primary patterns for coordinating microservices: choreography and orchestration. We explore the choreography pattern. You learn how Pub/Sub and Eventarc can help you choreograph communication between microservices. We also discuss when you should use Eventarc for your applications. You also learn about Workflows, Google Cloud's orchestration service. We discuss when Workflows is the correct coordination solution. We compare the use cases for choreography and orchestration, and you learn how each pattern can be used in your applications. You learn about Cloud Tasks, a service that helps you manage asynchronous HTTP requests. You learn about Cloud Scheduler, a service for managing scheduled jobs. Finally, this module concludes with a lab where you use all of these Google Cloud services to create a machine learning-driven image application.

### Video - [Coordinating microservices](https://www.cloudskillsboost.google/course_templates/465/video/511522)

* [YouTube: Coordinating microservices](https://www.youtube.com/watch?v=9cKxqYwL-fI)

One challenging aspect of using a microservices architecture is coordinating the communication between microservices. When you use a microservices architecture, you benefit from scalability, reusability, and ease of change. Each microservice is smaller and simpler to design than a monolithic application, but some complexity is shifted from the service to inter-service communications. Multiple microservices are often combined to form business processes. The coordination of the communication becomes a key aspect of the design of your application. There are two basic approaches to coordination in an event-driven architecture: service choreography and service orchestration. Service choreography has similarities to the choreography of a dance performance. When a dance is choreographed, the dancers are instructed how to perform the dance, but dancers are fully responsible for performing their parts during the performance. With service choreography, each service works independently. Each service is responsible for receiving and sending events asynchronously, typically following defined rules of interaction between services. The event structures that are exchanged between services are specified, and each service must generate and expect services in the correct formats. With choreography, services are loosely coupled, and can be created, changed, and scaled separately. One choreography challenge is that the business logic is distributed. A distributed application can be harder to understand because there's no central source of truth. Service orchestration is similar to an orchestra performance. Each musician in the orchestra knows how to play their instrument, but the conductor takes an active role during the performance to ensure that the musicians are synchronized. With service orchestration, each service performs its own tasks, but the central orchestrator controls all interactions between the services. Services do not need to know about or communicate with other services in the orchestration. As with service choreography, the services are loosely coupled, and can be created, changed, and scaled separately. Another benefit of orchestration is that it provides a high-level view of business processes which helps with understanding the application, tracking execution, and troubleshooting issues. Unlike the fully distributed services in the service choreography pattern, service orchestration has a single point of failure. If the orchestrator is not operable, the orchestrated processes cannot run.

### Video - [Choreography in Google Cloud](https://www.cloudskillsboost.google/course_templates/465/video/511523)

* [YouTube: Choreography in Google Cloud](https://www.youtube.com/watch?v=J33V9EXfFsg)

Now that you understand the basics of service choreography and orchestration, we will discuss how you can choreograph services in Google Cloud. Pub/Sub is one of the services on Google Cloud that can be used to choreograph services. Pub/Sub is a fully managed real-time messaging service that lets you send and receive messages between independent services or applications. A publisher sends a message to a Pub/Sub topic. This publisher is often a custom-built application, but it could also be a Google service. The message is stored within Pub/Sub... ...and then delivered to the message queue for each subscriber for the topic. Each Pub/Sub subscriber then receives the message. A subscriber with a pull subscription would occasionally poll for messages that have been sent to the topic. A push subscription would cause the message to be automatically sent to a configured endpoint for the subscription. The subscriber would then acknowledge the message. Acknowledging a message removes it from the queue. The deletion of the queued message follows handling of the message, which guarantees that a message will be handled at least once. Here's an example of using Pub/Sub to connect services and build an application. This diagram shows an image resizing application. A Pub/Sub topic is created for image uploads. A specific Cloud Storage bucket is configured to send a Pub/Sub message to that topic when a new image is received. When the mobile device application uploads a new image to the Image Uploads bucket, a Pub/Sub message is automatically sent to Pub/Sub. This message is then forwarded to the two subscribers, the Resizing Service and the Upload Confirm application. The Upload Confirm application updates Firestore, storing the fact that the image upload completed successfully. The Resizing Service resizes the image, storing it in the Resized Images bucket and also updating Firestore with the status. The application can track status updates in Firestore using Firebase Realtime Database updates. Each of the Cloud Run services can remain fairly simple, with Pub/Sub initiating processing when there's an image to act upon. Eventarc is Google Cloud's fully managed eventing system that makes building event-driven applications easy. Eventarc supports many Google Cloud products as event sources. For some Google Cloud services, the source can directly send events to Eventarc. For Google services or event types that do not support direct access, Eventarc can seamlessly use Cloud Audit Logs entries to generate events. Third-party providers can also utilize the Eventarc API to create events. Applications don't need to write code to parse audit logs or poll for events. Pub/Sub messages to specified topics may also be used as event sources. This integration allows custom applications to send events. An event trigger is a rule-based filter to route specific event types from a particular event source to specified event consumers, or targets. Eventarc uses Pub/Sub as its transport layer due to its superior reliability and observability. Eventarc automatically creates and manages Pub/Sub topics and subscriptions to facilitate event delivery. Your applications only need to accept HTTP requests that are automatically sent by Eventarc. Applications do not need to use Pub/Sub directly. Events are delivered to targets using the standard CNCF CloudEvents format, regardless of event source. Whenever you create a trigger, you can see the format and fields that will be used for that specific event. The CloudEvents format used by Eventarc specifies a common metadata format for describing event data, providing interoperability across services, platforms, and systems. Publishers of events historically tended to use their own formats for their events. By standardizing on a specific format, CloudEvents allows developers to use the same event handling logic in their code regardless of the source or type of the event. CloudEvents provides SDKs for many of the common programming languages in use today, like Python, JavaScript, Java, Go, C#, Ruby, and PHP. Developers can use these SDKs to easily parse incoming events, increasing code portability and developer productivity. Eventarc is an abstraction layer on top of Pub/Sub that provides some significant benefits when designing an event-driven application. Eventarc can use many built-in services as a source for events. Eventarc makes it easy to detect changes within many Google Cloud services and third-party applications, and automatically trigger code to run in response to those changes. Eventarc provides a simple, rule-based interface to select the source, filter, and destination of a trigger. With Pub/Sub, you must write code to ingest events and manage topics and subscriptions. Finally, you should use Eventarc when you want a standardized event format. By using the standard CloudEvents format, you can use CloudEvent SDKs to create and consume events.

### Video - [Orchestration in Google Cloud](https://www.cloudskillsboost.google/course_templates/465/video/511524)

* [YouTube: Orchestration in Google Cloud](https://www.youtube.com/watch?v=O8rFzTqZcwQ)

Google Cloud's Workflows platform can be used to implement the service orchestration pattern. Workflows is a fully managed orchestration platform which acts as the central orchestrator for the service orchestration pattern. You design and deploy workflows, which orchestrate Google Cloud services and API calls, to build stateful, automated processes. A workflow provides a central source-of-truth for the application flow. Each execution of a workflow is logged and is observable, which makes it easier to understand the current state of the workflow and troubleshoot any issues. A workflow can hold state, retry, poll, or wait for up to a year. This flexibility allows for creation of long-running business processes. Here's an example product ordering workflow. The first step in the workflow process is to check the Firestore inventory database for availability of the ordered products. If the items are available, they are locked. The workflow follows one of two paths, depending on whether any of the items are out of stock. The out of stock boolean condition is available throughout the workflow, and is also used at the end of the process. If every item in the order is available, the workflow calls a Cloud Run function to prepare the order confirmation message. If one or more items is out of stock, a Cloud Run service is triggered to request more inventory from the relevant suppliers. After the Cloud Run service is called, a "we're sorry" message is prepared for the customer. Next, the inventory and order details are updated in the Firestore databases. The customer is then sent an email indicating whether the order was successful or not. Finally, if one or more items is out of stock, a Slack message is posted to notify the sales rep. Each workflow execution, which handles a single transaction, is logged for troubleshooting or tracing. The workflow handles retries or exceptions thrown by APIs, improving the reliability of the entire process. Workflows is an excellent choice when you want to chain HTTP-based microservices into durable and stateful workflows. Workflows lets you implement long-running processes and maintain observability for each execution. Workflows is also a great choice for performing operations on a set of items or batch data. Robust error handling can guarantee that each item is processed correctly.

### Video - [Should I use choreography or orchestration?](https://www.cloudskillsboost.google/course_templates/465/video/511525)

* [YouTube: Should I use choreography or orchestration?](https://www.youtube.com/watch?v=S8yglkyMU2E)

Now that you've learned how choreography and orchestration work in Google Cloud, which pattern is better, choreography or orchestration? Like many application architecture decisions, the answer is "it depends." The better question is "when should I use choreography, and when should I use orchestration?" When you use event-based choreography, you rely on the receiving service to control the communication. When Service A completes some work and sends an event, Service A has no idea whether any other service will act on that event. It is not the responsibility of Service A to know whether any downstream service or services are consuming the event. Using Eventarc, most Google Cloud or custom services can act as an event producer. A receiver of an event, though, must understand the details of the event to be consumed. In the example shown here, Service B consumes the event that was sent by Service A. Service B understands the formatting of the event and how to act on the event. Service B might also know that the event was sent by Service A, but it is not directly coupled to Service A. It's possible to implement the product ordering flow using choreography. Each service would send an event to indicate readiness for the next step in the process. The "out of stock" decision points could be implemented by specific services, deciding whether to send the "in stock" or "out of stock" events. However, an enterprise order system requires visibility, error handling, and retries. Implementing these features in an event-based solution can be difficult. How would you troubleshoot issues with an event-based system? What happens if the process somehow aborts between locking the inventory in the database and updating the inventory and order? How do you make sure that requests are successfully sent to suppliers? With orchestration, each workflow execution is tracked separately. The ordering process logic, which may be built using many services or functions, is defined in a single location. Retries and error handling can provide a reliable order handling flow. Sometimes, your architecture requires decentralized control which cannot be provided by a single orchestrated workflow. With orchestration, if these services are built and managed by different teams or organizations, shared management of the central orchestration process can be difficult. Choreography provides decentralized control, where each of the services or applications connects to the others using events. Each service can be separately managed by a different team or organization. Orchestration is a strong pattern when you want to control a complex process that you can manage centrally. Choreography is more appropriate when combining separate, decentralized services and applications using events, or when you want to leverage events from Google Cloud services. You may find that using Workflows and orchestration provides the visibility, error handling, and reliability required to create your complex services. You can use Eventarc to send events between the services. In the example shown here, the Order, Fulfillment, and Marketing services are implemented using Workflows. Event triggers between the services and the detection of new order files being uploaded into a Cloud Storage bucket are implemented using Eventarc.

### Video - [Cloud Tasks](https://www.cloudskillsboost.google/course_templates/465/video/511526)

* [YouTube: Cloud Tasks](https://www.youtube.com/watch?v=WbvkN8Hojzs)

Cloud Tasks lets you manage the execution, dispatch, and delivery of large numbers of distributed tasks. A task is a piece of work that can be processed independently by dispatching it to an HTTP service. You can set up a queue for tasks that will be sent to a particular service. A task added to this queue will be automatically dispatched to your chosen HTTP service. The returned status code indicates whether the task has been completed successfully or should be retried. When sending a task to a queue, you can schedule the task to be dispatched at a specified future time. You can configure the queue with a maximum rate to dispatch tasks or a maximum number of tasks that can be dispatched concurrently. You can also specify the maximum number of attempts and the delay between attempts when tasks are retried. Cloud Tasks also guarantees at-least-once delivery and eliminates any duplicate tasks that are created. HTTP services that require authentication may be called by automatically attaching a token associated with the service account of the application creating the task. Although Cloud Tasks and Pub/Sub are conceptually similar, both implementing message passing and asynchronous integration, they are designed for different use cases. With Cloud Tasks, the task creator uses explicit invocation, where the creator retains full control over the execution and destination of the task. The creator places the task in a queue attached to a specified endpoint, and the creator can defer the dispatching of the task. With Pub/Sub, the message publisher uses implicit invocation. The publisher implicitly causes any subscribers to execute by publishing the message, but the publisher has no control over which subscribing services receive the message. Cloud Tasks is appropriate for use cases where an application wants to asynchronously execute a specific service, and possibly control the timing of the execution. Pub/Sub should be used for event-based architectures that rely on receiving services reacting to events generated by other services. Cloud Tasks does a great job of separating out independent pieces of work to be processed asynchronously. Slow background operations can be offloaded to a separate worker, reducing the work required by the main application and improving response time. Unlike Pub/Sub, the application retains control of the execution, specifying the endpoint to handle the offloaded task. Cloud Tasks lets you configure retries, scheduling, and rate limiting.

### Video - [Cloud Scheduler](https://www.cloudskillsboost.google/course_templates/465/video/511527)

* [YouTube: Cloud Scheduler](https://www.youtube.com/watch?v=P8MMtjSrnv0)

Another managed service that can be used in your orchestration and choreography designs is Cloud Scheduler. Cloud Scheduler is a fully managed, enterprise-grade cron job scheduler which can be managed from a single dashboard. Cloud Scheduler is used to schedule jobs that should be executed on a defined schedule or at regular intervals. Jobs are specified using the familiar Unix cron job format, allowing a job to be run multiple times a day or on specific days and months. Jobs can be sent to Pub/Sub topics, App Engine applications, or publicly accessible HTTP endpoints. Like Cloud Tasks, Cloud Scheduler can attach tokens associated with a specified service account to HTTP requests. Jobs also have guaranteed execution, and failed job executions can be retried. The Unix cron string format is a set of five space-separated fields on a single line that indicates when a job should be executed. The first field is the minute. A 15 in this field means that the job would execute 15 minutes past the hour. The second field is the hour. A 0 in this field indicates that the job executes within the hour following midnight. The third and fourth fields are the day of the month and month respectively. These fields limit execution to the specified days of the month and months. The last field is the day of the week, ranging between 0 for Sunday and 6 for Saturday. A field can contain a single number, a range of numbers, or a list of numbers and ranges. Ranges are two numbers separated by a hyphen, and the range is inclusive. An asterisk indicates the entire allowed range. Following a range with a slash and a number will skip that number of values throughout the range. An hour setting of "* / 2" would indicate that the execution should occur every two hours. A list of numbers or ranges can be specified by separating the values with commas. Your job schedule can be specified for a specific time zone. The default timezone is UTC. Time zones with daylight saving time can cause jobs to be skipped (when clocks are set forward) or run twice (when clocks are set backward). Using the UTC time zone is recommended to avoid this issue. Cloud Scheduler is Google Cloud's solution for scheduling recurring jobs. Scheduled jobs are managed from a single dashboard. Jobs are created using the industry-standard unix-cron format, and can trigger Pub/Sub messages and securely call Cloud Run functions, Cloud Run services, or HTTP endpoints. Many of the previous examples come from this sketch note "Service Orchestration in Google Cloud." This sketch note introduces the tools that make up the Application Integration toolbox. A full-featured application, developed using a microservices architecture, may benefit from any or all of these services. Now you understand when to use choreography and orchestration, and how these application integration products can help you create compelling and maintainable applications.

### Video - [Lab intro: Building Event-Driven Orchestration on Google Cloud](https://www.cloudskillsboost.google/course_templates/465/video/511528)

* [YouTube: Lab intro: Building Event-Driven Orchestration on Google Cloud](https://www.youtube.com/watch?v=ddioDlEpPG8)

Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler provide a powerful set of features that can be used to create exciting applications when using a microservices architecture. In this lab, you use these four services to implement a series of steps that occur when an image is added to a Cloud Storage bucket. You create an Eventarc trigger that detects when an image file is uploaded to a Cloud Storage bucket. The trigger starts a workflow to analyze the image and create a thumbnail. Another Eventarc trigger will run a Delete Image service in Cloud Run when an image file is deleted from the bucket. You create a workflow that receives the file creation event from Eventarc. This workflow calls Cloud Vision to analyze the photo, and then the workflow extracts metadata from the Cloud Vision response. If the image content is safe, the image metadata is stored in Firestore, and a Cloud Task is queued to create an image thumbnail. The Cloud Task starts a Cloud Run service that creates a thumbnail of the uploaded image. Finally, Cloud Scheduler starts a Cloud Run service every minute to create a collage of the latest image thumbnails. This lab shows how easy it is to build compelling applications in Google Cloud using Eventarc, Workflows, Cloud Tasks, and Cloud Scheduler.

### Lab - [Building Event-Driven Orchestration on Google Cloud](https://www.cloudskillsboost.google/course_templates/465/labs/511529)

In this lab, you build an event-driven orchestration of microservices that processes images. You will use four services that support application integration on Google Cloud: Workflows, Eventarc, Cloud Tasks, and Cloud Scheduler.

* [ ] [Building Event-Driven Orchestration on Google Cloud](../labs/Building-Event-Driven-Orchestration-on-Google-Cloud.md)

### Quiz - [Quiz: Choreography and Orchestration](https://www.cloudskillsboost.google/course_templates/465/quizzes/511530)

#### Quiz 1.

> [!important]
> **Which of the following are features of Eventarc? Select two.**
>
> * [ ] Pub/Sub is the transport layer.
> * [ ] Event formats are flexible as long as the formatting is identical for all events of a particular type.
> * [ ] Applications handle events by monitoring the events that are published to an event queue.
> * [ ] Eventarc can generate events for entries written to Cloud Audit Logs.

#### Quiz 2.

> [!important]
> **Which of the following are features of Cloud Tasks? Select two.**
>
> * [ ] Tasks can be scheduled for delivery at a future time.
> * [ ] At-least-once delivery is guaranteed.
> * [ ] HTTP destinations may be called by automatically attaching a token for the Cloud Tasks service account.
> * [ ] The creator of a task has no control over which endpoint receives the task.

#### Quiz 3.

> [!important]
> **Which of the following are features of Workflows? Select two.**
>
> * [ ] Workflows supports long-running processes.
> * [ ] A workflow provides a decentralized view of event communication.
> * [ ] A workflow is appropriate only for simple business processes.
> * [ ] The state of each workflow execution is observable.

#### Quiz 4.

> [!important]
> **Which of the following are benefits of the service choreography pattern? Select two.**
>
> * [ ] An event producer maintains full control over downstream operations.
> * [ ] Service choreography allows for decentralized control.
> * [ ] Business logic is easy to understand.
> * [ ] Services are loosely coupled.

### Video - [Module summary](https://www.cloudskillsboost.google/course_templates/465/video/511531)

* [YouTube: Module summary](https://www.youtube.com/watch?v=OXa1wRW-5TM)

You've reached the end of the course "Service Orchestration and Choreography in Google Cloud." In this module, "Choreography and Orchestration," you learned about two popular microservices coordination patterns, choreography and orchestration, and you learned when you should use each pattern. You learned about how Pub/Sub and Eventarc support choreography, and how Workflows allows for service orchestration. We also discussed Cloud Tasks and Cloud Scheduler. We finished with a lab that demonstrated these patterns and used these application integration services to build an application.

## Course Resources

Links to module PDFs

### Document - [Course Resources](https://www.cloudskillsboost.google/course_templates/465/documents/511532)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
