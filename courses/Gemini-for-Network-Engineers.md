---
id: 884
name: 'Gemini for Network Engineers'
datePublished: 2024-05-14
topics:
- Gemini
- Networking
- VPC
type: Course
url: https://www.cloudskillsboost.google/course_templates/884
---

# [Gemini for Network Engineers](https://www.cloudskillsboost.google/course_templates/884)

**Description:**

In this course, you learn how Gemini, a generative AI-powered collaborator from Google Cloud, helps network engineers create, update, and maintain VPC networks. You learn how to prompt Gemini to provide specific guidance for your networking tasks, beyond what you would receive from a search engine. Using a hands-on lab, you experience how Gemini makes it easier for you to work with Google Cloud VPC networks.

Duet AI was renamed to Gemini, our next-generation model.

**Objectives:**

- Enable Gemini.
- Use Gemini to get information needed to plan, implement, and maintain a Google Cloud VPC network.

## Gemini for Network Engineers

Learn how to create and maintain a VPC networlk with with help from Gemini.


### Video - [Introducing Gemini for network engineers](https://www.cloudskillsboost.google/course_templates/884/video/476761)

- [YouTube: Introducing Gemini for network engineers](https://www.youtube.com/watch?v=_DY7YDZInPM)

[MUSIC] This is a network engineer. In this video we see how they use Gemini to get help to create a custom VPC network. They have on premises experience and are new to setting up networking in Google Cloud. They must explore and understand how to create a network with dual stack subnets in their organization's environment. They need to get a better understanding of how networking works in Google Cloud and are hoping to use Gemini to help them create a custom VPC with dual stack subnets. Let's observe this network engineer as they use Gemini to simplify the task at hand. First things first, they want to know how to set up a virtual private cloud or VPC network in Google Cloud. They go to Google search, look for VPC network on Google Cloud, scroll through documentation, watch a video and read a bit more and they aren't sure on how best to proceed and decide to take a quick coffee break to clear their head. After explaining their situation to a co-worker, they recommend a potential solution. Try Gemini. It's an AI companion that saves time, especially in these situations. Thanks helpful co-worker. Let's open Gemini and learn how it can help speed things along. They prompt Gemini to help them understand how to create a VPC network in Google Cloud. Gemini responds, and the network engineer is amazed. They recall that they want to ensure that the subnet created here is dual stack. So to achieve this, they ask Gemini to adjust the gcloud CLI command. They are happy and excited that Gemini responded with that modification for dual stack. Now, they are ready to proceed with setting up this VPC and making it a reality. They use the gcloud CLI command Gemini provided, and then create the dual stack subnet in that VPC by using the gcloud CLI command Gemini provided. They are amazed and thrilled that their VPC and subnets are created. Now that the VPC is set up, our network engineer is interested in learning more about connecting Google Cloud to their on premises network because they have applications running on premises that they want to connect to the ones running in Google Cloud. For this, they need to have some sort of private connectivity between their on premises network and Google Cloud, so they decide to use Gemini to assist them with understanding the options available to them. Gemini responds with instructions on how to connect a VPC in Google Cloud to an on-premises private network. Although it's helpful to know that they can use cloud vpn tunnels or vlan attachments with cloud interconnect, they want to get a more detailed comparison to help them make a decision. So they prompt Gemini which they should use, and ask to provide details supporting the use of each according to their respective strengths. Geminis response includes a helpful comparison visual along with more context and additional factors to consider when making their decision. Gemini is amazing. This is now their new exploration and learning tool. They decide to keep going with this. Now, they want to use Gemini to explore DNS in Google Cloud. They prompt Gemini to help them understand networking in Google Cloud and ask, how does DNS work in Google Cloud? Gemini responds and the network engineer is pleased to get all this information in context without having to context switch and leave the google cloud console because they know they already have primary private DNS resolution on premises. They want to use Gemini to help them understand if this is possible to integrate with Google Cloud DNS. So they prompt Gemini with a question asking how DNS forwarding works between Google Cloud DNS and potential on premises private DNS servers. Gemini responds with context and advice on how to go about configuring DNS forwarding. From this response, they gather that forwarding zones in Google Cloud DNS provides the functionality they need, and they can follow up by clicking the show related content button in which official documentation is linked for them to learn more about configuring forwarding zones. But why stop their quest for knowledge there? The network engineer wants to understand ip addressing in Google Cloud, so they ask Gemini once again. Wonderful. This information provides useful context for our network engineer because their team requires both ipv four and ipv six support. They also want to understand if they can run a dual stack subnet in Google Cloud. So they prompt Gemini with the question. Gemini responds with some helpful info, yes you can, and provides a link to the docs with more info. And with all that time saved, they can now finally get around to exploring science. Thanks, Gemini. What will you build? [MUSIC]

### Lab - [Creating a VPC Network with Gemini](https://www.cloudskillsboost.google/course_templates/884/labs/476762)

In this lab, you configure VPC Network Peering between two networks. Then, you verify private communication between two VMs in those networks.

- [ ] [Creating a VPC Network with Gemini](../labs/Creating-a-VPC-Network-with-Gemini.md)

### Video - [Designing an enterprise network with Gemini](https://www.cloudskillsboost.google/course_templates/884/video/476763)

- [YouTube: Designing an enterprise network with Gemini](https://www.youtube.com/watch?v=yHixSs8v1nY)

[MUSIC] I'm an IT networking engineer with on-prem experience, and my company has recently joined Google Cloud. I need to create and modify a virtual private cloud, or VPC, with dual stack subnets in my company's new cloud environment. So that we can continue to run our business smoothly with a hybrid cloud approach. I'm fairly new to the cloud in general, but I've been told that Gemini can help me create this VPC using gcloud, the command line tool for Google Cloud, without needing much previous cloud knowledge. To start, I'll ask Gemini some questions to get a better understanding of how things work in Google Cloud. To prompt Gemini, I can click the Gemini button at the top right corner of the console to open up the chat and write my prompt directly here in natural language. I know that I already have a primary private domain name system, or DNS resolution, on-prem. But I want to know if it's possible to integrate it with Google Cloud DNS. So I'll ask Gemini how DNS forwarding works between Google Cloud and on-premises servers. Cool, it's telling me that Google Cloud DNS can forward queries to on-premises DNS servers, and vice versa. So my on-premises DNS servers can forward to Google Cloud DNS, which is what I need. My next question is about the dual stack subnet requirement. I imagine I can use IPv four and IPv six subnets in Google Cloud, but I want to double check before I move forward again. I'll ask Gemini if I can use both IPv4 and IPv6 subnets in Google Cloud. And yep, it tells me that I can use both. And a VPC network can contain any combination of these subnet types. Now that I have my questions answered, let's get into actually creating this VPC. I know I want to use gcloud to create the VPC, so I'll give Gemini that context in my prompt. So how can I use gCloud to create my first VPC network in Google Cloud? Gemini gives me a response with the steps that I need to take. It gives me the initial command to create the VPC, and then a follow up command to create a subnet in the VPC network. This is a good start, and they seem like pretty easy steps, but I just realized that I didn't specify that I want dual stack subnets. So instead of retyping my prompt with that edit, I'm going to ask a follow up question about adjusting the command that was just provided. So let's say, like, how can I adjust the gcloud command provided to create a subnet to ensure that it's dual stack? Gemini gives me a response and I can see here that the stack type flag specifies that the subnet should be dual stack. This is helpful because Gemini was able to use the context from the previous interaction to follow up, which saves me time. Now that I know how to make my subnet dual stack, I can start with the commands provided to create my network. So first, I'll open up the gcloud CLI by clicking this button on the Cloud Console toolbar. [MUSIC] Then I can run the first command I was given to create a network VPC, making sure to replace network name with the name that I want for my network and I can click enter to run it. Great, and I can see here that my VPC was created. Next, I'll create the dual stack subnet in my VPC network by running the other command I was provided. This time, I'll need to replace the subnet name, network name, access type, subnet range, and region. [MUSIC] Nice, and just like that, my VPC and subnet have been created. If I wanted to make additional subnets, I can just repeat this step. So that was actually pretty easy. With the help of Gemini, I was able to find helpful networking information for Google Cloud. And how to create a VPC without having to leave the console and with really minimal knowledge of Google Cloud. [MUSIC]

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/884/quizzes/476764)

#### Quiz 1.

> [!important]
> **How can you use Gemini chat to help you with a network architecture task?**
>
> - [ ] With a brief description of your needs, Gemini can design a complete network architecture.
> - [ ] Type a specific prompt into Gemini related to your network architecture concern.
> - [ ] Gemini automates the creation of most parts of a Google Cloud VPC network architecture.
> - [ ] When performing network architecture tasks in Google Cloud console, Gemini automatically guides you through the process.

### Document - [Next Steps](https://www.cloudskillsboost.google/course_templates/884/documents/476765)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
