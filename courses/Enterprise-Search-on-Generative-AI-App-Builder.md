---
id: 612
name: 'Enterprise Search on Generative AI App Builder'
datePublished: 2023-10-02
topics:
- Search
- Generative AI
- Web Development
type: Course
url: https://www.cloudskillsboost.google/course_templates/612
---

# [Enterprise Search on Generative AI App Builder](https://www.cloudskillsboost.google/course_templates/612)

**Description:**

Enterprises of all sizes have trouble making their information readily accessible to employees and customers alike. Internal documentation is frequently scattered across wikis, file shares, and databases. Similarly, consumer-facing sites often offer a vast selection of products, services, and information, but customers are frustrated by ineffective site search and navigation capabilities.

This course teaches you to use Generative AI App Builder to integrate enterprise-grade generative AI search.

**Objectives:**

- Understand the different Generative AI product offerings in Google Cloud and their enterprise use cases.
- Learn to create an Enterprise Search engine and index several data sources.
- Configure search results outputs and analyze search accuracy.
- Integrate Enterprise Search in your applications and websites.

## Introduction

Introduce learners to the course

### Video - [Course Introduction](https://www.cloudskillsboost.google/course_templates/612/video/412250)

- [YouTube: Course Introduction](https://www.youtube.com/watch?v=bOiyxNK55XU)

Welcome to the course Enterprise Search on Generative AI App Builder. This course is intended for Developers that have some coding experience. You will be referencing examples of how to use the APIs and SDKs to access Enterprise Search on Generative AI App Builder. In this course, you’ll learn: The different Generative AI product offerings in Google Cloud. You'll explore several use cases where Generative AI App Builder can provide better search and recommendation experiences. And, the gain a better understanding of the Enterprise Search product architecture and how to configure the product to be secure, accessible, and cost effective. You’ll also learn to... Index several data sources in the search engine. Display only information of interest in search results. Integrate Enterprise Search in your applications. And, understand product usage through analytics and metrics. Please be aware that this is a rapidly evolving space and you can expect this course to update over time. Some aspects don’t fully reflect the current state of the product, and some of the features are still in development. With that said, let’s get started with the course.

## Generative AI on Google Cloud

Define generative AI, its history and product offerings on Google Cloud, and the target personas for each product.

### Video - [History of AI at Google](https://www.cloudskillsboost.google/course_templates/612/video/412251)

- [YouTube: History of AI at Google](https://www.youtube.com/watch?v=RBWmiMJbLGs)

Welcome back to the course Enterprise Search on Generative AI App Builder. This is the Generative AI on Google Cloud module. In this module, you'll explore the history of AI at Google, Generative AI building blocks, and Generative AI products in Google Cloud. Let’s start at the beginning with the history of AI at Google. The Generative AI revolution started at Google, and Google continues to lead the way in Large Language Models and enterprise solutions. These innovative large language models already power a range of Google Cloud AI products and many others. There are different types of AI models. Machine Learning or predictive AI are the most classical models, which are trained on historical data to classify or make predictions on similar data. For example, you would train a vision model to identify whether the animal is a cat, by providing a dataset of images labeled as cats or other animals. Then, when you provide a new image, the predictive model will be able to tell you whether it is a cat. Generative AI is the new paradigm, which creates new data based on the patterns it has learned from training data. Training data is general and not specific to a particular task. It can come in several formats of unlabeled data, such as images, text, or audio. In the pre-training stage, large general datasets are used. Later smaller and more specific datasets are used to fine-tune the model. Once the model is trained, it can generate new, unique data that it has not seen before. Google Cloud products empower enterprises to embrace Generative AI with the confidence that there's Data Governance built-in. This is especially important in highly regulated industries like financial services and healthcare. You need a guarantee that no one can see the questions your users are asking or the training data that provides your unique competitive advantage. Google Cloud doesn’t believe that one model fits all. In fact, bigger is not better, especially from a cost of inference perspective. Large 300 billion-parameter models can cost as much as $1000 per user, per year to run. Which adds up to $1B for one million users. You shouldn't need to use a public model that has to search through the player rosters in every world cup, or the inspiration for every Taylor Swift song, in order to answer a question like: “when can I withdraw from my retirement account?”. Instead, Google Cloud provides match to cost value that gives you the ability to choose the right model for the right job. In the enterprise it's important not just to provide an answer, but to prove where the answer came from, and what information was used to create the answer. This process ensures that your results are grounded in factuality. Enterprise customers have built stores of knowledge, and data warehouses filled with facts. They also integrate many third party data sources with highly curated facts. Google Cloud provides a wide range of easy to use tools, including out-of-the-box Search and Conversation, and quick access APIs. This helps you to get started in days, rather than requiring you to learn the deep mathematics in Generative AI or tune a model to every possible question that could be asked. Enterprises will need to manage many models, user interfaces, data corpora, and integrations with first and third-party data sources. Google Cloud provides a manageable-at-scale platform that integrates into your existing user security, data management, and entitlements workflow. Generative AI comes with its own set of unique challenges. At Google, we are integrating AI into our products boldly and with a deep sense of responsibility the highest standards of information integrity with our AI principles. This includes education, research, and tools, including online training courses such as this one, guidebooks, research papers, and our product documentation. There are also product and use case reviews, such as customer AI use case reviews, product development reviews, and fairness testing. Additionally, there are highly relevant responsible AI resources and tooling for new generative AI offerings. These are being rapidly developed and will be coming soon. In continuous development are governance and assurance tooling to support the responsible development and implementation of AI. In 2022, the Vertex AI Explainable AI offerings were expanded to include new features as part of Model Evaluation, Model Monitoring and Model Registry to support data and model governance. This is in addition to Google’s open source Responsible AI Toolkit that is available to Google Cloud customers for their projects and anyone with an AI project at no cost.

### Document - [Generative AI building blocks](https://www.cloudskillsboost.google/course_templates/612/documents/412252)

### Document - [Generative AI products in Google Cloud (Vertex AI and Gen App Builder)](https://www.cloudskillsboost.google/course_templates/612/documents/412253)

### Video - [Generative AI products in Google Cloud (Enterprise Search and Cloud Retail Search)](https://www.cloudskillsboost.google/course_templates/612/video/412254)

- [YouTube: Generative AI products in Google Cloud (Enterprise Search and Cloud Retail Search)](https://www.youtube.com/watch?v=_HXtgNO1QUA)

In this lesson you'll learn whether to use Enterprise Search or Cloud Retail Search in your solution. With access to Google’s no-code conversational and search tools powered by foundation models, organizations can get started with a few clicks. They can quickly build high-quality experiences that can be integrated into their applications and websites. There are three key elements to Generative AI App Builder: Enterprise Search, where you can build a Google-quality search engine on your own data and embed a search bar in your web page or application. Personalized self-serve customer experiences, such as building a state-of-the-art recommendation engine on your own data that can suggest content similar to the content that the user is currently viewing. And, Generative AI Agents, which complements Dialogflow CX with an LLM-based chatbot trained on links or documents, so that your end users can have conversations about the content. Now let’s explore Enterprise Search in a little more detail. There are two key components to Enterprise Search, the Enterprise Search Platform, and Cloud Retail Search. Enterprise Search is a horizontal search platform that isn't industry-specific. It's used to build an AI-enabled search capability and embedded vertical solution. Developers and Data Scientists from a wide range of industries have started to use Enterprise Search… for use cases such as Medical records history, Artifacts Search, Customer Support, and Manufacturing Inventory Search. Enterprise Search helps deliver more relevant results than traditional keyword-based search techniques by using Natural Language processing and machine learning techniques. This allows Enterprise Search to infer relationships within the content and the intent of the user’s query input. Enterprise search is something you can build on top of, however it’s not going to have the retail-specific tuning. That’s where Cloud Retail Search comes into play! Cloud Retail Search can be considered a vertical-specific, pretuned instance of the Enterprise Search platform. It’s industry-specific for ecommerce and external catalog services optimized for ecommerce transactions. Suppose you're an ecommerce business looking to use a fully-managed service to increase the performance of the Revenue Per Visit of your digital properties. In that case, Cloud Retail Search is the right choice. Cloud Retail Search is an Industry solution for retailers and ecommerce; providing personalized product search, browsing, and recommendations. It is tuned for retail through large language models, which means it is not tuned for clicks or conversion prediction, but rather revenue prediction with access to Google shopping data. And the Time to value for Cloud Retail Search is as fast as 6 - 12 months. Also because they are complementary products, customers that upgrade to Enterprise Search enhance their benefits from Cloud Retail Search. So some important questions to ask when trying to decide between Enterprise Search and Cloud Retail Search could be: Are you earning revenue online? Are you selling products? Does each product have its own price? Does your data fit the retail product catalog schema? And, are you interested in optimizing for Profit and Loss? Another factor that can affect your decision is your team's application development and AI skills. Google Cloud’s out-of-the-box search products are fast and easy to set up even if your application developers have no Machine Learning experience. To develop a customized or tuned search product, your developers should have a firm understanding of Machine Learning. And to create a fully custom built Search product, you will require AI practitioners with advanced machine learning abilities in model training and tuning. It's important to know that 'Tunable search' and 'Build your own search' are future capabilities of the product still in development and will be available soon.

### Quiz - [Generative AI on Google Cloud Quiz](https://www.cloudskillsboost.google/course_templates/612/quizzes/412255)

#### Quiz 1.

> [!important]
> **Which products should you use for your enterprise use cases?**
>
> - [ ] MakerSuite + Generative AI App Builder
> - [ ] Bard + Vertex AI
> - [ ] Bard + MakerSuite
> - [ ] Vertex AI + Generative AI App Builder

#### Quiz 2.

> [!important]
> **What tool should you use to provide search functionality in your financial services product?**
>
> - [ ] Enterprise Search
> - [ ] BigQuery
> - [ ] Cloud Retail Search
> - [ ] Google Cloud Search

#### Quiz 3.

> [!important]
> **What product should an enterprise use if they don't have any ML expertise?**
>
> - [ ] Generative AI App Builder
> - [ ] VertexAI
> - [ ] MakerSuite
> - [ ] Bard

#### Quiz 4.

> [!important]
> **What features are available as part of Generative AI App Builder?**
>
> - [ ] Enterprise Search, Personalize, Dialogflow Agents
> - [ ] Conversational AI, Coding, Personalize
> - [ ] Enterprise Search, Coding, Personalize
> - [ ] Enterprise Search, Image Generation, Conversational AI

## Enterprise Search Use Cases

Discover several use cases where Generative AI App Builder can provide better search and recommendation experiences.

### Video - [Enterprise Search with Generative AI](https://www.cloudskillsboost.google/course_templates/612/video/412256)

- [YouTube: Enterprise Search with Generative AI](https://www.youtube.com/watch?v=fiqwD1nnc1o)

Welcome back to the course Enterprise Search on Generative AI App Builder. This is the Enterprise Search Use Cases module. In this module, you'll explore Enterprise Search with Generative AI, Then look at use cases for Enterprise Search; an intranet website search and a public website search. Let’s begin by exploring Enterprise Search with Generative AI in more detail. There are three main challenges when implementing a search service for an enterprise. First, the service level requirements for any enterprise search service is high. Most organizations don’t have the time or budget to build service that is capable of handling large amounts of data in a wide variety of formats, all while being scalable and available 24 7. The second challenge is that traditional keyword search is too restricted, especially for users who are familiar with AI powered search and recommendations on social media platforms and other apps. These experiences are standard today, but it’s much more difficult to implement. The third challenge is how to take advantage of Generative AI and Large Language Models or LLMs, that are the pinnacle of information retrieval technology. Generative AI App Builder with Enterprise Search from Google Cloud provides a simple to setup service that unifies all this information together and makes it easy to find. Gen App Builder supports creating search engines and chat interfaces. So let’s start by discovering how to bring the power of search to your applications. Gen App Builder is an out of the box solution, which means you can deploy a fully managed search engine quickly. You don’t have to build and lead an entire DevOps team to manage it. It also utilizes semantic search, which provides a next generation search experience. Enterprise Search provides LLM based summarization, multimodal search, and chatbot integration, utilizing the latest in Generative AI technology. One of the greatest features of Gen App Builder is its ease of use for developers. This is driving new opportunities, with the added benefits of operational efficiencies, cost savings, and value creation. For any type of analyst, whether that's a business analyst or a market analyst, Enterprise Search will improve time-to-value as you take large corpora of complex data and are able to search, navigate, extract insights, and understand that information. For example, LLMs can enable you to process market reports going back 30 years, and this is what could make the difference. For Customer Service operations, you can greatly improve the customer experience by making your online interactions more natural, conversational, and rewarding. When considering maximizing employee productivity and creative solutions, the ability to generate content at the click of a button is a game-changer. For example, if you're working on some code, you may visit Stack Overflow or search Google to find some solutions. You then copy and paste them into your project. However, with Generative AI, you can ask a chat bot to start or complete the code for you. Although it’s worth having someone double check that it actually works as expected. It’s the same process for writing a blog, social media copy or creating images. And for the more sophisticated user, like an AI practitioner that really wants to integrate systems into their existing platforms; the ability to integrate with Vertex AI and customize foundational models enables you to incorporate state of the art generative capabilities into your own internal platforms.

### Video - [A use case for an intranet website search](https://www.cloudskillsboost.google/course_templates/612/video/412257)

- [YouTube: A use case for an intranet website search](https://www.youtube.com/watch?v=0TpO5zmvQGo)

In this lesson you'll explore one of the main use cases for Enterprise Search with Generative AI App Builder: an intranet website search. This is an internal facing resource for an organization's private systems, documents, or data. Please be aware that the following use case examples don’t fully reflect the current state of the product and some of the features are still in development. These examples are here to raise awareness about what to expect from the product in the near future. Let’s explore the first use case on an intranet website search in a little more detail. Internal company search enables you to: Integrate Enterprise Search into your current internal systems, Find relevant information that is private to your organization, Integrate information stored in internal documents, such as PDF, CSVs, or data warehouses, And, find information that is publicly linked on user facing websites. Here is an example of an Internal facing search feature for an investment company which has been built using Gen App Builder and Enterprise Search, and integrated into the internal systems. A simple prompt in the search field returns a variety of both internal and external resources in a single user interface. Google Cloud wants to enable developers to imagine and build Generative Search Experiences for many Industry Applications. That’s why with Enterprise Search you can easily build a solution that includes: A conversational search field, A synthesized summary, With source citation and attribution built-in, And personal recommendations to further related data resources.

### Link - [Internal company search](https://www.cloudskillsboost.google/course_templates/612/documents/412258)

- [Internal company search](https://www.youtube.com/watch?v=kOmG83wGfTs)

### Video - [A use case for a public website search](https://www.cloudskillsboost.google/course_templates/612/video/412259)

- [YouTube: A use case for a public website search](https://www.youtube.com/watch?v=p-8HWcw56uY)

In this lesson you'll learn explore another use case for Enterprise Search: a public website search. For example if you have a catalog of hundreds of products and you wanted to add a search feature for your customers. Public website search enables you to: Integrate Enterprise Search into your current website, Find products, articles or services from a Natural Language search, Customize the appearance of the search results, And, get recommendations for similar content. Here is an example of an External Customer facing Food enthusiast website, that has integrated an Enterprise Search feature using Generative AI App Builder. It contains everything a customer expects from a Generative AI Search engine, and more! Including Natural Language processing, which means it's really good at understanding and generating human language. The customer can enter a conversational Natural Language prompt into the search bar. They receive an immediate conversational response that makes it feel like they are talking to another person. And it doesn’t stop there… The customer can continue their search query with more questions, including: Multimodal input - by uploading images, documents, maps, audio, and much more, to form part of another prompt. And receive multimodal output as part of the response, in this case an image of the restaurant, but this could also include some customer reviews, the restaurant menu, a link to the restaurants booking service, or any other information a customer may want. And along with the personalized responses to your customers' prompts, they will also receive personalized search results and recommendations tailored to your expectations. Generative AI App Builder and Enterprise Search can enable you to build and customize, personalized self-serve customer experiences, with a state-of-the-art recommendation engine on your own data that can suggest content similar to the content that the user is currently viewing.

### Quiz - [Enterprise Search Use Cases Quiz](https://www.cloudskillsboost.google/course_templates/612/quizzes/412260)

#### Quiz 1.

> [!important]
> **Why do business analysts choose Generative AI technologies like Enterprise Search?**
>
> - [ ] When coding, they want to reduce time from looking for code snippets online and copy-pasting them into their project.
> - [ ] Customize large models and incorporate state of the art generative capabilities natively into their own internal ML operational platforms
> - [ ] Improve time-to-value to search, navigate, and extract insights and understanding from large amounts of complex data
> - [ ] Build rich apps and automated processes without writing a line of code.

#### Quiz 2.

> [!important]
> **In which of the following scenarios should you use Enterprise Search? (Choose two).**
>
> - [ ] Quickly search and summarize your company's annual compliance training videos and create study guides.
> - [ ] You have machine learning expertise and want to tune and deploy foundation models directly into your applications.
> - [ ] Improve existing search result experiences with LLM-based capabilities such as summarizing results.
> - [ ] Improve developer productivity using code completion and code generation features.
> - [ ] You lack the time to build a custom search system that is scalable and available.

#### Quiz 3.

> [!important]
> **Choose the use case that cannot be satisfied with Enterprise Search**
>
> - [ ] Public website search for end customers to better find answers stored in the different web pages such as company blogs and FAQs.
> - [ ] Build custom search engines without machine learning expertise.
> - [ ] Internal company search for employees to find relevant private information.
> - [ ] Code search, where developers can paste a bug and Enterprise Search finds the piece of code that caused the issue.

## Generative AI App Builder Architecture and Security

Generative AI App Builder architecture, authentication to Gen App Builder apps, access control with Identity and Access Management (IAM), data governance and compliance, and pricing.

### Video - [Generative AI App Builder architecture](https://www.cloudskillsboost.google/course_templates/612/video/412261)

- [YouTube: Generative AI App Builder architecture](https://www.youtube.com/watch?v=ehyol1ff9XQ)

Welcome back to the course Enterprise Search on Generative AI App Builder. This is the Generative AI architecture and security module. In this module, you'll explore the Generative AI App Builder architecture, Authentication to Gen App Builder apps, Access control with IAM, and Data governance and compliance In this module, you'll explore the Generative AI App Builder architecture, Authentication to Gen App Builder apps, Access control with IAM, Data governance and compliance, Enterprise Search pricing, and General guidance on competitive situations. Let’s start by exploring the Generative AI App Builder architecture. Gen App Builder provides the same security controls as many other Google Cloud Perimeter products, such as BigQuery. Customer data is always stored with encryption… using Customer Managed Encryption Keys when provided. Also, in the very unlikely event that a member of the Google operations team must access customer data, know that all such access is logged and is traceable by using Access Transparency. Data residency and VPC Security Controls continue to be respected. When considering the security controls of the LLMs specifically, it's important to be aware that: LLMs are stateless, meaning the weights are frozen and cannot be reconfigured. They do NOT use customer data to improve the model. And, they do NOT store customer data, including customer-specific parameters. You can also use alternative cloud data with our LLMs, but the customer will need to process the data into the json format that they need on the alternative cloud, before moving it over to Cloud Storage. Additionally, it's important to remember that: Data in flight is always encrypted. And your data is not used to benefit another Customer. Gen App Builder provides the security expected from Google Cloud Perimeter to enable the best of AI. So, whether you're deploying a large language model or running a batch prediction job on structured data, Google Cloud's entire stack is optimized for AI workloads in three main ways: First, is scale and speed: Google’s AI infrastructure makes it fast and cost-effective for organizations to scale their end-to-end machine learning workloads - from data preparation and model training, to feature engineering and deployment. Second, is price-performance and efficiency: Google is a leader in hardware, optimized for running large models, and has created the Tensor Processing Unit, or TPU, which is a highly specialized processing unit for training large models. With Google Cloud, you can choose from GPUs through the partnership with Nvidia, Google’s own TPUs, or CPUs to support a variety of use cases including high performance training, low cost inferencing, and large scale data processing. Third, is sustainability: It’s important to have a low carbon footprint when training your models – and Google’s TPU infrastructure runs on 90% clean energy and is the most sustainable cloud option for enterprise customers.

### Video - [Authentication to Gen App Builder apps](https://www.cloudskillsboost.google/course_templates/612/video/412262)

- [YouTube: Authentication to Gen App Builder apps](https://www.youtube.com/watch?v=zS0Vqf8K_H8)

In this lesson you'll learn how you gain programmatic access to Generative AI App Builder, and authenticate your application. Gen App Builder Client Libraries are available for many of the most popular programming languages. Supported languages include: Python, Node.js, Java, Go, PHP, Ruby, and the . NET languages, including C#. [pause] If your application uses any of these languages, check out the corresponding Gen App Builder Client Library. Now, let’s examine an example of using the Python Gen App Builder Client Library to perform a search in an App Builder Search Engine. First, you import the package for the Google Cloud Client Library for App Builder. Next, create a client connection to the Search Engine, and configure the client. This must include the full resource name of the search engine serving config. Once the client has been configured, you're ready to perform a search and send the results back. The Gen App Builder Client Libraries let you easily manage your Gen App Builder resources by using the natural style of the programming language you've chosen. You can use a service account to authenticate your application, to do this you will need to: First, create the service account by using the Google Cloud console. You then generate and download your credentials file, Next, you can set an environment variable with the path to your downloaded credentials. The example shows commands to set the environment variable in both Linux or OS X and Windows. Finally, you can make an authenticated API request in your code. The example code is in Python and shows that if you don’t explicitly specify credentials when constructing a client, the client library will look for credentials in the environment.

### Video - [Access control with IAM](https://www.cloudskillsboost.google/course_templates/612/video/412263)

- [YouTube: Access control with IAM](https://www.youtube.com/watch?v=0sJ5VOrpaeg)

In this lesson you'll explore the types of access control with Identity and Access Management or IAM. it's extremely important to grant the right level of access and permissions to the right people when it comes to your Gen App builder resources. To do this you'll need to understand the levels of access that are available within IAM and the types of roles and responsibilities they might apply to. IAM provides three main levels of access for Gen App Builder: Discovery Engine Viewer, Discovery Engine Editor, And Discovery Engine Admin. These predefined IAM roles can be used to provide granular access to Gen App Builder resources. The Discovery Engine Viewer role provides read-only access to all Gen App Builder resources. For example, you might assign this role to auditors of the infrastructure. The Discovery Engine Editor role can read all Gen App Builder resources and write products, events, and other resources. This role is used for importing, updating and deleting documents in the search engine, creating, updating and tuning the model, as well as creating user events and updating widgets. The Discovery Engine Admin role has full control over all Gen App Builder resources. Those permissions include the management of data stores, controls, serving configurations and target sites.

### Video - [Data governance and compliance](https://www.cloudskillsboost.google/course_templates/612/video/412264)

- [YouTube: Data governance and compliance](https://www.youtube.com/watch?v=df_ITT95X2w)

In this lesson you'll learn more about data governance and compliance with Google Cloud. Google Cloud products empower enterprises to embrace Generative AI with the confidence that there is Data Governance built-in. This is especially important in highly regulated industries like financial services and healthcare where you need to guarantee that no one can access confidential or sensitive data. You also want to be certain that none of your data or your customers data is being used for any other purpose than determined by you. So, let’s outline Google Cloud’s approach to governance of customer data for Cloud LLMs and Generative AI. Google Cloud is always committed to transparency, compliance with regulations like GDPR and HIPAA, and privacy best practices. By default, Google Cloud does not use customer data to train LLMs, in accordance with the Google Cloud Terms and the Cloud Data Processing Addendum. And, Google Cloud will obtain customer permission before using any customer data to train LLMs.

### Video - [Enterprise Search pricing](https://www.cloudskillsboost.google/course_templates/612/video/412265)

- [YouTube: Enterprise Search pricing](https://www.youtube.com/watch?v=m7KfwWGIsDE)

In this lesson you'll explore some of the Generative AI App Builder and Enterprise Search pricing components. Google Cloud has set the pricing structure for these components as follows: There will be a cost associated with indexing and storing customer data. This index is shared across Enterprise Search and Conversational AI, so you won’t have to pay twice if you're using both products. The Search Service charges by the number of Queries, rather than Tokens. This is different from Vertex AI pricing, since Generative AI App Builder aims to provide an easier user experience. And, Search Queries are priced based on the number of inputs. More complex queries will cost more to run than simpler queries.

### Quiz - [Generative AI App Builder Architecture and Security Quiz](https://www.cloudskillsboost.google/course_templates/612/quizzes/412266)

#### Quiz 1.

> [!important]
> **The development team is creating a microservice that will be responsible for ingesting new documents into the Gen App Builder unstructured data store on bulk every hour. Which role should you assign them?**
>
> - [ ] Discovery Engine Admin
> - [ ] Discovery Engine Editor
> - [ ] Discovery Engine User
> - [ ] Discovery Engine Viewer

#### Quiz 2.

> [!important]
> **Choose the answer that best describes the security posture of Gen App Builder.**
>
> - [ ] Gen App Builder uses the latest GPU technology to encrypt your custom models.
> - [ ] Gen App Builder does not store any customer data, making all interactions secure and private.
> - [ ] Gen App Builder offers the same security capabilities as other Google Cloud products like BigQuery, including data encryption in flight and disk and no data sharing across customers
> - [ ] Gen App Builder encrypts data at rest, but does not encrypt data in transit.

#### Quiz 3.

> [!important]
> **The website team is creating a microservice that will be responsible for creating controls and serving configs to filter out what data is presented to users after they perform a query. Which role should you assign them?**
>
> - [ ] Discovery Engine Viewer
> - [ ] Discovery Engine Super User
> - [ ] Discovery Engine Admin
> - [ ] Discovery Engine Editor

#### Quiz 4.

> [!important]
> **The security team needs to perform some audit tasks to your datastores on Gen App Builder to make sure the right documents and user events are being ingested. Which role should you assign them?**
>
> - [ ] Discovery Engine Admin
> - [ ] Discovery Engine Viewer
> - [ ] Discovery Engine View-Only
> - [ ] Discovery Engine Editor

## Managing data in Generative AI App Builder

This module is about creating a search engine, ingesting data into a search engine, and managing data in a search engine

### Video - [Creating a Search Engine](https://www.cloudskillsboost.google/course_templates/612/video/412267)

- [YouTube: Creating a Search Engine](https://www.youtube.com/watch?v=TAijdShCatk)

Welcome back to the course Enterprise Search on Generative AI App Builder. This is the Managing data in Generative AI App Builder module. In this module, you'll explore creating a search engine, ingesting data into a search engine, and managing data in a search engine. Let’s start by outlining how to create a search engine. One of the greatest features of Gen App Builder is its ease of use for developers. You can index and search a publicly-accessible website, And you can create a search engine based on certain data types: Such as structured data that is organized in a specific format and follows a schema, such as BigQuery, JSON, a provider directory, and product catalogs, Or you can use unstructured data. Which is data that doesn't follow a schema. It may be stored in the form of HTML, PDFs with embedded text, plain text files, slides, or documents. Let's go through the process of setting up a basic search engine for the supported data types. First, choose the type of data that you want to import, whether it is website data, structured, or unstructured data. Any data needs to reside in BigQuery or Cloud Storage, or it needs to be a publicly accessible website. Second, prepare the data to be ingested. Data located in Cloud Storage can be either Structured or unstructured. Structured data must be in either NDJSON or JSON Lines format. Unstructured data can be ingested automatically, or you can add metadata. The metadata can be stored in a file in Cloud Storage, or as a table in BigQuery. The goal of the meta is to describe the contents of the data and therefore get better search results. Data located in BigQuery is structured and can be imported into your search engine without any further modifications. For public websites, Gen App Builder utilizes the existing indexed information for Google Search, so you'll notice that an engine built on external sites is immediately searchable. Third, when importing structured data, you can choose to auto-detect the schema, provide a custom schema, or a combination of both options. Auto-detecting a schema is the recommended method for your first engine because it’s the most straightforward. However, it will provide the worst quality results. To improve your search results you can choose to edit the schema once it’s been auto-detected. However, your data will have to be reindexed, which will take a long time. To speed up the process, you can ingest a small but representative subset of your data, review the schema suggested by auto-detect, provide any edits required, and then ingest the rest of your data. Finally, providing the schema as a JSON object is the fastest and most efficient option. The downside of this approach is that you have to create the JSON schema file manually without Cloud Console support. If you choose to provide a JSON schema file or edit the auto-detected schema, you should focus on the following fields. The keyPropertyMapping maps predefined keywords to critical fields in your documents, helping to clarify their semantic meaning. For example, you have the Title, Description, URI and Category. All properties have a primitive type, which can be boolean, object, array, number, string, or an integer. Additionally, fields have options that define the accessibility of using the search engine. Indexable defines whether a field can be filtered, faceted, boosted, or sorted in the servingConfigs.search method. You will explore those options in more detail in an upcoming module of this course. Searchable defines whether a field can be reverse indexed to match unstructured text queries, which can provide more accurate search results if the field is relevant. Retrievable indicates whether a field can be returned in a search response. Dynamic Facetable defines whether it can be used to present information organized in section headers. And finally, Completable indicates whether the field can be directly used as suggestions. Fields in auto-detected schemas are indexable, searchable, and retrievable by default, as long as they follow the type requirements and stay within the maximum limits. Here’s an example of an auto-detected schema in the Gen App Builder Console. Finally, import data as documents into a data store. At the time of this recording, an "engine" can only contain a data store that has search enabled. When you "create an engine" using the Google Cloud console, you are actually creating and naming a data store. Gen App Builder automatically enables the data store for search.

### Video - [Ingesting data into a Search Engine](https://www.cloudskillsboost.google/course_templates/612/video/412268)

- [YouTube: Ingesting data into a Search Engine](https://www.youtube.com/watch?v=RFO-n3j2lqw)

In this lesson you'll learn how to ingest data into a search engine. The process to ingest website data into a Search Engine is currently only available by using the Google Cloud Console. You can enter the URLs of the websites to include in your search engine. Feel free to include any websites you want, not just the sites that you own. You can also exclude any websites that you don’t want to be searched. At the moment, only public websites can be ingested. For private sites, create an unstructured Search Engine and upload the websites’ HTML files. You can use the Google Cloud console or code to create an engine and ingest structured or unstructured data from a Cloud Storage bucket or BigQuery. Here is an example written in Python about how to import documents both from Cloud Storage, and BigQuery. Notice that you can do either a full or incremental import of the data on both Cloud Storage and BigQuery. A Full import is a replacement of the data in the data store. And an Incremental import is adding additional data. It’s important to be aware that there are some limitations in the enterprise Search Engines. In terms of support, Website Search only supports public websites. For unstructured search, we can import at most 100,000 files each time with a maximum of 40MM and a single file size cannot exceed 100MB For structured search, we can import at most 100 files each time, and a single file size cannot exceed 2GB. The ingestion throughput is 200 rows per second. So for 1 million rows it would take around 1.4 hours. User events can help you improve your output. Sending user events can help improve the quality of your recommendations as well as the ranking of your search results. Search results with higher click-through rates are boosted, while results with lower click-through rates are buried. You can send real-time events using the API or using a Javascript pixel. Additionally, you can import historical events from Cloud Storage, BigQuery or Inline. You can record real-time user events using the App Builder SDKs or Javascript pixel. This example shows you a Python code snippet that performs the recording. As you see, there are a few straightforward instructions to import the App Builder libraries, create a client, initialize the request and make the request to the Search Engine backend. You can also import user event data from past events in bulk, this can help improve the quality of your recommendations as well as the ranking of your search results. This example shows you how to import historical user events using the Discovery Engine API.

### Video - [Managing data in a Search Engine](https://www.cloudskillsboost.google/course_templates/612/video/412269)

- [YouTube: Managing data in a Search Engine](https://www.youtube.com/watch?v=3gco8HwrwXM)

In this lesson you'll learn how to manage data in a search engine. These are the stages in the lifecycle of a Search Engine. First of all you start by creating an engine. Depending on the type of engine you choose, you might start by creating a schema for data to be processed correctly when it’s imported, or you might choose to import the data and optionally update the schema afterwards. Furthermore, you can always refresh data, by either adding incremental data or redoing an import of data. In case you changed the origin of the data, you might have to delete the existing data before doing a new import. Finally, deleting an existing schema or a full data store will require you to delete the data first. Here’s a python example that shows how to update your schema. There are some requirements and limitations when updating schemas. The new schema should be backward compatible with the schema you are updating. Non backward compatible schemas need to be deleted and recreated. And some updates are not supported including: Changing a field type. For example, a field mapped to an integer cannot be changed to string. And, removing a field. You can continue adding new fields but you cannot remove an existing field. Here’s an example in Python showing how to purge documents. The same is also available from the UI. You can purge a data store when you want to completely delete its contents and re-ingest fresh data. Purging deletes only the documents from the data store. However, it leaves your engine, schema, and configurations intact. And you can purge data from a structured data store or an unstructured data store. There is no option to purge data from a website data store.

### Link - [Vertex AI Search onboarding walkthrough](https://www.cloudskillsboost.google/course_templates/612/documents/412270)

- [Vertex AI Search onboarding walkthrough](https://www.youtube.com/watch?v=fY8aOe6H2nw)

### Quiz - [Managing data in Generative AI App Builder Quiz](https://www.cloudskillsboost.google/course_templates/612/quizzes/412271)

#### Quiz 1.

> [!important]
> **What data stores can have a schema?**
>
> - [ ] Only data stored in a comma-separated values file can have a schema.
> - [ ] Unstructured data - until you don't have a schema you cannot perform a search.
> - [ ] All data stores require a schema, but it can be auto-detected from the data structure
> - [ ] Structured data

#### Quiz 2.

> [!important]
> **What data stores are available in an Enterprise Search engine?**
>
> - [ ] Document, Table, and Image data stores.
> - [ ] Customer facing and internal search data stores.
> - [ ] SQL, No-SQL and Data Warehouse data stores.
> - [ ] Website, structured and unstructured data stores.

#### Quiz 3.

> [!important]
> **What can be deleted in Enterprise Search? Select all that apply.**
>
> - [ ] Schemas can be deleted.
> - [ ] Data stores can be deleted.
> - [ ] All of the above are correct.
> - [ ] Data inside a data store can be deleted.

#### Quiz 4.

> [!important]
> **How can you improve the quality of recommendations and search results leveraging user actions? Select all that apply.**
>
> - [ ] Sending real-time events using API or the JavaScript pixel on user actions such as click events.
> - [ ] All of the above are correct.
> - [ ] Import historical user events
> - [ ] Providing feedback on search results.

## Displaying Enterprise Search Results

Configure search results from websites, unstructured and structured data, as well as common search configurations and integrating search in your applications.

### Video - [Configuring search results from websites](https://www.cloudskillsboost.google/course_templates/612/video/412272)

- [YouTube: Configuring search results from websites](https://www.youtube.com/watch?v=lO2GFkoqa-c)

Welcome back to the course Enterprise Search on Generative AI App Builder. This is the Displaying Enterprise Search results module. In this module, you'll explore how to configure search results from websites, unstructured data, and structured data, common search configurations, and integrating search into your applications. Let’s begin by exploring how to configure search results from websites. In Generative AI App Builder you have some general configuration settings that can be applied to the search results in a website search engine widget. These settings are for enabling or disabling different features, such as, Autocomplete, which suggests letters and words for your search queries based on previous queries and data stored in your search engine, Feedback, which allows users to send feedback about search results, and safe search - which helps you manage explicit content in your search results, like sexual activity and graphic violence. This is a preview of the output Generative AI App Builder in the Google Cloud Console when performing a search query to a website engine. Adding a widget to your website will look very similar to this output. Enterprise Search can search for images on your website using the advanced site search functionality. At the time of this recording, advanced site search could only be enabled and used through APIs and SDKs. Before searching for images the first time using your website search engine, make sure you enable advanced site search and wait for indexing to complete. Enabling advanced site search is a long-running operation. Depending on how much data you have, indexing for advanced site search can take minutes or hours. To enable advanced site search, run the following call. To search for images on your website, specify the default_config.search method in the serving configurations object and then supply a text string query.

### Video - [Configuring search results from unstructured data](https://www.cloudskillsboost.google/course_templates/612/video/412273)

- [YouTube: Configuring search results from unstructured data](https://www.youtube.com/watch?v=V2IR4vO3XQY)

In this lesson you'll learn how to configure search results from unstructured data. There are two ways of showing information obtained from unstructured search results. The first is summarizations, and the second is snippets. Let's explore the first one. The top five results are summarized by default, but you can always customize this number if you choose to. A snippet is a short section of text, typically a sentence, under the document title. You can customize the display and contents of the snippet. By default, 1 snippet is displayed for each search result. In Generative AI App Builder you have some general configuration settings that can be applied to the search results in an unstructured search engine widget. You can enable or disable the Summarization, and specify the number of top results used to generate the search result summary. You can also enable or disable snippets, and specify the number of snippets to show for each result. The autocomplete, feedback, and safe search features can also be enabled or disabled. Additionally, you can configure Facets. Facets are organizational headers used to group relevant information together, so that you can navigate quickly to the section that you want in the data. Identify a Field in the document, and provide a Display Name that becomes the header for that field in the Facets list. You can perform a multi-turn, conversational-style search on an unstructured data search engine. Let's explore what supported features are available. The first is Natural Language query processing. First, submit a question using conversational language. The search engine then processes the question, identifies the intent behind a query, and returns the relevant results. The next supported feature is Context Awareness. This means that the engine remembers prior interactions, and provides context-aware answers. The final feature is Multi-turn, which allows users to ask follow-up questions and receive relevant responses. For example, suppose that you want to know about vacationing in Mexico: You ask a question using natural conversational language like: “When is the best time of the year to vacation in Mexico?” And you receive a relevant response in Natural Language. You then ask a second question like “What is the exchange rate?”. Notice here that you have not provided a context for your question. The multi-turn search engine has remembered the context and intent of your previous questioning and provides an answer that is consistent with your query. What makes this feature great is that you can ask multiple follow-up questions in a conversational way, as if you were talking with another person. You’ll continue to receive relevant and context-aware responses. To use a multi-turn, conversational-style of search on an unstructured data search engine, create a conversations store for a specific user. You can have multiple conversations per user. This command generates a unique conversation id, which you will use to perform conversational search queries on your engine. The user pseudo ID tracks and uniquely identifies a visitor on a single device. This can be implemented as an HTTP cookie. Use the generated conversation ID when you hit the converse endpoint to initiate or continue a conversation. Use the query parameter to supply the text string for your query. You can also view all the details about a specific conversation. List all conversations, with the option to add filters to look for conversations for a specific user or a given state. States can either be “in progress” or “completed”, and you can update the state of a conversation. Existing conversations from a data store can also be deleted.

### Video - [Configuring search results from structured data](https://www.cloudskillsboost.google/course_templates/612/video/412274)

- [YouTube: Configuring search results from structured data](https://www.youtube.com/watch?v=_DPCZw5-5WM)

In this lesson you'll learn how to configure search results from structured data. Here are the results from a structured data search. This example shows the search results from a popular mainstream film. Notice that the data was saved in a structured format, so it has a predefined schema. In this example, all fields of the schema are displayed. It's important to note that you can configure the fields of the schema, so that you only show a subset of those in your search results for the structured data. Let's analyze the fields that are specified in this example. The title of the search result is mapped with a field schema named title. Thumbnail - The URL of an image to be shown next to the item title in a search result. In the Thumbnail field, the image corresponding to the URL is shown next to the item title in a search result. And URL field adds a link to the URL the user is taken to when they click the item's title. You can include additional fields in your results from the schema values, which you previously defined as key-value pairs.

### Video - [Common search configurations](https://www.cloudskillsboost.google/course_templates/612/video/412275)

- [YouTube: Common search configurations](https://www.youtube.com/watch?v=LoPKjhh2_Ks)

In this lesson you'll learn about some common search configurations. You can use serving controls to change the default behavior of a search request. There are two types of controls: Boost controls, which can apply filters to the content to promote or demote the search results. And filter controls, which specify the requirements met by the document in order to be included in the response. To change the results of a request, first create a control, and then attach it to a serving config. A control only affects search requests served by serving configs that the control is attached to. If a control isn't attached to any serving config, it has no effect. For example, to use a boost control, start by using the APIs to create such control. Then, attach the boost control to a serving config, so that all search queries performed towards the serving config can benefit from these additional controls. You can also add queryTerms and an activeTimeRange to a control: Use queryTerms if you want a control to be used when specific queries are searched for. And use activeTimeRange to decide the start and end time when the control will be applied. Another useful feature is to add autocomplete to your search queries. For structured and unstructured search engines, suggestions are based on the content of the documents in the store. After document import, autocomplete takes a day or two to start generating suggestions. If you make autocomplete requests through the API, autocomplete can generate suggestions that are based on the search history or user events. For the Website search engine, by default, autocomplete generates suggestions from the search history. Autocomplete requires real search traffic. After search traffic begins, autocomplete takes a day or two before generating suggestions. The autocomplete data model determines what type of data autocomplete uses to generate suggestions. There are four autocomplete models: The document model generates suggestions from user-imported documents. This model isn't available for website search engines. The completable fields model suggests text taken directly from structured data fields. Only those fields that are annotated with completable are used for autocomplete suggestions. This model is only available for structured data engines. The search history model generates suggestions from the history of SearchService.search API calls. Do not use this model if there is no traffic available for the servingConfigs.search method. And, the user event model generates suggestions from user-imported search events. Autocomplete requests are sent using the dataStores.completeQuery method. Here’s an example of an autocomplete search query. Notice, the use of the dataStores.completeQuery method. If you set the include tail suggestions parameter to true, you will get completions of the last word. For instance, if you say “Songs with he”, the tail suggestions will suggest options like “hello world” and “hello kitty”. Finally you can specify a different autocomplete model to use for your request. You can choose between: document, document-completable, search-history, or user-event.

### Video - [Integrating search into your applications](https://www.cloudskillsboost.google/course_templates/612/video/412276)

- [YouTube: Integrating search into your applications](https://www.youtube.com/watch?v=08heFDp_WAQ)

In this lesson you'll learn how to integrate search into your applications. There are two main approaches to integrating search in your applications: You can copy and paste a widget in an existing website, this method has a low coding requirement. Or you can integrate your application with Enterprise Search using the APIs and SDKs, however this method requires coding. Let’s start with the Widget integration. There are two options for authorizing your Widget to connect to Enterprise search: For User authorization, you can use a JWT or an OAuth token. And for Public access, there are no restrictions on who can get results from a search query. You can also limit the domains that can use the Widget so that only your websites can perform search queries on Enterprise Search using your data. Let’s cover how to copy the snippet into your web page. The code snippet, in HTML, starts with the Gen App Builder widget bundle. The second element is defining the search widget with a configId and a triggerId. The configId is instantiated with a placeholder, and this will auto-populate with the correct configId in the Google Cloud Console. The triggerId is configured to the searchWidgetTrigger. The third element adds a "Search here" link that users can click to open the widget. In this case it is an input but it does not have to be. The search widget element is not visible by default, but the reCAPTCHA badge is displayed by default, which can be removed. This second snippet, is only needed when using OAuth or JWT for user authorization, a public access widget does not require it. This JavaScript snippet generates an authToken and passes it to the widget. The actual JWT or OAuth token is provided by your backend. The Generative AI App Builder search widget includes feedback buttons that help Google assess search quality issues. You can turn this feature on using the Google Cloud console. When the feedback feature is turned on, the widget displays Thumbs up and Thumbs down buttons. Users can click the buttons to indicate whether the quality of the results appeared as expected. If a user clicks the Thumbs down button, they are prompted to select from a list of reasons why the quality is not as expected and to provide additional comments. Now, let’s explore how to integrate your application using APIs. As an alternative to creating a widget to add to an HTML page, you can make API calls and integrate those into your server or applications. Here is how to make the API call from the shell. And the results are returned to your search engine in JSON format.

### Quiz - [Displaying Enterprise Search Results Quiz](https://www.cloudskillsboost.google/course_templates/612/quizzes/412277)

#### Quiz 1.

> [!important]
> **What kind of data can you search with a Website Engine?**
>
> - [ ] Images and public websites.
> - [ ] Private and public websites.
> - [ ] Images and private websites.
> - [ ] Images, private websites and public websites.

#### Quiz 2.

> [!important]
> **What do you use in unstructured search to divide or categorize information?**
>
> - [ ] Corpus
> - [ ] Facets
> - [ ] Snippets
> - [ ] Summarization

#### Quiz 3.

> [!important]
> **How do you change the default behavior of a search request?**
>
> - [ ] Facets change the order of results and boost removes entries from those results.
> - [ ] Facets change the order of results and filters remove entries from those results.
> - [ ] Boost controls change the order of results and facets remove entries from those results.
> - [ ] Boost controls change the order of results and filters remove entries from those results.

#### Quiz 4.

> [!important]
> **What do you use in unstructured search to divide or categorize information?**
>
> - [ ] Corpus
> - [ ] Summarization
> - [ ] Facets
> - [ ] Snippets

## Enterprise Search Analytics

This module reviews product usage through analytics and metrics.

### Video - [Enterprise Search Analytics](https://www.cloudskillsboost.google/course_templates/612/video/412278)

- [YouTube: Enterprise Search Analytics](https://www.youtube.com/watch?v=YEA_Yq0q3Rs)

Welcome back to the course Enterprise Search on Generative AI App Builder. This is the Enterprise Search Analytics module. Analytics gives you insight into the usage trends, search quality, and end-user engagement of your search engine. Gen App Builder provides an interactive dashboard experience powered by Looker. This is a fully customizable dashboard that provides filters so that you can refine your search, such as Date Range for a specific timeframe or date range in all the metrics and charts, Search Query for a specific query of interest, and Contains for key words across the dataset. Analytics come from several data sources. First, you have search logs, which are based on search requests and can include session analytics if the user pseudo IDE is included in search queries. Second, you have user events which automatically collected when using a widget, and can be programmatically added when using the APIs and SDKs. Search events might contain the user agent, so that you can filter your analytics based on the device type performing the search. Also, you can add Attribution tokens - unique IDs generated by Enterprise Search that allow you to link search results with actions performed afterwards. You also have view-item events, which allow you to see impressions, that is, item views or clicks performed on the results from a search. Specifically, you will have access to the following metrics: Search count is the number of searches performed, which tells you how much search is being used. No results rate is the count of search events without results divided by the total search count. If this number is very low, you might want to change some of the filters or boost conditions you configured. Click-through rate or CTR per search means the number of clicks per search count, which tells you whether users are finding what they were looking for. Search session count gives you an idea of how many users and how often they interacted with Enterprise Search. Page view per search visit gives you an idea of the usefulness of the results. And Bounce rate indicates how often users found answers using Enterprise Search.

### Quiz - [Enterprise Search Analytics Quiz](https://www.cloudskillsboost.google/course_templates/612/quizzes/412279)

#### Quiz 1.

> [!important]
> **Which metric indicates whether your users are finding what they were looking for?**
>
> - [ ] Search count
> - [ ] Click-through rate
> - [ ] Search session count
> - [ ] No results rate

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
