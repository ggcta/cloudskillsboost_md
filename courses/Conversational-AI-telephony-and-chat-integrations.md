---
id: 1013
name: 'Conversational AI telephony and chat integrations'
type: Course
url: https://www.cloudskillsboost.google/course_templates/1013
date_published: 2025-01-23
topics:
  - Customer Service
---

# [Conversational AI telephony and chat integrations](https://www.cloudskillsboost.google/course_templates/1013)

**Description:**

This course explores how telephony systems can connect with Google to enable phone-based interactions within the Conversational AI ecosystem

**Objectives:**

* Understand the basics of telephony connectivity and architecture.
* Identify how different telephony connectivity configurations can affect the accessibility of Conversational Agents and Agent Assist features
* Review other Frontend integration options from one-click telephony to open source SMS

## Telephony Connectivity

This module explores the key technologies that facilitate the integration of telephony systems with Google Conversational AI

### Video - [Basics of telephony networks and Conversational AI telephony architecture](https://www.cloudskillsboost.google/course_templates/1013/video/521877)

* [YouTube: Basics of telephony networks and Conversational AI telephony architecture](https://www.youtube.com/watch?v=dm6jedMkpZQ)

SPEAKER: Welcome to CCAI front end integrations. This training will provide you with an overview on how telephony contact centers connect to Google to enable phone based interactions within your CCAI ecosystem. We'll delve into the configuration of telephony conversation and how different integrations can affect the behavior and features of Virtual Agent and Agent Assist. We'll also introduce a range of integration options from one click telephony to open source SMS. Let's first gain an understanding of the key technologies involved connecting telephony with CCAI. We'll start by reviewing the basics of telephony networks and how they apply to the CCAI telephony infrastructure. We'll then review the preferred telephony integration options, including CCAI Platform, Google Cloud's own offering for a modern AI powered contact center as a service, as well as OEM telephony integrations and CCAI connectors. Let's get started. Let's start diving into the fundamentals of telephony networks and CCAI telephony architecture. Our starting point will be the basics of telephony connectivity. We will begin by defining two foundational concepts, public switched telephone network and session border controller. A Public Switched Telephone Network, or PSTN, is a combination of telephone networks used worldwide. It includes telephone lines, fiber optic cables, switching centers, cellular networks, satellites, and cable systems. A PSTN lets users make landline telephone calls to one another. A Session Border Controller, or SBC, is a special purpose device that protects and regulates IP communications flows. As the name implies, session border controllers are deployed at network borders to control IP communication sessions. It was originally conceived to protect and control VoIP networks. However, SBCs are now used to regulate all forms of real time communications, including VoIP, IP video, text chat, and collaboration sessions. Let's see how PSTNs and SBCs are used within CCAI. With a built in Dialogflow CX phone gateway integration, Google provides a phone number for your business that anyone can call. The caller's phone provider routes the call to Google's telephony platform through a PSTN, where the telephony provider network is paired with Google's. This is where Google uses an SBC to protect the network. As the call arrives and remains active, the SBC and media controller direct telephony audio into gRPC streams with the CCAI endpoints. Caller audio streams into CCAI and Virtual Agent audio streams back to the caller. This continues until the call is terminated by the caller or by Google telephony platform when Dialogflow reaches the end of the session. This direct integration at the PSTN allows the customer to control the call flow entirely with Dialogflow and webhooks. However, in reality, customers contact centers have multiple suites of solutions that require integration with CCAI. These integrations need control of the call flow from the customer premise, yet often customers prefer to not worry about the implementation details of the gRPC. What options do these customers have to connect their contact center suite with CCAI? One option they have is SIP, a Session Initiation Protocol commonly used to control audio sessions within contact centers. SIP is a signaling protocol used for initiating, maintaining, and terminating two way communication sessions around the world. It's supported by most session border controllers deployed within contact centers. SIP sessions can include two way voice, video, and messaging applications. Contact centers often use SIP as an additional layer of control over the phone call's audio streams and, as such, can be used to stream audio in and out of CCAI. One other option that can be pursued as an alternative or in conjunction to SIP is SIPREC. SIPREC or SIP for recording is similar to SIP in the sense that it offers some control over the media session. But while SIP supports two way audio, SIPREC is designed for recording and transcription. We'll see how this can be used for CCAI Agent Assist to analyze conversations, but note that SIPREC is not relevant to virtual agents that directly communicate with the caller. Let's see how SIP and SIPREC can help connect to CCAI. First, a system integrator or ISV sets up a SIP connection from your existing contact center solution to a CCAI connector. SBCs then secure each side of the SIP connection. The CCAI connector then has three options to connect to Google. GRPC, SIP, or SIPREC. In either option, no network is paired with Google's. The first option sees the connector communicating directly with CCAI APIs. The CCAI connector is responsible for effectively translating SIP streams to gRPC, and establishing other integrations with a contact center. The second option is to connect with Google's telephony platform using SIP. Technically, you can integrate directly with SIP to Google telephony. However, a direct SIP only supports Virtual Agents, not Agent Assist. A CCAI connector can enable Agent Assist as well. The third option uses SIPREC instead of SIP when connecting to Google's telephony platform. Compared to the other options, SIPREC offers limited control for handling the stream and is only capable of sending audio to CCAI. Likewise, SIPREC does not support virtual agents that need to reply to callers. However, Agent Assist integrations can work with SIPREC. While SIP connects the audio streams, other data about the CCAI session can be accessed through Pub/Sub. For example, Dialogflow session parameters or Agent Assist coaching. Integration partners subscribe to the Pub/Sub to make the data available within your existing business rules and agent desktops. With all that in mind, note that some full contact center suites offer direct integrations with CCAI. CCAI platform and OEM CCAI integrations both take control of the gRPC streams to call the CCAI APIs. By managing the streams directly, these integrations maintain the most control over the user experiences with CCAI. Regardless of the option you or your customer decides to pursue, each platform is responsible for maintenance, primary support, and implementing new features.

### Video - [Telephony integration options](https://www.cloudskillsboost.google/course_templates/1013/video/521878)

* [YouTube: Telephony integration options](https://www.youtube.com/watch?v=OD1R-i3aMog)

SPEAKER: With respect to the prior architectural considerations, as well as the specific demands of your contact center, you can pursue different integration options. One option is migrating your contact center solution to CCAI Platform. Another option may be to enable your existing solutions with one of the CCAI OEM partner integrations. And a third option is using CCAI Platform over the top or a CCAI connector to add AI to your legacy infrastructure. Let's explore each of these options, starting with CCAI Platform. CCAI Platform is Google Cloud's own CCaaS offering for a modern, AI-powered Contact Center As A Service. In other words, it is a complete solution to your contact center needs with CCAI built in. We will not deep dive into CCAIP in the context of this training. But it is important for you to know that CCAIP completes the contact center solution around the core CCAI technologies. On top of the core AI technologies offered by CCAI, the platform completes the picture by providing inbound and outbound integrations, visual IVRs, AI-driven agent routing, agent assist integrated desktop, prebuilt platform integrations, and even SDKs to embed support in your websites and applications. Refer to the additional resources for more information on Contact Center AI Platform. The second available option is to leverage CCAI partner integrations alongside your or your customer's existing interactive voice response and contact center operations. These integrations are certified by Google and bring the power of CCAI to the most popular contact center platforms by providing solution completeness, pre-engineered integrations, enterprise support, and seamless virtual agent handoffs to human agents, supercharged with Agent Assist for Voice. Let's review each capability, starting from solution completeness. For live voice use cases, or for omnichannel use cases, CCAI is not a complete solution in itself. Customers need additional components from their IVR or contact center platform provider to enable their Virtual Agent or Agent Assist use cases. CCAI OEM partners provide bundled solutions that include the CCAI APIs and the rest of the components required for a successful customer implementation. The second capability provided through OEM telephony is related to pre-engineered integrations. For live voice use cases in particular, the engineering required to integrate with an IVR and a contact center platform is non-trivial. CCAI OEM partners have already completed the integrations of CCAI with specific product or version levels of on-prem and cloud-based products. This increases quality and the speed of the integration and lowers the cost of deploying CCAI within supported products or versions. It also ensures end-to-end maintenance for solution upgrades over the life of the integrated products through the OEM partner. OEM partners provide enterprise support and take Level 1 and Level 2 responsibility for supporting the integrated solution end to end. When there is an issue, they troubleshoot from the front of the customer integration through fulfillment. Is it the phone gateway? Is it the IVR switching? Is it a routing table? Is it a network connection? All of those components are outside of Google Cloud's purview and directly addressed by the OEM partners. When the issue pertains to Dialogflow or Agent Assist or other Google Cloud products, Google takes part of the OEM partner support chain. Bottom line is, stringent support engagement procedures were established with all CCAI OEM partners, so there's predictability in the process when issues arise. Worth mentioning is also the ability for OEM partners to independently enable Agent Assist for Voice. There are many architectural requirements to provide live transcriptions and coaching to human agents in real time. Also, there's no public SKU, and customers cannot buy Agent Assist for Voice directly from Google Cloud without an OEM, certified CCAI connector, or CCAI Platform. Agent Assist integrations available through CCAI OEM partners allow for a seamless transition when a customer moves from a Dialogflow powered voice bot or chatbot to a live agent call with Agent Assist. With those benefits in mind, let's look at the two ways to complete an OEM integration. Some OEMs offer easy, one-click integrations with CCAI directly from the Dialogflow console. These partners include AudioCodes, Avaya, Genesis, SignalWire, and Voiximplant. One-click integrations are for customers who already utilize one of these providers and want to add the benefits of Contact Center AI on top of their existing solution. If you don't already have an implementation by one of the partners mentioned here, then you can reach out to your Google sales representative for a consultation. If your OEM telephony integration is not available as a one-click, then you'll need to manage the service accounts and keys yourself. Start at the IAM page of the Google Cloud console, also referenced in resource number two of the additional resources documentation at the end of this training. You'll need to create a new service account for the integration and assign the following roles-- Dialogflow API Client, Dialogflow API Reader, Dialogflow Conversation Manager. Next, create the service account key, and download the JSON file from IAM. Finally, follow your telephony partner's instructions to upload the service account key to your integration. The final preferred option for contact centers not on CCAI Platform or one of the OEM solutions is to utilize a CCAI connector. Connectors are an offering from system integrators or ISVs. As we learned earlier, the Google certified partner implements a SIP integration to the customer's existing contact center solution and integrates with CCAI using gRPC, SIP, or SIPREC. Some certified CCAI connectors can even provide Agent Assist for voice, just like the CCAI platform and OEM solutions.

### Quiz - [Telephony Connectivity Quiz](https://www.cloudskillsboost.google/course_templates/1013/quizzes/521879)

#### Quiz 1.

> [!important]
> **My customer wants to have a direct deal for CCAI, and not buy through an OEM partner or CCAI Platform.  Can I do that? (Choose three)**
>
> * [ ] Yes, the customer will implement their own streaming audio solution using gRPC or SIP.
> * [ ] Yes, the customer's telephony partner offers "bring your own AI" with a prebuilt CCAI integration.
> * [ ] Yes, the customer will not need live voice features
> * [ ] Yes, a third-party ISV offers a CCAI connector for the customer's contact center.
> * [ ] No, CCAI APIs are not publicly available.

#### Quiz 2.

> [!important]
> **Which of these protocols support telephony virtual agents? (Choose two)**
>
> * [ ] MQTT
> * [ ] SIPREC
> * [ ] gRPC
> * [ ] SMTP
> * [ ] SIP

#### Quiz 3.

> [!important]
> **Which of these connectivity protocols does CCAI support for live voice integrations? (Choose three)**
>
> * [ ] REST
> * [ ] SIPREC
> * [ ] SMTP
> * [ ] gRPC
> * [ ] MQTT
> * [ ] SIP

#### Quiz 4.

> [!important]
> **Which of these protocols support telephony agent assist? (Choose three)**
>
> * [ ] SMTP
> * [ ] gRPC
> * [ ] SIPREC
> * [ ] MQTT
> * [ ] SIP
> * [ ] Pub/Sub

#### Quiz 5.

> [!important]
> **What do OEMs, CCAI Platform, and CCAI connectors all provide on top of CCAI? (Choose four)**
>
> * [ ] Contact Center Solution completeness
> * [ ] Pre-engineered integrations
> * [ ] Quality projections based on historical call recordings
> * [ ] Seamless virtual agent handoffs with Agent Assist for Voice
> * [ ] Support for all third-party CRM
> * [ ] Compatibility with existing infrastructure
> * [ ] Full solution enterprise support

#### Quiz 6.

> [!important]
> **A customer wants to upgrade their DTMF-based IVR with a virtual agent. When the virtual agent cannot contain the call, the customer wants the call routed to a relevant department with all of the context from the virtual agent. Which of these integration options should you consider? (Choose two)**
>
> * [ ] gRPC endpoint
> * [ ] SIPREC endpoint
> * [ ] Dialogflow CX Phone Gateway
> * [ ] CCAI Platform
> * [ ] Partner integration or connector

## Telephony Conversations

This module explores the lifecycle of a telephony conversation, the most important configurations for the setup of telephony integrations and some key considerations for using third-party features with Conversational AI

### Video - [Telephony conversations overview](https://www.cloudskillsboost.google/course_templates/1013/video/521880)

* [YouTube: Telephony conversations overview](https://www.youtube.com/watch?v=GOaB3P4_ONg)

SPEAKER: Now that we know how telephony systems are connected to CCAI, let's look at the architecture of the conversation within CCAI. This section has three main objectives. First, you'll learn how a CCAI conversation operates. Then you'll explore important configurations for telephony integrations. And then you'll review some key considerations for using third-party features with CCAI. Let's dive right in. Starting at the beginning of any call, telephony providers have the ability to identify callers through caller ID, also known as CNAM, which is short for Caller ID Name. The originating phone switch sends the caller's number to the receiving telephony provider. The provider's software can then extract key information from its call records. Contact center software can often search this information against the business's database. This allows, for example, a business to look up names, addresses, account info, and recent support interactions by phone number to better support users. Any appropriate data can be used over the life of the call, even if it gets transferred throughout the call center. Your virtual agent can take advantage of this data to help authenticate users for personalized prompts and remain relevant to the caller's needs. Traceability of these interactions is important for routing as well as real-time and historical reporting. This is why a conversation ID is assigned to the session of each interaction at the beginning of the call. As mentioned, all real-time voice integrations are eventually converted to gRPC streams exposed via CCAI endpoints. A unary gRPC has a single request that may contain additional parameters for CCAI to use as session parameters, like caller ID. Conversations typically begin with a unary request for a welcome event. Event inputs are programmatic triggers to the virtual agent. In this case, they're used to begin the conversation. For telephony, the unary response contains synthesized audio for the client to play back. As the conversation continues, the client opens a new gRPC channel for each conversation turn. Although audio inputs are the most common, each stream can also handle text, programmatic events, and DTMF inputs. Telephony connections can support all of these input types, typically using a bidirectional gRPC stream. The client manages a stream of audio for CCAI to detect, process, and respond to user speech. If at any point in the stream the client sends some nonaudio input, the audio is ignored in favor of the other input. This example shows a client opening a second stream after the initial welcome event. This client starts streaming audio to CCAI. While the client continues streaming audio, Dialogflow listens for speech and transcribes it to text using speech to text. At some point, CCAI detects that the user has started speaking. The client continues streaming until CCAI detects that the user is finished speaking. When the client stops sending audio, CCAI's NLU finalizes its speech processing and proceeds by understanding the intent and satisfying the configured fulfillment, possibly calling customers' webhook, before synthesizing a final response through text to speech. The telephony client waits for the last response from CCAI. Once the virtual agent's response is generated, the bidirectional stream ends. The integration plays back the response to the user and begins a new stream for the next turn. This repeats for every turn. Responses can also be configured in Dialogflow to allow barge-in. This means that the caller is allowed to interrupt the virtual agent to proceed in the conversation. With barge-in enabled, new streams listen for input while the virtual agent is talking. If your webhook takes a long time to process, you can enable partial responses to say something while the user waits, like, OK, let me check that for you. And if CCAI detects no speech for some time, then it logs it as no input, which gives the virtual agent a chance to reprompt the caller. If the virtual agent is unable or not authorized to fulfill the request of the user, the virtual agent can escalate the request to a human. At this point, if your human handoffs are powered by Agent Assist, the integration adds the new human participant to the conversation. The integration opens two parallel streams to CCAI APIs, one for the caller and one for the agent. CCAI continuously listens to audio on both streams and offers assistance to the human agent in the form of Pub/Sub notifications to the agent's desktop. The CCAI integration handles these Pub/Sub notifications to update the agent's console with helpful information like transcripts or agent coaching.

### Video - [Conversation profiles and agent settings](https://www.cloudskillsboost.google/course_templates/1013/video/521881)

* [YouTube: Conversation profiles and agent settings](https://www.youtube.com/watch?v=zO85tgnmmV4)

SPEAKER: You've now reviewed the processing CCAI provides to the telephony clients. So let's identify the most important configurations that affect the behavior of the processing, starting from conversation profile. A conversation profile is the highest level configuration of your CCAI solution. When a CCAI integration receives a new call, it creates a new conversation object linked to a specific conversation profile. The settings in this conversation profile determine some security settings, Virtual Agent configurations, Agent Assist options, and more. Note, however, that these settings are best viewed as defaults that can be overridden. Here are a subset of the conversation profile options. Many fields are only accessible in the API, although the Dialogflow and Agent Assist console each provide a UI for some fields. For example, speech to text config and text to speech config can set the default speech recognition model and fulfillment voice for some integrations. But integration configuration and Dialogflow Agent Settings may override the conversation profile. For more on these conversation profile options, refer to resources number 4, 5, 6, 7, 8, and 9 in the additional resources document at the end of the training. Keep in mind that Dialogflow's advanced speech settings can further influence the signals and integration will receive. Advanced speech settings can be applied for your entire Virtual Agent, or even for specific flows and pages within the agent. Some examples of these settings include model selection, enable advanced timeout, end of speech sensitivity, enable barge in, no speech timeout, and audio export bucket. Let's take a few moments to explore these settings. One of the most important settings is speech model, since this affects all aspects of speech detection, including start of speech, end of speech, and transcript quality. Leaving the model unspecified is a good starting point, since this ensures other layers of your CCAI application can specify a model as needed. When a model doesn't meet your needs, try a new one. One model might perform better at collecting long digit sequences, while another is best for quickly understanding a yes versus a no. Setting specific speech models for specific Dialogflow pages can also be helpful for optimizing each conversation turn. When choosing a model, it's important to understand that not all speech models offer the same functionality. Notably, some models have strict end of speech, meaning Google decides when the user is done talking. These models include telephony short, latest short, and some command and search models. These models are tuned to recognize individual speech utterances and therefore work well for most virtual agents. Other models do not have end of speech detection built in. Telephony and phone call models, for example, were originally designed for open form telephony conversations that you'd expect in the human agent handoff. However, Dialogflow includes its own end of speech option, which can enable any of these models to work with virtual agents too. Without advanced timeout based end of speech, these models would listen endlessly and never respond to users. Dialogflow's custom end of speech detection can be enabled in the agent settings. Enabling this feature also allows you to use any speech model with telephony integrations. Enabling this feature allows you to tune end of speech sensitivity for any language and integration that relies on Dialogflow to detect end of speech. End of speech sensitivity allows you to adjust how quickly your agent responds to users. Does your agent take too long to respond? Then increase sensitivity for faster end of speech. Is your agent cutting users off too soon? Decrease sensitivity for slower end of speech. Note that strict end of speech models may not respond to decreasing sensitivity. A careful balance for each page can help keep the Virtual Agent feeling responsive, without running the risk of interrupting users. The default of 90 allows for roughly one second of a pause in speech before the bot responds. 95 risks interrupting users, but can work well for short responses. 75 will result in a slower response time to the user's input, but can be useful for collecting complex answers. We briefly discussed barge-in, where a user can interrupt the Virtual Agent. You can set specific responses in your Virtual Agent to be eligible for barge-in or not. Enabling barge-in instructs the telephony integration to start listening while a fulfillment is playing back to the caller. Otherwise, CCAI will ignore any interruptions until it encounters the first bargeable response. When a user doesn't barge in, Dialogflow counts the specified number of seconds to allow the user to start speaking after the bot's response. If the user stays silent for, say, 10 seconds, then Dialogflow provides a no input event that can be programmed into the Virtual Agent logic. This timer starts at the end of the bot's response, and can also be tuned for specific Dialogflow pages and flows when you need to allow the user more time to start speaking. Lastly, an important feature for record keeping and debugging is audio export. Configuring a Google Cloud Storage location for Dialogflow will give you the exact audio bytes received by CCAI for every turn of a conversation. These recordings can lead to significantly faster support resolutions if you experience any issues with your voice integrations, because they will allow you and support teams to reproduce the issue. The text to speech output is also exported for telephony integrations. When it comes to ensuring transcription quality, speech adaptation is your number one tool beside the model selection feature we already discussed. By default, auto speech adaptation knows what intents, training phrases, and entities are expected at any point in the conversation. Dialogflow uses this knowledge to bias speech recognition towards your use case. If you notice a phrase isn't being transcribed properly, try adding the correct phrase to your training phrases or entity synonyms. Also, stronger biasing is needed to accurately collect long digit and alphanumeric sequences. Follow the resources linked at the end of the training to use required form filling and a specific regexp entity in these cases. Additionally, please note that auto speech adaptation works best for sessions programmed within Dialogflow. This means that every conversation turn should contain some audio or event input. If you are programmatically modifying the Dialogflow state outside of a webhook, be sure to use event inputs and not text inputs to trigger these state changes. Dialogflow also allows you to specify manual speech adaptations when auto speech adaptation isn't performing well. For example, if your business jargon or product names aren't being recognized consistently. Manual speech adaptation works best when you specify multiple phrases both with and without the optional boost value. Empty or 0 boost means the biasing helps recognize continuous portions within the phrase. For example, a non-boosted phrase like, are you open to cell phones? Helps recognize utterances like I sell phones and Hi, are you open? Meanwhile, setting a positive boost value applies a stronger bias. But unlike no boost, a positive boost only helps recognize the exact phrase, not similar variations. For example, a boosted phrase cell phones helps recognize can you sell phones, but not do you sell any phones. You cannot set a negative boost value, and Dialogflow will still transcribe non-biased words and phrases to give you insight into what customers are really asking for, even if it can't be answered by the Virtual Agent yet. Be careful not to set too high of a boost, like 20, or your Virtual Agent may start hearing words that were not said. By default, Dialogflow sends all responses to the end user when the agent's turn is over. However, if you need to send responses sooner, then you can enable partial response for your webhooks. This keeps your Virtual Agent feeling responsive even when you need to execute a long webhook process or record lookup. It also allows you to avoid long periods of silence that might otherwise confuse or frustrate the caller. Another feature to offer convenience to your callers is Speaker ID, which lets you identify users based on their voice signature. It works especially well with telephony integrations thanks to caller ID. First, CCAI makes it easy to ask the caller if they want to enroll their voice. Once enrolled, Dialogflow can use the caller ID or some other information you collect to ask your webhook for up to five possible voice signatures to verify from. Speaker ID only verifies matching voices from a list of five options, for both technical and ethical reasons. Caller ID can allow a business to identify up to five customers who might use the phone number, then securely verify the exact caller with Speaker ID. Pre-built Dialogflow components exist for both verification options, either actively asking the user to repeat a random phrase, or passively listening and verifying as the user asks their normal questions. Another helpful feature worth mentioning for telephony integrations is Call Companion. When supported by your integration, Call Companion offers callers a text link to interact with the conversation visually through a visual interface on a user's phone. This way, users can see options quickly while the bot is talking, share input via text or images, and interact with visual elements such as clickable cards to support the conversation, all while the phone call voice input remains active. This can be helpful for collecting complex data like uncommon names, addresses, and long alphanumeric sequences, or just to interact with users that prefer a visual format. Ask your CCAI partner and Google sales representatives for more details about this feature.

### Video - [Overriding Conversational AI configurations](https://www.cloudskillsboost.google/course_templates/1013/video/521882)

* [YouTube: Overriding Conversational AI configurations](https://www.youtube.com/watch?v=HMujqQwFS3Y)

SPEAKER: Many of the features we just looked at are affected by multiple layers of configuration. Let's review some key considerations that may help you in debugging the behavior of your Virtual Agent features. Keep in mind that most features require some implementation from the integration. Therefore, some integration options may override or affect any behavior. Also, some features, like Advanced Speech Settings, Partial Response, and more can be configured from various layers of Dialogflow settings. For example, you can configure an audio export bucket in a Virtual Agent's flow settings. This will override agent-level settings and supplement conversation profiles security settings. Or you may, for example, enable barge-in for an entire flow. However, individual parameter and fulfillments may still explicitly disable barge-in. It's important to identify the specific pages and fulfillments when analyzing system behavior, so please make sure to check each of these Dialogflow settings if you experience unexpected behavior. Also note that OEM partners have other, oftentimes, legacy integration configurations that conflict with CCAI features. Using these features may lead to lack of support or unexpected behavior when used in combination with other features. When in doubt, make sure to contact the integration owner for primary support. Lastly, keep in mind that many noncertified integrations are created by other organizations and individuals using the public Dialogflow APIs. The implementation of these integrations has not been certified by Google, which means they may or may not cause issues. For example, some independent integrations mix and match services like separate APIs for Speech-To-Text and Dialogflow. In such a case, features like barge-in, speech adaptation, speech transcripts, agent assist, and more may operate differently than a certified CCAI integration. For these reasons, make sure to contact the integration owner for primary support.

### Quiz - [Telephony Conversations Quiz](https://www.cloudskillsboost.google/course_templates/1013/quizzes/521883)

#### Quiz 1.

> [!important]
> **Which of the following advanced speech settings is most impactful to the performance of your solution.**
>
> * [ ] Barge-in
> * [ ] Speech model
> * [ ] End of speech sensitivity
> * [ ] Advanced timeout-based endpointing

#### Quiz 2.

> [!important]
> **Which of the following are sent through telephony integration's gRPC to the CCAI APIs? (Choose three)**
>
> * [ ] End of speech detection
> * [ ] Start of speech detection
> * [ ] The caller's geolocation
> * [ ] Programmatic events that change the conversation state
> * [ ] The caller's audio stream
> * [ ] Session parameters

#### Quiz 3.

> [!important]
> **Which of the following are returned from the CCAI APIs through the telephony integration's gRPC. (Choose three.)
**
>
> * [ ] The Caller's IP Address
> * [ ] The caller's geolocation
> * [ ] Programmatic events that change the conversation state
> * [ ] Start of speech detection
> * [ ] Session parameters
> * [ ] The caller's audio stream

#### Quiz 4.

> [!important]
> **Google support asks you to share an audio recording of a problem behavior you've reported with your telephony experience. Which of the following considerations should you take: (Choose two)**
>
> * [ ] Record calls from your CCAI contact center solution.
> * [ ] Test in the Dialogflow console and record your screen and mic.
> * [ ] Record your call from an app on your phone to get the original audio source.
> * [ ] Encode as MP3 files so they can be shared with support more easily
> * [ ] Check that the caller and agent audio are in separate files, or separate channels of a stereo audio.

#### Quiz 5.

> [!important]
> **You need at least one conversation profile per: (Choose three)**
>
> * [ ] Session
> * [ ] Human Agent
> * [ ] Release version
> * [ ] Dialogflow agent
> * [ ] Unique Agent Assist feature combination
> * [ ] Language

#### Quiz 6.

> [!important]
> **Built-in Dialogflow features like barge-in, speech adaptation, and partial responses ensure consistent experiences regardless of your integration method.**
>
> * [ ] False
> * [ ] True

#### Quiz 7.

> [!important]
> **Your virtual agent has trouble understanding users. When you check Dialogflow conversation history, the transcripts do not match what the user said. You enable Dialogflow's audio export bucket to record some calls that exhibit the issue and notice the speech is clear and understandable. How might you fix this?**
>
> * [ ] There's nothing I can do without implementing my own speech recognition..
> * [ ] Enable call companions to offer users an alternative input method.
> * [ ] Specify manual speech adaptations for the phrases I want to transcribe correctly.
> * [ ] Be patient. Google models will eventually adapt to my users' speech and my use-case.
> * [ ] Check that auto speech adaptation is enabled, then make sure the agent's training phrases and entities contain the phrases the users are actually saying.
> * [ ] Ensure that I collect alpha/numeric sequences (like 12345678 or ABCD1234) through form-filling.
> * [ ] Configure a different Google speech model better suited for my use-case.

#### Quiz 8.

> [!important]
> **When you test your virtual agent through your telephony integration, you experience long periods of silence before hearing a response to your inputs. How might you fix this? (Choose four)**
>
> * [ ] Check the performance of my fulfillments' webhooks.
> * [ ] My integration offers an option to specify the maximum number of seconds to wait after a user speaks.
> * [ ] Contact my integration owner for troubleshooting any networking or other processing issues.
> * [ ] Enable advanced timeout-based endpointing and increase the sensitivity slider.
> * [ ] Enable advanced timeout-based endpointing and decrease the sensitivity slider.
> * [ ] Specify a different speech model.

#### Quiz 9.

> [!important]
> **Which of the following features could help reliably authenticate users to your virtual agent? (Choose three)**
>
> * [ ] Speaker ID tells me which one of my many enrolled users is speaking
> * [ ] I can use a regexp entity and collect an alpha/numeric ID with required form-filling
> * [ ] I can use a regexp entity and collect an alpha/numeric ID by annotating the entity in intent training phrases.
> * [ ] I can lookup known users from Caller ID then use Speaker ID to tell me which one is speaking
> * [ ] I can cross-reference Caller ID with a DTMF-collected pin code

## Other integrations

This module explores examples of additional integrations, covering both open source solutions and those built into Conversational Agents

### Video - [Other integrations](https://www.cloudskillsboost.google/course_templates/1013/video/521884)

* [YouTube: Other integrations](https://www.youtube.com/watch?v=UE7vCfLDFKQ)

SPEAKER: While telephony is critical to many contact-center operations, it's not the only place where people seek help or information. Let's review some other types of integrations to understand more. The objectives of this section are to introduce additional integration points, both open source and built in, and deep dive into one of each, the built-in Dialogflow messenger and an open-source WhatsApp integration. Although these integrations do not offer all of the CCAI features, they can still help extend a customer's support reach across several popular online platforms. So what's the difference between built-in integrations and open source? Built-in or one-click integrations are supported by Google and are easily configured in the Dialogflow console. Examples include Google Chat, Facebook, LINE, Slack, and Telegram. Open-source integrations are integrations that Google contributed code to, supported by the community. They can be forked, modified, and published for more custom integrations. Examples include Skype, Twitter, and Viber. Both types of integrations let you leverage your CCAI virtual agent to help reduce you or your organization's support-channel contact rate. Let's review an example of how to reuse the same Dialogflow agent that powers your contact center to create a Dialogflow CX Messenger functionality for your website visitors to ask questions. Dialogflow CX Messenger provides a customizable chat dialog for your agent that can be easily embedded in your website with five to six lines of code. You can even reuse the same Dialogflow agent that powers your telephony integration. However, please note that this integration does not include human handoff, agent assist, and insights built in. You can implement custom functionalities in Dialogflow CX Messenger through additional HTML and JavaScript. Let's look at the main steps for this configuration. After creating a virtual agent in Dialogflow, just click Publish in the console, configure the required options in the pop-up, and then get the HTML to embed on your website. Once you identify the pages where the chatbot should be embedded, add the copied code to the appropriate location and deploy the app. Once the app is deployed, you'll see the chat bubble showing up in your website. You can create a custom event on your agent's start page to greet the user when the page loads or use JavaScript to call built-in Messenger functions programmatically. The integration offers large amounts of customization. For example, Dialogflow Messenger allows you to define custom templates, like a date selector. Components like this can make it even easier for users to get things done. By adding a date picker, users can choose to enter a date with natural language text or visually. To configure this option, we first need to create a custom web component. This can be created within JavaScript, and it can implement the HTML element, manage custom UI elements, and then respond to events to handle user input. Refer to the additional resources documentation at the end of the training for more information on custom components. Here's a simple example of a web component created in JavaScript for a date picker. We define dfPayload and dfResponseId, which will be automatically filled by Dialogflow Messenger when selecting a new date calls the input's change EventListener. The connected callback then adds the UI elements to the DOM and defines what to do when the user changes the selected date. In this example, the selected date is sent to Dialogflow as a text input for further processing. Once the web component is defined in the web app, we can tell Dialogflow Messenger to render it with any fulfillment using a custom payload response. Please note that the name defined in the custom payload and the name of the registered web component should match. When the Dialogflow returns the custom payload to Messenger, this will allow you to see the date picker up here. Another feature is the ability to upload files to a virtual agent. This can bring multimodal capabilities to the experience-- for example, the ability to upload an image to a vision AI to detect product defects. This feature is available out of the box with Dialogflow Messenger. Enabling file upload involves two steps. First, set the attribute enable-file-upload in the df-messenger HTML tag. Second, provide the name of the cloud storage bucket into which this file needs to be uploaded using attribute gcs-upload. On deploying, you will be able to see the File Upload button. For end users to be able to upload files to this bucket, make sure to add the Storage Object Creator role to the allUser or allAuthenticatedUsers principal, as shown here. This will allow you to upload any file to the provided Google Cloud location. This was just an example of a one-click integration. Keep in mind that Dialogflow permits similar integrations with other conversation platforms, such as Google Chat, Google Assistant, Slack, and Facebook Messenger. These built-in integrations are seamless and make it easy for many developers to just focus on bot quality rather than front-end integration. Each integration handles end-user interactions in a specific way. For more details on the documentation for your chosen integration platform, refer to the additional resources. Now let's look at one example of an open-source integration. Let's take the example of an integration Google contributed code to, but this code is not available out of the box through Dialogflow. These integrations require a little more effort to set up and maintain, but they can greatly expand the reach of your virtual agent. For example, let's see how we might expand the reach of a virtual agent to all of the WhatsApp users around the world through an open-source integration with Twilio SMS service. Start by setting up a free Twilio account. After following some quick steps, including providing your account details and authorization tokens, you'll receive a Twilio sandbox to develop with. Refer to the Additional resources document for links to Twilio and the WhatsApp sandbox. After setting up your account and sandbox, you can deploy the open-source integration between Twilio and Dialogflow. Clone the open-source WhatsApp integration repo, and follow the steps on the README file as follows. Replace the environmental variables with your details. Build and push the image. Then run the container on Cloud Run with a single gcloud command. Once the Cloud Run service is up, you can enable unauthenticated access to ensure Twilio can invoke the service. Note that this approach only applies for a test or a demo, as a production service must always properly authenticate. To perform authentication for a demo or a test, go to Cloud Run Console, open the new twilio-df-integration service, and then click on Security and Allow unauthenticated invocations. For more information on authentication in Twilio, refer to the Additional resources document at the end of the training. Finally, you can connect Twilio to the Cloud Run endpoint you deployed. On the Cloud Run console, locate the twilio-df-integration service. Then open the service and copy the Cloud Run-assigned URL. On the Twilio sandbox configuration, locate the When a message comes in setting. Then append the designated POST method name to the provided URL. Ensure this updated value is saved. For reference, the method name employed within this repository /twilio-dialogflowcx Once all the steps are completed, you can test the integration from the Twilio sandbox. For more information on connecting Twilio to Cloud Run and configuring your Twilio sandbox, refer to the Additional resources document at the end of the training. This concludes this training. Congratulations, and good luck choosing the best integration options for your CCAI solutions.

### Quiz - [Other Integrations Quiz](https://www.cloudskillsboost.google/course_templates/1013/quizzes/521885)

#### Quiz 1.

> [!important]
> **Dialogflow CX Messenger has built-in support for these CCAI features:**
>
> * [ ] Agent Assist
> * [ ] Chat with a virtual agent
> * [ ] Contextual handoff to a human agent
> * [ ] Export sessions to CCAI Insights

#### Quiz 2.

> [!important]
> **What are some benefits of choosing an open source integration?**
>
> * [ ] Allows you to extend your reach to platforms that do not have built-in integrations.
> * [ ] The community maintains the code so my integration will stay up to date.
> * [ ] You can get all the benefits of CCAI, plus you can customize how the integration works.
> * [ ] Your developer team may fork the integration to suit your needs.

#### Quiz 3.

> [!important]
> **Your employer asks you to design an AI-driven multi-channel automated voice and text solution across telephone, website, and social media. Which approach should you take?**
>
> * [ ] Integrate voice, web, and social channels in one solution architecture with a common Dialogflow virtual agent.
> * [ ] Create separate telephony, text, and social channel solutions, and keep the dataseparate too. You cannot mix channels in your virtual agent.
> * [ ] Utilize separate telephony, chat, and social channel solutions, but use the same Dialogflow for each so you can merge data at the backend.
> * [ ] Build a separate Dialogflow virtual agent for each channel (voice, web, social) and connect them together using backend logic to transfer conversations seamlessly.

## Additional Resources

This module includes the list of additional resources that complement the course learning

### Document - [Additional Resources](https://www.cloudskillsboost.google/course_templates/1013/documents/521886)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
