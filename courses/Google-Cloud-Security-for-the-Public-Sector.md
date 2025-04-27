---
id: 502
name: 'Google Cloud Security for the Public Sector'
datePublished: 2024-07-02
topics:
- Google Cloud Armor
type: Course
url: https://www.cloudskillsboost.google/course_templates/502
---

# [Google Cloud Security for the Public Sector](https://www.cloudskillsboost.google/course_templates/502)

**Description:**

Work Safer

With Work Safer, public sector organizations can benefit from a cloud first, zero trust security model that provides always up-to-date protection against cyber-attacks. The endpoint security covers mobile devices, desktop devices, Chromebook laptops, and meeting room hardware giving an elevated user experience for all users.

DDoS mitigation and network threat intelligence in Google Cloud

This session discusses mitigation techniques provided by Google Cloud to protect workloads from distributed denial-of-services (DDoS) attacks using Google Cloud Armor and its advanced threat intelligence features. Mitigation topics covered in this course include Adaptive Protection, bot management, rate limiting, and managed protection.

Assured Controls in Google Workspace

Assured Controls helps you meet compliance standards in regulated markets such as the public sector. Learn how you can control provider actions related to your data.

**Objectives:**

- Describe Google Cloud's approach to security.
- Recognize how Google Cloud incorporates their own security best practices into products and services.
- Protect your business with BeyondCorp and ReCaptcha.
- Describe how Google Cloud implements their own security practices to provide customers with enterprise-grade protection.
- Describe Google's network security architecture.
- Summarize Cloud Armor and use it to protect workloads from DDoS attacks.
- Describe Cloud Logging, Cloud Monitoring, and the Security Command Center.

## Cloud-first, zero trust cybersecurity with Google Cloud

This module gives an overview of Work Safer and introduces some common use cases. In addition, this module explains Google's approach to security and shows how Google implements their own security measures into customer products and solutions.

### Video - [The increased risk of cybersecurity attacks](https://www.cloudskillsboost.google/course_templates/502/video/490329)

- [YouTube: The increased risk of cybersecurity attacks](https://www.youtube.com/watch?v=VHu2miCQNew)

Rancho: Introducing Work Safer program. Work Safer gives you that end-to-end detection and protection against all these threats and malware attacks that we have all seen. This is essentially what we are going to talk about today on, what are these components and how they all tie together, giving you that whole security and reduced overhead for your admins? And how does this look like for your end users when they are trying to use the day-to-day applications that they are familiar with? Let's look into the why. We all can agree that we-- the whole way that we work has completely changed. There are several of us who are working from home at this point. With a show of hands, I can say you all would agree. Not only working from home, but I've seen telehealth services being provided. I have seen field offices running around with field engineers still being engaged and working out of mobile devices and tablet devices, going on the road, and making sure that everything is accessible wherever they are connecting from. And those that are working from home, we all have challenges with distracted environments, whether it being pets or the family or other dependencies that we have going on around us. With all these distracted environments, the focus towards saving our data and keeping it secure, it loses a little bit. We are seeing customers suffer due to phishing attacks. And emails still continue to be the number one vector of attack. Can you imagine one of your CFOs or CEOs being spoofed and all your employees getting emails pretending them being a CEO and asking for some confidential, sensitive information. A simple spoofing attack or a phishing attack, it brings in all the vulnerabilities from your users. There are about 80% of the reported security incidents that emerge out of phishing attacks. And due to these tactics and ever-changing newer methods of hacking, the whole security platform needs to be constantly upgraded. Coupled with possible employee negligence and 15 times rise in ransomware attacks because of all this working-from-home and distributed-work environments, we need to have additional focus towards keeping the domain secure.

### Video - [How Google can protect your business](https://www.cloudskillsboost.google/course_templates/502/video/490330)

- [YouTube: How Google can protect your business](https://www.youtube.com/watch?v=b0oBZq1GKns)

Rancho: So while we are thinking on that, Google made sure we took a different approach towards all these attacks. Because these attacks, even though they are evolving, they have predominantly remained the same over the past 20 years. So how can we get ahead of it? How can we make sure that we identify and detect these malware and threats ahead of time with an action plan of how to mitigate that? There is no point on finding stuff when you don't know how to remediate or act upon it. So with that, Google made sure that our infrastructure is designed with the core tenets of trust nothing, detect everything, secure collaboration, and making sure we protect all the data, whether it's the endpoints, users, and the data itself. Trust nothing. Implicitly it assumes breach and focuses on detection and response. So we provide consistent verifiable control throughout the Cloud. No matter which endpoint a user is logging in from, we need to be able to authenticate the user and allow authorization to the respective apps the user is allowed to log into. And when the same user is repeatedly logging in, we trust nothing and the same amount of authentication protocols are executed again. With client-side encryption on Google Workspace, customer data is indecipherable by Google. Where customers and the domain owners themselves, they own the keys and the data that is being stored in Google. It gets encrypted using customer-owned keys. And detecting everything, only Google has breadth and depth of data to identify and train machine learning models. And we'll look into how that works in the upcoming slides. Talking about spam and phishing. With the scale of data that Google deals with, with over eight Google services that have over a billion users, we've collected a lot of spam and malware and heuristics and patterns of bad actors, which has helped us train our machine learning models to prevent spam and phishing messages from reaching your end users' inbox and we can quote 99.9% accuracy on that. With the rollout of FIDO approved Titan keys as your second step verification for your logins, beyond username and password, these keys keep your accounts secure and we have seen zero account hijackings when these keys are being used. Work Safer hereby gives you that power to bring not only a secure collaboration for the end users, but it also removes that overwhelming overhead for the admins in order to configure this, roll this out, and also maintain that in the future. ReCAPTCHA is going to give you that frictionless granular ranking of users when they are trying to log in without having to go through multiple ways to prove themselves as not being bots or bad actors. And with Pixel phones, we have added multiple layers of security that gives you that true Android device management where you can push policies, you can make sure that all endpoints are secure. And when I talk about endpoint security, BeyondCorp is our foundational solution that ties all of this together. Not only for your end users, but also for the devices. And not only for the Google solutions, even for on prem solutions, LDAP based apps that are connected to your identity. BeyondCorp makes sure that all those apps can be accessible in a secure way. Chrome Enterprise gives you that mobile device management capability and it extends also to browsers. So even your Windows laptops, your Linux, your macOS, whichever OS you are using, your Chrome browsers are fully secure. And to add another layer of protection, we have Palo Alto Chronicle and Crowdstrike together. So this program altogether gives you that end to end security that is applicable for any size of domains that you are working with. And talking about Google, Google has made the commitment towards improving cybersecurity. And not just commitment, we have given the promise of investing $10 billion over the next five years to strengthen cybersecurity, and there are several programs that are getting initiated and Work Safer happens to be the first of the actions so that we can bring in the true zero trust architecture that all public sector and highly regulated industries can implement on their end.

### Video - [Google Workspace Security and Resilience Framework](https://www.cloudskillsboost.google/course_templates/502/video/490331)

- [YouTube: Google Workspace Security and Resilience Framework](https://www.youtube.com/watch?v=8Tni2X_DaVc)

Rancho: Talking about regulated industries and public sector, there are several compliance standards that we all have to deal with, right? Whether you are creating a mapping of what features you're going to use or Google trying to present our capabilities, we all go through how our solutions are compliant to your regulatory standards. So taking NIST and FedRAMP regulations, all of these compliance standards into mind, we have put this together as our resilience framework, which shows you typically for NIST tenants identify, protect, detect, respond, recover are the main pillars of execution for your framework, right? So considering that, identifying your assets and understanding your overall cyber risk is the crucial first step. And Google helps you do that using asset management, device management within Google Workspace, and it also has a very granular IM permissions when you are hosting workloads within GCP. When we talk about protection, it's not only just for the admins, we also are aiming towards de-risking the user. Because end users need not hold the responsibility, but the system, by itself, has to remind the user they need to do something about it, right? So with that in mind, when you are dealing with sensitive data in a Google Sheet, automatically the Share button will turn into a shield icon, implicitly reminding the user that you are dealing with a sensitive content. And added to that, data loss prevention policies are there, which can prevent you from sharing sensitive data externally, be it intentional or unintentional, right? Intentionally, someone would want to share it as a leak, or unintentionally, someone is just trying to download their data or share it to their personal email so that they can go home and work from home or work while they are traveling or sitting in a park supervising their family. So unintentional or intentional, any common use cases can be protected using DLP policy. And with Advanced Protection Program, it adds another layer of security for all incoming emails and outgoing emails that prevent any malicious content from getting into the users. There is the Security Sandbox that gives you the capability of detonating an email even before it reaches your inbox or even your domain, right? So these additional layers of defense within your email path gives you a whole layer of protection. And with all these context aware access, you can add more access controls using multiple attributes such as IP addresses, geolocation, which device someone is logging in from. So that's protection. And when we talk about detection, as I said, Google has about eight products with over a billion monthly active users. So the scale of the data that we see, the security signals that get generated by this, it allows us to create a better machine-learning model so that we can automatically identify and protect against these sophisticated attacks. Talking about 10 million spam messages that are prevented every minute from reaching Gmail customers. This breadth of security signals that Google has collected, we don't just keep it to ourselves. We are part of the BeyondCorp Alliance, so we do share it out with other internet security agencies who are working with us so that we can keep the entire internet safe for all of us. And detection and response. When we talk about finding a problem, Google has a Security Center in Workspace and it also has a Security Command center in GCP that helps you detect a problem, remediate this, and create further alerts for the future so that you can be prepared when such things happen again. And with Google Workspace, you also have Google Vault that helps you retain data for any of your e-Discovery and legal needs.

### Video - [How Google Workspace sets the foundation for security](https://www.cloudskillsboost.google/course_templates/502/video/490332)

- [YouTube: How Google Workspace sets the foundation for security](https://www.youtube.com/watch?v=FqF8wh_R5JY)

Rancho Iyer: So let's talk about how Google Workspace sets the foundation. Google Workspace has evolved over the years so that we can truly address large enterprise domains and large public sector domains. We have a whole lot of public sector, city-state, local counties. We have federal agencies who are using Google Workspace. And what we have found is this baseline commitment on privacy, ownership and compliance that we have set, that has provided the trust for our customers. No ads ever. You cannot see any ads in Google Workspace. That proves that we do not collect, scan or use any of the data that you use on your Google Workspace for advertising purposes. And you are your owner of the data. You have the ability to add another layer of encryption with client-side encryption keys so that you can protect your data however you want it to be. And helping you meet your compliance needs, we are currently FedRAMP high for Workspace, and it is also running in our Google Cloud infrastructure, which, by itself, is also certified as FedRAMP high. We are also HIPAA compliant, and we have all the settings that are required to comply with GDPR, ISO, and SOC controls. Talking about users, we have about three billion users using Gmail, four billion devices that are protected with Google's Safe Browsing technology. With this level of scale in data, we have seen that users are very familiar with the product, and the end user experience is much more elevated than what they are used to. So the amount of time that you have to spend in training your users or even learning the evolving product is much more reduced than before. With all our feedback from our existing customers, we've seen that no amount of-- no amount of change management can please them, but when we go from any on-prem solution to Google Workspace, there is an increased amount of adoption, and it decreases the amount of support requests that come after moving to Google Workspace. So this gives you evidences on how it reduces the admin overhead so that you can focus your energy towards meaningful initiatives for your agencies. Titan Security Keys, which is also part of the Work Safer program, and it is included when you go for the Work Safer program, this Titan Key is FIDO approved and it acts as your multi-factor authorization. We do have other options, such as SMS, text messages, phone calls, but we've seen hijacking attempts across those and bad actors intercepting those SMS messages. But when Titan Keys, which are FIDO approved, are rolled out, we've seen zero hijacking attempts on that.

### Quiz - [Quiz: Cloud-first, zero trust cybersecurity with Google Cloud](https://www.cloudskillsboost.google/course_templates/502/quizzes/490333)

#### Quiz 1.

> [!important]
> **When a user logs into Workspace, Google assumes breach and focuses on detection and response. This is an example of which Google core security tenet?**
>
> - [ ] Protect Everything.
> - [ ] Trust Nothing.
> - [ ] Secure Encryption
> - [ ] Detect Everything.

#### Quiz 2.

> [!important]
> **Most of your company is working from home, which has increased the risk of cybersecurity attacks. How does Google Cloud ensure that your domains are secured?**
>
> - [ ] Google Workspace is combined with Chronicle and Crowdstrike to provide optimum protection.
> - [ ] Employees can only access sensitive information when they are in office.
> - [ ] Google Workspace permissions are enhanced when employees are working from home.
> - [ ] Only some services in the Google Workspace suite are available when working from home.

#### Quiz 3.

> [!important]
> **The Work Safer approach uses which of the following security products?**
>
> - [ ] IAM, Chrome Enterprise, Titan Security Keys, and reCAPTCHA.
> - [ ] Crowdstrike, Two-factor Authentication, IAM, and Beyond Corp.
> - [ ] Google Workspace, reCAPTCHA, BeyondCorp, Titan Security Keys, Chrome Enterprise.
> - [ ] reCAPTCHA, Chronicle, and Two-factor Authorization.

#### Quiz 4.

> [!important]
> **Asset and device management within Google Workspace helps you during which phase of the Security and Resilience framework?**
>
> - [ ] Identify
> - [ ] Respond
> - [ ] Protect
> - [ ] Detect

#### Quiz 5.

> [!important]
> **What was one of the first actions initiated to improve US cybersecurity?**
>
> - [ ] Palo Alto Networks
> - [ ] BeyondCorp Enterprise
> - [ ] BigQuery
> - [ ] Chrome Enterprise

#### Quiz 6.

> [!important]
> **Which is a Google commitment to data privacy, ownership, and compliance?**
>
> - [ ] Google handles all compliance requirements.
> - [ ] Google controls your data.
> - [ ] You own your data.
> - [ ] Ads are displayed only if you give Google permission.

## BeyondCorp and reCAPTCHA

This module introduces two components of WorkSafer: BeyongCorp and reCaptha, and shows how they are used to counter threats.

### Video - [Introduction to BeyondCorp](https://www.cloudskillsboost.google/course_templates/502/video/490334)

- [YouTube: Introduction to BeyondCorp](https://www.youtube.com/watch?v=hxfK5NujSQs)

Rancho: Moving on to BeyondCorp Enterprise, we've heard this BeyondCorp Enterprise in several other meetings and blog posts and announcements, right? So let me start with what it's not. It is not just a Chrome extension. It is not just a security for Workspace. It is not just something to secure your access for the web apps. It is a complete, true, zero-trust access solution that provides access to applications and cloud resources with integrated threat and data protection,. So why is this relevant? It's because your users, whether it is the end users, the devices they are logging in from, and any other third-party applications that are accessing your work-- accessing your GCP or Workspace apps, you can now make sure they go through BeyondCorp access policies so that they get evaluated with zero trust. And it's monitored so that it goes through a no-VPN access. And it opens up access for only the application that the user is allowed to access. So it handles not only the authentication, but also the authorization, along with your policies that you decide. The policies could be anywhere from creating IP address regulations, geolocations. Say someone is going on a vacation. They are going to Europe or Antarctica. You can prevent them from accessing their work data from their mobile devices or from their work laptops. That adds another layer of security to make sure the devices your users are traveling with, it doesn't go into a bad actor. This BeyondCorp Enterprise has been designed so that it can give you that whole trusted cloud experience, and it relies on the three pillars, the transparency, and sovereignty. We make sure that you have complete control towards your data. You can create your access layers. And you can enhance them whenever you want it to be. You can diversify your access to a smaller subset of users instead of your entire domain. So that's transparency, sovereignty, giving you verifiable controls, and it gives you the zero-trust architecture so that you can focus on detection and response. And it also comes with a shared fate. So going beyond shared responsibility, we make sure that there is this shared fate so that we have an active stake in your security outcome. So this brings in BeyondCorp, which is the modern zero-trust platform, that is proven, scalable, and reliable.

### Video - [BeyondCorp Architecture](https://www.cloudskillsboost.google/course_templates/502/video/490335)

- [YouTube: BeyondCorp Architecture](https://www.youtube.com/watch?v=md9QtqnWVWo)

Rancho: So how are we doing this is we make sure that this scale piece is our agentless approach. So no additional software is needed. That is the first question that I always get from a customer. How easy is it to do it? Well, it is not difficult at all. You don't need any additional software. BCE is delivered through Chrome browsers, which supports over 2 billion users currently, and it's growing every day. And reliability means that you can work reliably from anywhere with 144 edge locations over 200 countries. We can completely cover your network base. And it's proven to absorb all the DDoS attacks, which we have seen from [INAUDIBLE],, South Africa, all over the countries. And talking about BeyondCorp, as I mentioned, we make sure that all these data points and security signals that we have collected so far, these attack patterns, we can constantly update our ML models so that we can better protect our customers. We just don't stop there. We also talk to the broader ecosystem and how we are democratizing the whole 0 trust so that for the larger goodness of the world, we want to keep internet safe and secure. And we know customers don't operate in just a one-vendor world. As we are venturing on multiple operations and digitizing our whole process, we know customers want to use multiple options. And that's why we leverage our existing environments and share the signal information with our BeyondCorp Alliance and make sure it's easy for you to enable policies based on that. So how easy is it to deploy? The good news is that the deployment of BCE does not require a complete overhaul of your environment. No, no, no. It can be deployed as a no-impact overlay that can completely either replace your existing VPN. It doesn't require any VPN. We can make this a reality without disrupting your operations. So at this point, if you are curious how this works or if you are interested to try it out yourself, please do reach out to your respective Google sales managers. We would be happy to walk you through the whole process of how it looks like. In simple words, the context of our axis, this is a high-level architecture of what it looks like. Your right side or my left side is all employees, contractors, part-time workers, partners you work with. They can access all the applications that you need to grant them access to, whether it is Google Workspace or any applications hosted on JCP, whether they are hosted in any other web applications or even on-prem applications or other third party SaaS applications. So imagine using Zendesk or ServiceDesk or Salesforce or Workday, whatever that is. You can integrate that and keep BeyondCorp as your foundation to pass through all your access policies. So users who are leveraging your network, they don't have to use any proxy traffic, and we eliminate the need of having a VPN by that. So how are we protecting the extended workforce? All of these sound brilliant, but what does it look like for the end user? So this screenshot literally shows you what it looks like for the end user. It's a tiny icon that sits on your Chrome browser that makes sure that you have the BeyondCorp protected profile. And that is this endpoint protection that makes sure your users, even if they are logging in from an unmanaged devices without the need of a VPN, they are still securely authenticated and allowed to use your apps. So this new and revamped Chrome profile experience, it makes sure that your users can separate their work profile from their personal browsing, and they can access their data wherever they want it to be. So another important use case for protected profiles is for remote workforce, so not only for people who are working in your hybrid work environment but also those that are still traveling or working from field offices or other locations. And those that need to use their own devices, bring your own devices or personal devices or contractors, you can still add them to these beyond core policies and grant them limited access or whatever access that they need. So this is the extended architecture of what it looks like while they are using BeyondCorp with no agent or VPN, no proxies. The concept of data loss prevention gets extended to any app, whether it is hosted on Google or elsewhere. So it gives you the true experience of accessing and executing their applications wherever they are, any device, any users anywhere.

### Video - [reCAPTCHA overview](https://www.cloudskillsboost.google/course_templates/502/video/490336)

- [YouTube: reCAPTCHA overview](https://www.youtube.com/watch?v=rFZKHrRyaAM)

Rancho: Moving on to reCAPTCHA. How familiar are you with this image, right? We've all seen this over the years when we access any particular random website and trying to log in. You would enter all the information, and then there is the reCAPTCHA with skewed image asking you to pick stuff, right? ReCAPTCHA Enterprise gives you that frictionless security for your website so you don't have to look through all these grids and select images that match what it's asking for. So why are we talking about this, right? Any agency, whether it is public sector, any public office appointments, or any other login for the wider public, right? Or any other customer that we are dealing with, there is always a need of hosting a website which opens up for non-Google customers or end users to log in and do stuff. And with this distributed work environment-- I have to stress on that-- people are so distracted that they end up clicking on random things, they end up doing a typo on the website URL, and the page opens up into a hacker or a phishing website, and they enter sensitive information, right? It could happen to anybody when someone is nagging right beside you while you are trying to get work done, right? It is in our latest market research, we've seen that bot attacks have increased 84%. And over the past two years with all this pandemic going around us, 65% of our customers have said that they have seen an increase in this attack. So not only are these attacks resulting in revenue loss, in having to mitigate this, or they have to change something in their website to prevent such attacks, talk about the mental well-- mental health, right? The torment that you have to go through in fixing this, the stress that they have to go through in fixing this, the time that gets spent in resolving the attack, all of that are hurting quite a lot. So considering all that, we want to make sure your reCAPTCHA experience is seamless and it still gives you the best-in-class protection for your website. And this is provided with reCAPTCHA Enterprise. The evolution of reCAPTCHA, what we've seen in the past is having those skewed words where you can type. That was version one. And then we changed it to make sure that you can click on inboxes that had traffic signals, or crosswalks, or trucks, or dump trucks, and all that, construction trucks. And with version three, we made sure that it came up with a behavioral analysis, so that it's more frictionless user experience. This is better for the users, they don't have to pick anything. You are asking the user and you are basically enabling reCAPTCHA to detect fraud by comparing all manner of transactional behavior. And reCAPTCHA Enterprise is adding another layer of unique capabilities so that you can push this functionality for mobile devices as well. And also, it uses extra granular scores and reason codes for these high risk are also made visible so that you can fine-tune your risk analysis and make sure your website is still easily accessible for users, and removing all these hurdles they have to go through for logging in, right? Doesn't that feel nice that you don't have to do that? Google does it for you behind the scenes. ReCAPTCHA Enterprise service helps you detect abusive traffic on your website without any user friction. Using a score-based detection system, you can rest assured that the website that you are opening it up for the wider public, it relies on data about online activity, and it stops bots and any other automated attacks. And this reCAPTCHA is also included in Work Safer program if you choose to go for the entire use case.

### Video - [Introduction to Chrome Enterprise](https://www.cloudskillsboost.google/course_templates/502/video/490337)

- [YouTube: Introduction to Chrome Enterprise](https://www.youtube.com/watch?v=BlIaRq4Zkro)

Person: Chrome Enterprise, it gives you that true endpoint security for your devices and browsing. When we talk about endpoint protection, Chrome also prevents eavesdropping and tampering of websites. So using Safe Browsing mechanism, it makes sure that data that users are uploading into Chrome are valid. And users who are downloading data are also not that sensitive. And you can make sure that your Chromebook has device encryption enabled. So even if it gets lost, nobody can do anything about it. You can have a whole lot of functionality pushed through your browser management.

### Video - [Demo: BeyondCorp](https://www.cloudskillsboost.google/course_templates/502/video/490338)

- [YouTube: Demo: BeyondCorp](https://www.youtube.com/watch?v=qPcVmsJmKvg)

Rancho: So at this point, let me actually show you what it looks like. I'm moving the screen here and going into some details. This is BeyondCorp's context-aware access and what it looks like for your Workspace access. So when you create your access level, you have the option of-- let me blow up the screen a little bit so you can see better. There we go. So you can use your geographic location, IP address, any device policy, what type of devices they are logging in from. And then you can frame your access based on that and issue this access on a subset of users or a subset of applications. Similarly, when you see such alerts that come in saying that there is a suspicious login noticed, what would an admin do? What am I going to do with this information? What should I do? So here it is. Google not only gives you an alert about suspicious activity, it gives you more details whether this is OK, some action needs to be done, what is the alert history looking like, is this a repeat offender? So when I click on the View Virus Total Report, it's going to give me more patterns about this IP address. Is it a bad actor? Is this actor repeatedly attacking my domain? So this gives me more data points so that I can act upon it. And when I go into my Domains Chrome browser Device Management Settings, you see here, there is a whole lot of device management settings available. And when I go into my Chrome browser, I can actually do content analysis of what type of content is being downloaded or uploaded. I don't care what they download, but I want to make sure that my work data never gets uploaded elsewhere. So you can actually prevent people from uploading sensitive content that has confidential keywords or sensitive data. And you can also throw in a custom warning message. You can check for malwares, if they are downloading something. And you can also prevent people from uploading any password-protected files or any files that are larger than 500 MB. So there are granular patterns available for download content and upload content as well that gives you a true BeyondCorp Chrome browsing experience within Workspace. And even if not Workspace, if they go into any random URL, you can also use that real-time URL check to make sure that it is not a malicious URL or a bad actor.

### Quiz - [Quiz: BeyondCorp and reCaptcha](https://www.cloudskillsboost.google/course_templates/502/quizzes/490339)

#### Quiz 1.

> [!important]
> **Which applications can you grant employees, contractors, and partners access to with BeyondCorp?**
>
> - [ ] Zendesk.
> - [ ] All of the above.
> - [ ] Google Workspace.
> - [ ] Workday.

#### Quiz 2.

> [!important]
> **Your organization has apps that are accessed by third parties. You need to make sure that the third parties are evaluated using the zero trust architecture. What Workspace security feature ensures secure access to apps and resources?**
>
> - [ ] Authentication Manager
> - [ ] BeyondCorp Enterprise
> - [ ] Zero Trust Enterprise

#### Quiz 3.

> [!important]
> **How does Google ensure that BeyondCorp is scalable and reliable?**
>
> - [ ] The deployment process is robust, providing enhanced security.
> - [ ] It's agentless, meaning no additional software is needed.
> - [ ] It's accessible to everyone.
> - [ ] It's applicable for almost any Workspace security use case.

#### Quiz 4.

> [!important]
> **What is one benefit of using Chrome Enterprise to prevent suspicious web activity?**
>
> - [ ] Continuous and automatic updates, with no security patching required.
> - [ ] Protection against data loss.
> - [ ] It ensures clear separation between work and personal activity.
> - [ ] Tools for meeting compliance standards.

#### Quiz 5.

> [!important]
> **Your extended workforce needs to access corporate resources. You need to make sure protection is provided and that there is clear separation between work and personal activity. What is the benefit of using BeyondCorp to achieve this goal?**
>
> - [ ] BeyondCorp is not run through the Chrome Browser.
> - [ ] BeyondCorp opens in an incognito window in Google Chrome, to ensure that there is separation between work and personal activity.
> - [ ] Because a VPN is required, access is more secure.
> - [ ] Your extended workforce can access the apps and resources they need without the need for a VPN.

#### Quiz 6.

> [!important]
> **BeyondCorp can cover which of the following endpoints? (Choose 2)**
>
> - [ ] Mobile Phones
> - [ ] Nest Camera
> - [ ] TV

#### Quiz 7.

> [!important]
> **Which Work Safer solution gives you the best protection for your website?**
>
> - [ ] ReCAPTHCA Enterprise
> - [ ] Chrome Enterprise
> - [ ] Chronicle
> - [ ] BeyondCorp

### Lab - [Securing Cloud Applications with Identity Aware Proxy (IAP) using Zero-Trust](https://www.cloudskillsboost.google/course_templates/502/labs/490340)

In this lab, you will deploy a sample application and enforce the access restriction capabilities using Identity-Aware Proxy.

- [ ] [Securing Cloud Applications with Identity Aware Proxy (IAP) using Zero-Trust](../labs/Securing-Cloud-Applications-with-Identity-Aware-Proxy-(IAP)-using-Zero-Trust.md)

## CyberSecurity with Chronicle, Crowdstrike, and Palo Alto Networks

This module explores different tools and products available to counter cybersecurity threats.

### Video - [Chronicle](https://www.cloudskillsboost.google/course_templates/502/video/490341)

- [YouTube: Chronicle](https://www.youtube.com/watch?v=fhPU75FdYgI)

Rancho: Cybersecurity-- we spoke about Google Workspace, reCAPTCHA, hosting data in Google Cloud platform, and what is Chronicle, and what are the cybersecurity solutions available. Chronicle is a petabyte-scale security analytics platform that gives you the true detection of modern threats. Whether you are investigating to scope out the problem or finding the root cause of a threat, you can use Chronicle for all of these analyses. You can feed your workspace data into Chronicle and can blow up analytics for you that can be actionable at a later point. Talking about Chronicle, it's Google's modern cloud-native platform that helps you detect, investigate, and respond to threats. And all of this is done in an unprecedented speed and scale which makes this truly remarkable and valuable when you add it with Workspace. Chronicle was built a few years ago within Google. It's a solution that helps our customers modernize their SOC. And the first layer of security information and event management is data layer. Chronicle ingests your own data into a private container, such as network alerts, any DNS details, EDRs, other useful logs. And it ingests a variety of other security heuristics and patterns that we have and makes sure you can have an analytics data presented that actually makes sense out of it. And finally, the data is exposed to you via our investigation hunting and detection capabilities so that you can make sense out of it and you can get some action items out of it. And talking about Chronicle, what we truly solve is it's cloud native, and it is at a fixed cost, and it gives you those clear signals that you can use for enrichment and activities that come out of these threat detections. With Workspace, you can have better investigation and response. So you do have Workspace coming with Security Center that helps you with Investigation tool and Alert Center. But feeding those logs into Chronicle is going to give you that additional layer of detection response across a whole layer of footprint, not only just Workspace but also your other applications. So Chronicle can not only pull logs for your workspace but also for other applications. And you can truly have that one place to see everything, detect everything, and respond quickly. This is Chronicle, then its whole expanded portfolio of security telemetry that it can generate out of your Google Cloud portfolio. So that means your endpoint data, network data, cloud data, all of that is visible. It includes alerts-based events from all security tools, and everything-- it will help you make sense out of what are the actionable ones and what are sort of suspicious, what we'll have to look at patterns for further.

### Video - [Google Cloud and Palo Alto Networks](https://www.cloudskillsboost.google/course_templates/502/video/490342)

- [YouTube: Google Cloud and Palo Alto Networks](https://www.youtube.com/watch?v=xKGo01PadSw)

Rancho: Palo Alto Networks-- so switching gears a little bit, we saw about the Google portfolio of products. And then, what are the additional products that can add value towards your Work Safer program? One such is Palo Alto Networks with this end user Cortex XDR which is a client that's going to live in your users' devices. It gives you another layer of protection against endpoints that are connecting, whether it is files that are saved, preventing those files from going into Google Drive, or preventing any other ransomware attacks or threats or malicious content that are sitting in on your files, or any other executables that get accidentally downloaded. All of that can be blocked and prevented using this additional layer of security. So how does this add or work in conjunction with Workspace or GCP? Let's look at a sample architecture of what it looks like. So your left side with Workforce and your right side with your applications, BeyondCorp forms your central point of axis definition. And Cortex acts as your additional layer that gives you more security towards protection of multiple endpoints. This Cortex XDR is a client that works on your computer. Whereas, if you want to look at other SaaS-based protections, they do have SAS Security API, which will help you use their API to protect your applications that are hosted elsewhere or on on-prem. So if this is something of interest, we are happy to get you connected. This is one small component that brings in the whole Work Safer experience. And how it gets applied, we can see in the upcoming slides about use cases.

### Video - [CrowdStrike](https://www.cloudskillsboost.google/course_templates/502/video/490343)

- [YouTube: CrowdStrike](https://www.youtube.com/watch?v=B7PVNK1J8nk)

Rancho: All right, moving on to Crowdstrike-- so this is another complimenting solution that gives you a similar endpoint protection. So we've seen customers, some of them are using Palo Alto, whereas some of them are using CrowdStrike. So whichever that you are comfortable with, both are included in the Work Safer program. The ultimate goal is to secure endpoints. And you need to provide dedicated capabilities to protect them as well as detect and respond. So if your domain is not using Chrome OS, Crowdstrike is another industry-leading solution you could consider. Specifically the Falcon Platform provides a full comprehensive solution for your endpoint protection, delivering that whole prevention, detection, and response, the whole nine yards of security capabilities, and all of that in a lightweight agent because we don't want to be weighing down on the computers that you are running this on. So this makes sure-- [COUGHING]---- it continuously monitors the activity on the endpoint. It captures events in real time for local analysis. And you can also keep track of the graph of activities over a period of time. So this gives you a complete pattern. And you can exploit the data for further planning of security changes on your end.

### Video - [Work Safer Use Cases](https://www.cloudskillsboost.google/course_templates/502/video/490344)

- [YouTube: Work Safer Use Cases](https://www.youtube.com/watch?v=1hxMSSwj8B0)

Rancho: Another one-- so summing this all up is Work Safer program-- we spoke about CrowdStrike's Falcon Platform that can tie up with Workspace, BeyondCorp Enterprise, and Chronicle, giving you that true experience in a quick manner. So these are all the topics we saw on all these slides. Now let's look into what type of use cases that we have to go into. Whether you are working just with a frontline worker, whether they are a field worker-- or think about parks and recreations, the kiosk worker, an employee who lives in the remote part of a park where they are supporting it from. So those frontline workers, we want to make sure that all endpoints are secure. And for that, we would recommend using Workspace Enterprise along with BeyondCorp and supplying them with Chromebooks. This gives them that lighter work access that gives you complete resistance towards malware and other traditional attack vendors. And if you are talking about implementing zero-trust security where-- whether you are a CISO or in the IT department, if zero trust is on top of your mind, something we would like to look into is beyond implementing BeyondCorp Enterprise, look at rolling out Titan Keys. So adding Titan Keys provides that layered security solution with the strongest form of second-factor authorization. So this solution gives you a full sense of security and trust towards keeping your data secure. Further, if you are looking into adding some monitoring-- I just don't want zero trust, but I want further to know about proactive notifications, what is happening, and I want to follow up with everything. So for that, we would recommend adding Chronicle. And Chronicle as a destination for your rich telemetry generated from GCP or Workspace, and it gives you that traditional logs in a much more digestible fashion. It solves your problem with fixed-rate pricing as well. So Chronicle is also an open platform. You are not limited to just Google log types. You can load any type of logs from your on-prem applications and mix it all up and find out any bad actors or patterns from that. Looking into security and endpoint protection, when is this applicable? When you are talking about best-in-class solution with device insights. If you have people who are using multiple devices on a rotation basis or if you have people using any other third-party products much more frequently-- you are just using Workspace or you are just using GCP for your workloads, but you would like to use other solutions, as well, other local softwares, clients that you are installing. So in that sense, we recommend using additional layers. It could either be Palo Alto or CrowdStrike, so whatever that you deem best for your Windows or Mac devices. Given Palo Alto and Crowdstrike are both best-in-class, with Work Safer, it gives you that nicest solution to augment any of your existing SaaS tools. Another use case-- completely summing it up with end-to-end Work Safer. If you want to go the whole length, completely implementing everything in Google strategy and adopting all of the solutions, then this is something that we would highly recommend. Work Safer gives you the option to truly replace an on-prem solution with an end-to-end security protection and a whole CM solution for your threat detections as well. Due to the scope and complexity, this will probably be something that you are looking at, oh, this is too much or I don't want to rip and replace everything. But we can completely peel on all these layers and show you that all of these can be implemented with the least amount of disruption possible. So this gives you the whole end-to-end security.

### Quiz - [Quiz: CyberSecurity with Chronicle, Crowdstrike, and Palo Alto Networks](https://www.cloudskillsboost.google/course_templates/502/quizzes/490345)

#### Quiz 1.

> [!important]
> **Your organization needs to be sure all Workspace data is free of cybersecurity threats. What solution should you use to detect, investigate, and respond to threats?**
>
> - [ ] SaaS Security API
> - [ ] Cloud Audit Logging
> - [ ] Chronicle
> - [ ] Cloud VPN

#### Quiz 2.

> [!important]
> **Your organization needs to be sure all Workspace data is free of cybersecurity threats. What solution should you use to detect, investigate, and respond to threats?**
>
> - [ ] SaaS Security API
> - [ ] Cloud Audit Logging
> - [ ] Chronicle
> - [ ] Cloud VPN

#### Quiz 3.

> [!important]
> **How does Cortex XDR give end-users extra protection?**
>
> - [ ] Cortex XDR acts as the central layer of defense.
> - [ ] It prevents 100% of Ransomware attacks.
> - [ ] It's integrated with WildFire for malware detection.
> - [ ] Cortex XDR is faster than other solutions, so you can verify threats quickly.

#### Quiz 4.

> [!important]
> **You need a security solution that will scale with your data. How does Chronicle provide a solution to this challenge?**
>
> - [ ] Chronicle is on-premise and operates at scale and speed.
> - [ ] Chronicle is Cloud-native and operates at scale and speed.
> - [ ] The cost of Chronicle scales with your data.
> - [ ] Chronicle does not scale with your data.

#### Quiz 5.

> [!important]
> **What is the primary function of Crowdstrike?**
>
> - [ ] Video monitoring.
> - [ ] User authentication.
> - [ ] Protection against phishing attacks.
> - [ ] Endpoint protection.

#### Quiz 6.

> [!important]
> **An organization is looking to build their own Zero Trust Architecture. They use Google Workspace, and want to reduce the risks associated with log ingestion, missed threats, and lack of security expertise. What solution should the organization choose?**
>
> - [ ] Security and Endpoint Protection.
> - [ ] Secure Corporate and Frontline Workers.
> - [ ] Zero Trust Security.
> - [ ] Zero Trust Security + Monitoring.

## Assured Controls in Google Workspace

This module introduces assured controls and describes Assured Controls features and benefits. In addition, you'll explore Google's solutions for compliance.

### Video - [Introduction to Assured Controls](https://www.cloudskillsboost.google/course_templates/502/video/490346)

- [YouTube: Introduction to Assured Controls](https://www.youtube.com/watch?v=WmPxLp2JFv0)

Nicolette: Assured Controls-- what in the world is Assured Controls? So security has been at the core of Workspace since the beginning. We were G Suite. We were Google Apps. Since the beginning, security has been at our forefront. We are, as you all know, cloud-native, which means that we get all the security benefits from the best and brightest security engineers. And what this does is it ensures Google operates safely across our entire fleet. No matter whether you're using GCP, whether you're on Google Workspace, again, everyone is receiving the same security standards. For Workspace, security comes with no updates or patches. We're FedRamp High-certified across our cloud. Regardless, again, if you're a commercial customer or a public sector customer, you're on the same cloud, and the compliance and security features are there for everybody. So we don't separate that. Everybody gets those security features. With Assured Controls, we can enable that every user benefit from this the intelligence and collaboration of Google Workspace without sacrifice. So you might be saying, great, Nicolette, that's great. What does this look like in Google Workspace? So Assured Controls is something we launched last March to really help our positioning for the for-public sector because we have to meet those compliance and regulatory regimes. So Assured Controls is an add-on to Google Workspace. And what it does is it helps our customers control provider actions related to your data. So Access Management is that first feature that we released within Assured Controls. With future Assured Controls releases, we are going to give you more control over provider access. And I'll dive into that in just a few moments. But really, what Access Management does is it allows you to control which subsets of Google's staff can take actions related to your data based on specific staff attributes. With competing solutions, access to similar restriction capabilities is only available in GovCloud environment. So being native to Google Workspace means that you will have the opportunity to access all of the latest workspace features in conjunction with Access Management while avoiding the complexity and cost of managing a totally separate GovCloud. What does that mean for us? For us, as you know, we're on restricted-- you know, we're kind of restricted here, right? We want you to trust that-- we want you to trust Google with your sensitive data. And we're doing that by providing you Assured Controls.

### Video - [Google's Solution to Compliance](https://www.cloudskillsboost.google/course_templates/502/video/490347)

- [YouTube: Google's Solution to Compliance](https://www.youtube.com/watch?v=sXx2J4g69Dg)

Nicolette: So Assured Controls is Google's solution to compliance. Let's talk about that a little bit. How does Google actually comply with things? There's two questions to be answered here. One, where is my data located? OK, where is my data located? This is the first piece to address compliance. And we address this with data locations? So data locations focuses on the concept of keeping your data within the states, which is part of that CJI security policy. And Google is able to make this guarantee to you by providing you the option to choose where your data is stored within the Workspace Admin console. The second question is, who has access to my data? Who has access to my data really has two options here. You'll notice the first one is encryption, so our client-side encryption offering. And then our second option is Assured Controls. What Assured Controls really means is, one, access transparency; two, access management; and three, access approvals. So what Assured Controls is providing you is FBI-fingerprinted, background-checked individuals that your organization can pick from. So what does this mean? This means that we'll send you those fingerprint cards. You can review them. You'll approve those individuals, as well as execute a CJIS Security Policy with us to see what controls we have in place for both Workspace and GCP. I want to be very clear with that. We're going to do this once with you, and it's going to cover all of Google Cloud, Workspace and GCP. So whether you choose one or the other. Let's say you go down the Workspace path and then, later on, you're like, hey, I want to test out some items in GCP. You don't have to go through this whole process again. We're gonna do it one time. We're gonna get everything set the first time, and you'll be good to go. So we're meeting CJIS security policies at the point in time when you sign that addendum, and then we'll run through red lines with your attorneys and ours. But essentially, we execute that contract with you. OK. I do want to touch really fast on encryption because some folks do have questions about it. And Google calls this client-side encryption. This is another way to achieve this CJIS. Note, the reason why that Google rolled out Assured Controls is because client-side encryption sacrifices the collaborative experience and product capabilities that Workspace offers. So this is why we typically don't advise clients to go down this path, unless you have very strict additional requirements through CJIS because it does create a poor user experience. Meaning that the keys themselves, yes, you manage, you own them, but things like search or other features in Drive, they're not available. So that's why we chose to go down that Assured Controls path, which, again, we've been using in GCP for a while. So we brought that over to Google Workspace. And what we do is get access, again, to only those FBI-fingerprinted, background-checked individuals that you have authenticated and said are good to support you in the event of a support action. They're not just gonna willy-nilly access your data. Now, again, some of you, because we work in public sect and because we're always thinking about security, you're saying, well, what if? What if, Nicolette, in the event that somebody does access-- or you submit a ticket. What happens? You are routed to one of those pre-approved, FBI-fingerprinted, background-checked individuals. And in the event that we have to access your data, that individual that has that background check and fingerprint is the one who can access your data, which keeps you CJIS compliant. So when you look at those two components and the underlying NIST controls that you need to meet for that FBI mapping, we meet them for FedRAMP high and IRL4 for DoD. And essentially, we've mapped to them. I would like to note that when you sign and execute a CJIS addendum with Google, again, we perform the audit for Workspace and GCP at the same time. So just bringing that up one more time. You don't have to do it multiple times. In parallel, we'll start that background/fingerprint process, and we send those to you for review.

### Video - [Assured Controls Products](https://www.cloudskillsboost.google/course_templates/502/video/490348)

- [YouTube: Assured Controls Products](https://www.youtube.com/watch?v=gdKUODB-mTw)

Nicolette: Assured Controls products-- let's talk about this. There are three products right now. Access Transparency is our logging to customers and almost-real-time logging inside of your environment. So you can go into your administrator console, and you can see this right now, who has access to this. Keep in mind, this is for Enterprise+ SKUs. Access Management, like I said before, restricts those Google staff 24 by 7 to US persons in the US only. So that's kind of our litmus for public-sector regulations. Coming soon-- and I encourage you to keep attending our roadmap sessions because we talk about this a lot-- is Access Approval. So similar to Microsoft Customer Lockbox where any time administrative action is taken on customer data-- read, write, support, et cetera-- you actually have to say yes. So you have to give us the OK to go ahead and support you and access your data. Again, this really puts you in the driver's seat. So these three pieces provide a set of trust for you, so you can see what Johnny Smith who has been authenticated and approved by you, what action he did take to support you, et cetera. And if any-- if he did take any action outside of that and gives you-- it gives you the trust that Google's doing the right thing to support you.

### Video - [Scope of Coverage](https://www.cloudskillsboost.google/course_templates/502/video/490349)

- [YouTube: Scope of Coverage](https://www.youtube.com/watch?v=LZdzsbrDp-M)

Nicolette: Let's talk about the scope of coverage here. So your data has access controls around it. And in any event, let's say, for some reason, an EU-based support person was somehow stumbled in and tried to support your case, or they're supporting another case, and your data happens to be intermingled with that. That would be blocked. Essentially, we have the data access controls in place that check the adjunction attributes and also the desk location and the actual personhood as being in the US who has gone through, again, those US background checks, fingerprinting in your state. Our data access controls block on that. So that's how we're able to provide the guarantee to you and meet those CJIS security policy requirements. This is something that Google has worked very closely with the FBI on and one of the reasons why it kind of took us a little bit longer to get CJIS. Because this is a new way of supporting CJIS data. The FBI has never done it like this before because our competitors don't do it like this, right? Usually what would happen is let's say you store your data in a GovCloud. It's in a building. The vendor puts their people there with machine guns. They walk around with alligators or whatever the path is. At the end of the day, you are supposed to trust that. Google takes this many steps beyond. No matter where our data centers are, no one has access to them and to that data. And on top of that, the persons who do support you, we gate them. Essentially, we are providing you a more strict model.

### Video - [Implementing Assured Controls](https://www.cloudskillsboost.google/course_templates/502/video/490350)

- [YouTube: Implementing Assured Controls](https://www.youtube.com/watch?v=Qbn8iYY8WuQ)

Nicolette: So what does this look like? Assured Controls a surface as a simple one-click admin console policy for groups or users. So if you were to enable or add on a shared controls to your Google Workspace, you would see this in your Admin Console as-- in your Access Management. And you will be able to turn this on or off for groups or users. Access Transparency. Oh my word, I'm so sorry. That is a horrible slide. Let me walk you through this one. This is our logging to customers, again, in almost real time. You already have access to this in your Admin Consoles. If you go under your Audit Logs, there's an Access Transparency option there. So you'll already have access to that today for Enterprise Plus folks. Access Management, like I said before, restricts those Google staff 24 by 7 to US persons in US locations. So again, it's our litmus for public sector regulations. Access Approvals. OK, this is coming this year. It's on the roadmap, officially announced. This is, again, similar to Microsoft Customer Lockbox where any time an administrative action is taken on your data, you actually have to-- we put in a request and you actually have to say, yes, I approve this, or no, I do not approve this. So it puts you in the driver's seat.

### Quiz - [Quiz: Assured Controls in Google Workspace](https://www.cloudskillsboost.google/course_templates/502/quizzes/490351)

#### Quiz 1.

> [!important]
> **What does Assured Controls give you more control over?**
>
> - [ ] Cloud service provider's access to customer data.
> - [ ] User access to your data.
> - [ ] Workspace usage.
> - [ ] Customer access to your data.

#### Quiz 2.

> [!important]
> **With Assured Controls add-on feature, you can:**
>
> - [ ] Meet compliance requirements.
> - [ ] Control Workspace app usage.
> - [ ] Control access to the Google Cloud Console.
> - [ ] Approve administrative access to your Workspace data before it happens.

#### Quiz 3.

> [!important]
> **Assured Controls addresses which part of compliance?**
>
> - [ ] Data location
> - [ ] Encryption
> - [ ] Data retention
> - [ ] Access

#### Quiz 4.

> [!important]
> **How does Google guarantee that it meets policy requirements?**
>
> - [ ] Data access controls restrict access to only Google staff.
> - [ ] Security access is combined with data access for advanced protection.
> - [ ] Access transparency blocks individuals with a zero trust architecture.
> - [ ] Data access controls ensure that individuals have gone through proper background checks, and block individuals if necessary.

#### Quiz 5.

> [!important]
> **Your organization needs to make sure Google staff with administrative rights are background checked at all times. Which Assured Controls product achieves this?**
>
> - [ ] Access Approvals
> - [ ] Access Management
> - [ ] Access Transparency
> - [ ] Access Security

#### Quiz 6.

> [!important]
> **Where can you enable Assured Controls for your Google Workspace?**
>
> - [ ] Within a project.
> - [ ] In the Admin console.
> - [ ] In the Assured Controls Hub

#### Quiz 7.

> [!important]
> **What are the two questions that need to be answered to address CJIS data?**
>
> - [ ] Who can share my data, Where is my data located.
> - [ ] Where is my data located, Who has access to my data.
> - [ ] Who has access to my data, Who controls my data.
> - [ ] Who controls my data, Who can share my data.

## DDos Mitigation

This module shows how Google Cloud Armor can be used to counter DDoS threats.

### Video - [Module Introduction](https://www.cloudskillsboost.google/course_templates/502/video/490352)

- [YouTube: Module Introduction](https://www.youtube.com/watch?v=7nzi5uUog2o)

Haider: Good morning, afternoon, everyone. My name is Haider Witwit. I'm a Customer Engineer Networking Specialist supporting the Global Public Sector Organization here at Google. I've been with the Google team for a little bit over two years now. Prior to that, I was an individual solutions architect doing something similar with respect to supporting public sector for close to six years there. And prior to that, I was a full-time network engineer. So my experience really goes across the board with a hands-on experience and Cloud experience. My role usually around enabling customers, understand the platform capabilities, design solutions in the Cloud that meets their security requirements, and help customers usually on each step on the way. Our session today, as John mentioned, is about DDoS mitigation. So we're going to go over the capabilities provided by Google Cloud platform to mitigate attacks-- distributed attacks that are targeted to bring down systems and applications by exhausting resources that serve these applications. We have one hour targeted for the session. I know we have some larger windows so that we can cover other stuff. But I think we should be good to continue These Conversations Until 1:30-- 2:30, I'm sorry, Eastern time zone if there are any active conversations for us to have. A little bit heads up. This is a technical content. And because it's a learning series, I like these sessions to be interactive. So feel free to post questions in the chat window. I will also take pauses during the session to take a sip of water and maybe open it up for questions. If you have-- at any point, if you feel you have a burning question, feel free to unmute yourself and shoot the question. I'll do my best to take those as we go along. From an agenda perspective, we will start by going over the network security model with Google Cloud. And then, we can focus-- have more focus on Cloud Armor as a product focused on our positions to address DDoS mitigation. We are going to cover capabilities available today by Cloud Armor. We are going to go over what was launched recently to improve our security model. And around the end, we will explain the logging and monitoring and capabilities that are sent or generated by our systems and where you can find them in Google Cloud.

### Video - [Cloud Network Security Overview](https://www.cloudskillsboost.google/course_templates/502/video/490353)

- [YouTube: Cloud Network Security Overview](https://www.youtube.com/watch?v=YMv39jOFSFU)

Haider: So let's start with an overall network security model. And usually, the way I like to explain that concept is by going over the location or the access model for your services at Google. And primarily, there are two levels to discuss. The first one is what is provisioned within a VPC network. And VPC, as we know, is that virtual private space that you can configure in the cloud. You assign it IP addresses. You control routing rules for who can talk to who. That's one place. Other place, usually, is, you know, Google-- like Google Public Backbone or a place where we host our usually managed services. With examples for, you know, that level of public APIs or BigQuerys or Google Cloud Storage service. Good examples for VPC network, so what the provision inside your VPC networks are services that usually aligns more with the infrastructure as a service model like VMs, Google Compute Engine machines, or GKE clusters. Then, of course, with the VPC networks, because you have control over routing, you can enable private routing to your on-premises environments. And you have routing rules to control access to and from public networks over the internet. So the first security control to explain here is a VPC firewall. And this is a stateful layer 4-- layer 3, 4 firewall capability that's going to allow or deny traffic based on source IP, destination IP, or source or destination port. Firewall rules can be used to allow or deny traffic between resources in the same VPC. Networks are trying to access your resources over interconnect or over these hybrid connections, interconnect or VPN, or from the internet. So VPC firewall rules is the-- is the first security control. The second security control is a VPC Service Controls. Service Controls is service that was specifically designed to address data exfiltration concepts. And the idea here is you as a user or as an owner of an application on Google Cloud will be able to create a boundary for your application. And data can be moved freely within this boundary. But any call, even if it was an authorized call, meaning an API call with a user-- agenda user who is using their agenda IM credentials-- these calls that are aimed to transfer the data outside of this boundary will be denied. So Service Controls typically used to, you know, maintain the data within this boundary that we explain, no matter if the call or if the data sits in-- [INAUDIBLE] Services as part of your VPC or Managed Services at BigQuery and Storage Buckets. And you know, it can include the calls coming from on premises or from outside of the internet. Cloud NAT is another control that we provide. And Cloud NAT is really positioned or designed to enable public access-- public egress access for resources-- for private resources that does not need public IP addresses. Next control is Cloud IDS, Cloud Intrusion Detection System. And this is a native idea system that's provided by Google powered by Palo Alto Networks. And with Cloud IDS, you'll be able to get threat intelligence data about communications within your VPC environment and take actions based on the findings of that system. We also have packet mirroring, which is a capability to mirror traffic from a subnet or from a machine and send this packet-- the middle data to a third-party sensor that are provided by our partner networks. And at the end, we'll talk about Cloud Armor, which is the focus of our session today as the last control [INAUDIBLE]. . Cloud Armor and Identity-Aware Proxy are advanced layer 7 capabilities that are positioned to deal with web traffic. So now we're moving away from layer 3, layer 4, getting all the way up to layer 7 of the OSI portal, where we discuss, you know, capabilities that will break down the web traffic and look into the contents for inspection. IAP is an important piece of our zero-trust strategy and our BeyondCorp model.

### Video - [Google Cloud Load Balancing](https://www.cloudskillsboost.google/course_templates/502/video/490354)

- [YouTube: Google Cloud Load Balancing](https://www.youtube.com/watch?v=SQdrGl0F22Q)

Haider: Because Cloud Armor, as explained earlier, integrates really with your load balancer, the global load balancer, it's important to cover at a high level what is a model or model for external load balancers. And in brief, external load balancers are a fleet of highly available and scalable web load balancers that are provisioned at the edge of Google network as close as possible to the user. So this positioning will give it a global axis represented by a single anycast public IP address. This public IP address can be accessed from anywhere. And because our VPCs are global-- Google VPCs are global-- we enable the customer or the app owner to design or to provision backends that support that application in all of the regions they feel that they have presence in that area to minimize latency. So the idea here is that we have a single load balancer, virtual IP address we call short by zip. This is a 200 IP address. You access this IP address and depends on where you coming from, your request will be directed to the closest backend service. And because it's deployed on the edge, this is going to be, as I said, as close as possible to the user to maintain the latency and enhance performance. With the positioning of the load balancer service and the capabilities of SSL offloading, this is going to enable the TLS everywhere more than we are trying to encourage here in Google Cloud. And the idea, in brief is, because my load balancer is really close to the user, I'm going to enable HTTPS offloading-- SSL offloading using Google managed keys or customer-provider keys. Strengthen that in addition to the SSL offloading with SSL policies that will be configured by the user to control who-- what are the levels-- the minimum levels of SSL encryption supported. Those are needed to maintain compliance requirements that sometimes have limitations around the minimum version for SSL encryption, for example. And we'll take that on the load balancer level. So now, we have encryption from the user to the load balancer. And then, everything between the load balancer to the back end will be routed over Google backbone that encrypts all the traffic by default. Of course, for this last piece of the load balancer to the backend, we can take care of the encryption by Google Managed Keys or the customer can use customer managed keys if they want to configure HTTPS traffic between these two-- the load balancer and the backend service. This is all configurable by the user. But by default, it will also be encrypted even if the customer is using HTTP traffic only, meaning the back end is listening to not encrypted backbone data. But that's still encrypted by Google backbone.

### Video - [Google Cloud Armor Overview](https://www.cloudskillsboost.google/course_templates/502/video/490355)

- [YouTube: Google Cloud Armor Overview](https://www.youtube.com/watch?v=K-1ki1Myy5A)

Haider: So Cloud Armor is going to fit into this picture by building integration with our external load balancer to build protection as close as possible to the user. Cloud Armor and external load balancer as a reverse proxy layer will provide protection starting from layer three of the OSI model all the way up to the layer seven by adding capabilities to create security policies on the inline traffic to allow, deny traffic, create geo based filtering. They have built in WAF rules that we're going to explain later in the session, and are creating custom rules that best match the access requirements of the application. So now let's get into more details of Cloud Armor. But before I go to that, is there any questions, John, that came through the chat or anyone who feel the need to interject with a quick question? John: No, no questions as of yet. Haider: Cool. Cool. So Cloud Armor is the focus of our session today. And Cloud Armor is our solution to address data mitigation concepts. The capabilities you'll get with Cloud Armor varies. First capability is that layer three, layer four attacks are disabled or are blocked by default by the load balancer, because the load balancer is a reversible proxy tier, which means that only well-formed TCP connections will be able to pass through the backend, your backend, your instances, your buckets, your serverless environments. So you're doing that on the edge level before even the traffic is routed over Google dashboard. In addition to that, we have capabilities, as I mentioned, where you can filter based on IP networks or certain IP addresses. This is good for IP whitelisting, geo-based filtering where we have situations where the application, this application only needs to be accessed from certain geo areas. Or we have situations where I have some high risk countries in the world that what I need to quickly create a rule to block all of the traffic from this country, and of course, advanced rule based on custom expression language that supports variety of rules to match and then actions to take in on the match traffic. In addition to that, we have OWASP rules. These are built-in rules in Cloud Armor that customers can enable and tune based on their application requirements. And it's as easy as creating a basic rule to enable the evaluation of that preconfigured rule. And eventually, as with any really security practice data, looking at the data, evaluating the logs is always important. And we have rich metrics provided by Cloud Armor for the customer to view. And we try to minimize the actions needed by the customer by building features that we can explain during the session today. So policies-- I said Cloud Armor is going to give you the capability to create security policies between the load balancer and the back end. So these policies, the structure of these policies is really straightforward. Policies will have rules. These rules are processed in the order they are configured. So they have different priorities and based on the lowest priority will be processed first, although going down to the default rule, the default rule is the last rule that gets evaluated. And it's configurable by the customer, whether it needs to have a default allow, like allow all or deny all. And this is based on environment, if this is a lock down environment or if it's an open environment. What that means is that let's say you have a public website and you want to have a default allow rule. But before that, you create multiple rules to filter out the possible attacks. But if the match traffic is not a possible attack, then allow all traffic. On the other side, you have more restricted environments where you may want to set a default deny rule and only create rules before that to allow legitimate traffic. And this will be based on advanced IP headers or source networks that generate the traffic. So the service is also flexible to support both models. Now, these policies, as I said, they will be configured and they will be assigned to a back end. A policy can be assigned to more than one back end, but a back end service can only have one policy at a time. So to explain what's in the rule itself, you'll have a condition. And a condition can be as easy as an IP address or can be a complex condition where custom expression language will be used. We'll give examples for these custom expression languages, common examples. If a condition is matched, an action will be taken. And the action can be allow, deny, or as we recently added, we can throttle the traffic or you can create a temporary ban or you can redirect to a [INAUDIBLE]. We can explain those features in more detail during the session today. Priority, as I said, rules are processed in a certain priority. And the rule itself, it can be enforced or in preview. As a best practice with WAF and any DDoS [INAUDIBLE] technique that will enable you to create that level of custom rules, it's always recommended to put things in a preview mode first where the rule is in place but it does not enforce the action. And the goal of that is that you will collect data to make sure that you are not blocking legitimate traffic first before you start enforcing the rule. So taking that window depends, of course, on the application requirement, depends on your team that's reviewing this information. But the preview option pretty much means that the rule's in place. It's being processed. It used the conditions, the defined conditions, but the action is not taken if the match conditions happen. Now what can be protected by Cloud Armor? John: Haider, I think we had a couple of questions on that last slide. So Nicholas had a question around the next generation firewall heuristics. Do we have a next generation firewall heuristics based service? Haider: So not natively. So next generation firewall usually gets into deep packet inspection and IPS capabilities. We don't have a native offering yet for our next generation firewall. The solution to deploy next generation firewall is using a marketplace appliance. We do have best practices for how these appliances can be deployed, skilled, and designed for high availability. John: And then Brooks had a question around when features are only available in Managed Protection Plus version. Can you mention that as you work through the discussion? Haider: I have a slide that actually list out which service is available to what model. So we'll cover that in more details. John: Perfect. Haider: OK, cool. So what is protected by Cloud Armor policies? Think about it as anything that you can put behind a load balancer. And this will include in this case back end services that are based on VMs like managed or end managed VMs, auto scaled VMs. It could be Google Cloud Storage buckets, CDN origins. Because our edge policies are enforced on CDN origins as well. So the cache hits are also included in inspection. Storage buckets, as I mentioned. It can also include GKE services. So if you have services that are [INAUDIBLE] GKE clusters, those are natively supported as a back end behind [INAUDIBLE] load balancer. It can be serverless services like App Engine or Cloud Function. These services, again, natively supported by as a back and forth [INAUDIBLE]. As a result traffic to these services can be inspected as part of these policies. And finally, we also support a hybrid model where you can point to any public IP address as your back end to the load balancer. We call this a hybrid NEG service, network endpoint service. So these NEGs are supported as a public IP address. So anything that could be running on your on premises environment or a different cloud platform that you want to protect as well, these are all configurable. And the condition is pretty much as long as there is an internet connectivity in place that will enable the communication to this public IP address, it will be supported.

### Quiz - [Quiz: DDos mitigation and network threat intelligence](https://www.cloudskillsboost.google/course_templates/502/quizzes/490356)

#### Quiz 1.

> [!important]
> **SSL offloading policies are defined by:**
>
> - [ ] The user
> - [ ] Customers
> - [ ] Google
> - [ ] Developers

#### Quiz 2.

> [!important]
> **What are external load balancers?**
>
> - [ ] A fleet of load balancers that are positioned as far as possible to the user.
> - [ ] Cloud resource provisioning tools.
> - [ ] A fleet of load balancers that are positioned as close as possible to the user.
> - [ ] Load balancers that operate in the cloud.

#### Quiz 3.

> [!important]
> **Which Google Cloud product integrates with external load balancers, to build protection as close as possible to the user?**
>
> - [ ] Cloud IDS
> - [ ] VPC Service Controls
> - [ ] Assured Controls
> - [ ] Google Cloud Armor

#### Quiz 4.

> [!important]
> **Google Cloud Armor gives you the capability to create security policies between:**
>
> - [ ] Cloud Load Balancer and the backend
> - [ ] App Instances and Cloud Load Balancer
> - [ ] Coud Armor rules and the backend

#### Quiz 5.

> [!important]
> **Your organization has an application that only needs to be accessed from certain geographical locations. How does Google Cloud Armor help mitigate DDos attacks in this instance?**
>
> - [ ] Users can specify their location when they access your applications.
> - [ ] Google Cloud Armor is more effective in specified geographical locations.
> - [ ] It runs on a server so it can scale globally.
> - [ ] It allows, blocks, or rates limit traffic based on Geo parameters.

#### Quiz 6.

> [!important]
> **What network security control allows public access to private resources?**
>
> - [ ] Cloud VPN
> - [ ] Cloud IDS
> - [ ] Cloud NAT
> - [ ] VPC Controls

#### Quiz 7.

> [!important]
> **Which security control addresses data exfiltration concepts?**
>
> - [ ] Cloud IDS
> - [ ] VPC Service Controls
> - [ ] Packet Mirroring
> - [ ] VPC Firewall

#### Quiz 8.

> [!important]
> **What are firewall rules used for?**
>
> - [ ] Align services with the Infrastructure as a Service model.
> - [ ] Enable access to private resources.
> - [ ] Establish what gets provisioned inside your VPC network.
> - [ ] Allow traffic between resources in the same VPC.

#### Quiz 9.

> [!important]
> **Which is not a part of a Cloud Armor rule?**
>
> - [ ] Update
> - [ ] Preview
> - [ ] Action

## Google Cloud Armor Features and Benefits

This module walks through the features and benefits of Google Cloud Armor.

### Video - [Cloud Armor Features and Benefits](https://www.cloudskillsboost.google/course_templates/502/video/490357)

- [YouTube: Cloud Armor Features and Benefits](https://www.youtube.com/watch?v=PVSM7wWSIfc)

Haider: Now let's go over some of the features and capabilities available today with Cloud Armor. And we have it all listed here. And we're going to explain-- I'm going to go quickly through the list and explain some of those more details during this session. We mentioned the layer three, layer four DDoS Defense. Think about it as you have a reverse proxy. So only work from PCB connections will pass through. IP-based filtering, ASN. ASN, in this case, is the BGP autonomous system number. And this is your filtering based on the source. The source ASN of the traffic initiating the request. And of course, geo-based rules, as I mentioned, with certain countries if you want to have it only accessible from certain countries or if you want to block traffic from other certain countries that are considered as a high risk. Or if you don't expect any traffic or any valid request to come from this country. WAF rules. We have the pre-configured WAF rules. Those are based on the OWASP T10 attack. OWASP top 10, which means the top 10 common web attacks. We saw custom exclusion languages for our rules. We support bot management. And bot management here will enable you to differentiate human versus bot traffic. There are-- some of the common attacks that can always be-- part of the challenge of understanding if this is a DDoS attack or legitimate traffic is really by filtering based on bot versus human traffic. Because the traffic itself is-- really legitimate traffic looks legitimate traffic on all levels. So bot management becomes an important piece of protection, which is something we can expand on later. Adaptive Protection. Engage machine learning engines and capabilities to analyze traffic, generate signatures, and give you suggestions to block traffic. To block possible attacks. Managed Protection Plus is our feature to provide managed protection where you will have a team of security experts monitoring your traffic and collecting-- in the case of there was an attack, you have advanced capability supported with Managed Protection as well. And you also have a price protection where you're not going to pay for any resources that were scaled up due to a response to a DDoS attack. As you know, Cloud resources are scalable by design. So you're not going to pay for any scale on the backbone that was caused by attacks. And that's another metric that is important-- that financial insurance there. Edge Policies to protect backends on CDNs and GCS. I mentioned that. Rate Limiting is a new feature, as well, that we added. And with Rate Limiting, you're going to have-- be able to have an additional action of-- it's not just allow or deny the traffic that match the rule you created, it's also throttling that traffic if you feel that you want to make sure that resources are not exhausted on your back end but you don't want to really block the traffic. The telemetry and logs and findings of the Cloud Armor are reported to our Security Command Center. And at the end, named IP lists, which is a new feature that we added where we integrate with IP lists that are managed by third-party providers. This is another thing that I'm going to discover-- discuss in more details later today. So let's go through-- let's expand on some of these capabilities here. So things that are blocked by default, they will be dropped, like SYN flood, right? ICMP floods or ICMP ping attacks. Slowloris where a number-- you have a basic attack that tried to kind of open up a lot of connections and maintain these connections open for the purpose of exhausting backends. All of those attacks are blocked by default. Because they are blocked by default, you're not going to have a level of customization for-- if it was a SYN flood attack, send this error message to the attacker. So the attacker is not going to get that error message in this case. But if it's something that is more advanced that you're going to capture with a rule, then you do have the level of control for what is the return error if the traffic matches. So that's the first thing we mentioned, layer three, layer four volumetric attacks. With the origin, we-- with our rules-- with our custom rules, custom expression languages can be used where you will filter based on the request origin country code. These codes are defined by the ISO 3166 standard. And those are two digit country codes. The information is all published and our tuning guide, as well, where you will list the countries where you want, in this case, in this example, allow traffic. So this is US and Singapore. And everything else will be denied. As I mentioned, there could be situations where you're blocking traffic from certain countries. And in this case, you will use a reverse strategy where you start blocking the traffic while your default rule is going to have, let's say, allow all. Or based on the order, you can have, first of all, countries that you block. And then, after that, traffic that you want to identify and allow. Then you can maintain a denial all rule at the end. So it's really flexible around the security model needed.

### Video - [WAF Rules](https://www.cloudskillsboost.google/course_templates/502/video/490358)

- [YouTube: WAF Rules](https://www.youtube.com/watch?v=O4DfSfwf2js)

Haider: The pre-configured WAF rules is a really important feature. And the pre-configured WAF rule with Cloud Armor are based on the ModSecurity rule set, OWASP rules. Those rules are maintained by a third party. But we use it as is. What we do from our side is that we always keep the information current around our updates and the core rules. So right now, we are deploying rules from their 3.0.2 version. We have 20 name signatures that you can evaluate. And the evaluation is as easy as creating a rule and you say evaluate, for example, the SQL is stable or the [INAUDIBLE] scripting access stable signature. As you can see, there's a stable and there is a canary version. As you can tell, stable is more stable, canary is where the bot fixes get reported first before they go to the stable version. And the available signatures today covers SQL injection, cross-site scripting, more file inclusion, local [INAUDIBLE] inclusion, remote code executions, a lot of things really that are available in this-- in the ModSec rules. In addition, when a new vulnerability get discovered, we'll always work on making sure that the new signature that's created to match this traffic is added. A good example was the Log4j vulnerability was discovered. And we had a lot of customers who wanted to make sure that they're going to leverage this new rule to make sure that they can protect their applications. And as a matter of fact, that was a use case for moving a lot of workloads behind HTTPS load balancer in Cloud Armor to be able to address this vulnerability. And it's going to be available-- that's for a signature called Cve-canary. Of course, because these rules are standard rules, and every application will have specific requirements, the tuning of these rules is needed. And the goal is to minimize noise and false positives. These rules comes with four sensitivity levels, starting from level one all the way to level four, level four being the noisiest, which means level four will just evaluate all of the sub-signatures. Level one is going to be the less sensitive because it's going to have a lot of executions around signatures that can generate a lot of false positives. As you can see here, this is an example of a SQL stable signature, but we are [INAUDIBLE] all of these sub-signatures that are known to generate a lot of false positives. The recommendation, of course, as an example of a level two. The recommendation is that you set the rule-- you start to evaluate these signatures, but don't start to enforce the traffic day one. Put the rule in preview mode. And once you do that, you'll start to capture logs and then you get to review logs to make sure that you are not blocking legitimate traffic. And this is where, at the end of the session, you're going to have the section about telemetry and logging to tell you where you're going to find these nodes. But as part of any best practice, when you deploy these resources, you need to make sure that you're not blocking legitimate traffic, just because DDoS attacks are, by nature-- use legitimate traffic to bring down your application.

### Video - [Adaptive Protection](https://www.cloudskillsboost.google/course_templates/502/video/490359)

- [YouTube: Adaptive Protection](https://www.youtube.com/watch?v=_VhtUuVLpO4)

Haider: So let's cover the new features. And with the new feature, the first one that comes at the top of the list is Adaptive Protection. Adaptive Protection enabled the use of machine learning algorithms and engines that are developed by Google to detect possible attacks. And this is as easy as a checkbox, literally. You don't have to do anything special other than visiting your policy and check box, enable a checkbox that says, turn on Adaptive Protection. What we will do under the hood is that we will deploy this engine. The engine is going to go through a learning phase. And this learning phase can be from one hour to a few days for the purpose of understanding what's normal for your application. And then, start to give predictions about what is not normal, looking for anomalies where there is a change in the pattern of accessing your application. So Adaptive Protection is going to look for HTTP GET flood and POST flood attacks. And those are really hard to discover, typically, because they are perfectly legitimate traffic. Their goal is to either upload a huge amount of data to your application or site or download a lot of data from your site, distribute it from multiple locations. This is where bot attacks also-- bot sources comes in play. And that's why they are really hard to discover. And they are so common and they have taken down websites in the past. So what Adaptive Protection is going to do is it's going to analyze logs generated by Cloud Armor. And it will give you real time data about possible attacks that will generate-- it will generate a signature to block this attack and propose to block that signature. The customer will-- based on evaluating this data, they will need to enforce the-- place that role. And of course, when they place the role, they will have the option of, are you going to put it in enforcement mode where it will start to block that traffic immediately, or you want it to be in evaluation or in preview mode for you to review alerts before you enforce the traffic. The phases where the traffic or the enablement is going to go through a learning phase first. We'll start to understand the normal access pattern. After that, it will start to detect attacks. So just use rules and the mitigation piece-- give you the mitigation piece, which is as easy as click of a button. To really maximize the effectiveness of blocking their GET and POST clouds in addition to Adaptive Protection, bot protection is going to be needed, really, to get to a point where you feel that you really have a solid policy here against that type of attacks. Bot protection or bot management, we're going to cover that in the next slide-- not this one, the one after.

### Video - [Cloud Armor Per-Client Rate Limiting](https://www.cloudskillsboost.google/course_templates/502/video/490360)

- [YouTube: Cloud Armor Per-Client Rate Limiting](https://www.youtube.com/watch?v=OXcDgiUfUkw)

Haider: But speaking of new capabilities, we've covered actions where you have a condition and you have an action of either allow or deny. With the throttling or rate-based-ban, we are introducing additional action where you may not want to block that traffic, but really throttle that traffic only. And the new actions that we added is you can either throttle the traffic to a certain number of requests per interval that you configure, or you can have a temporary ban. And in this case, it will give-- define that ban period for that request. Of course, this is going to come as part of-- once the traffic matches, the action will be taken. We also have a control for what you want to do with the traffic that exceed the limit. Do you want to deny that traffic? Do you want to redirect? Sending external 302 redirect? Or do you want to send it to a recapture? Recapture is going to be that bot management tool where the recapture-- I'm going to explain shortly-- you can either solve a puzzle to make sure that this is human traffic, or there's a frictionless mode that we also have available. So this is a new feature that we recently launched and is currently generally available. John: So I had a quick question on this one. So this is kind of a two-part question that I was thinking about before. So when we look at this, a lot of times, we work with like state agencies and they may have integrated eligibility or people within the state signing up for stuff. In certain cases, there's a lot of concern around fraud. Around people coming from outside the country or things along those lines and you don't necessarily want to block those folks. But could you rate limit them and slow down their performance so that their customer experience is not as good as maybe somebody in your state or in the US? Is that a potential use case for this? Haider: Absolutely. Absolutely. That's a really valid use case here. And with the limits that can be defined, it can be starting from one to I think around 10,000. So that's absolutely a valid use case. Other use cases, sometimes we see is a backend with a limited capacity of resources. And you want to make sure that no single user or group of users will exhaust the resources of the backend. Having a deny or a block action sometimes is limiting with respect to assuring a good user experience. Specifically, when there is a doubt about is this is an attack or that's a legitimate traffic. John: Yeah, and that's another use case. So would this be a valid use case if you're worried about your backend system not being able to handle the load? You're turning it on day one. A lot of folks that we work with have systems on premises that can't horizontally scale or scale up as fast as you could if that application was on the Cloud. And a lot of customers want to move to the Cloud. But obviously, that's not-- day one, you can't necessarily do that. Can we leverage Cloud Armor and the Global Load Balancer capabilities against on premises deployments, or maybe even another Cloud environment? Haider: Absolutely. As I mentioned with the hybrid model, you can point to a backend that resides outside of the Cloud. And that's a very good point that you're bringing up here. We actually work with customers-- agencies like local agencies where the backend is something that's really not scalable. And they wanted to make sure that, during certain times, with the increased number of requests-- we went through the multiple cases of the COVID impact, people signing up for unemployment benefits or people signing up for the vaccine. Those were all valid use cases. At that time, the service-- this feature was not generally available. But we did actually provide access for the customers for those agencies to be able to leverage this feature. Very good call out. John: Cool. Thank you.

### Video - [Cloud Armor Bot Management](https://www.cloudskillsboost.google/course_templates/502/video/490361)

- [YouTube: Cloud Armor Bot Management](https://www.youtube.com/watch?v=ZZGuk7_Oec4)

Haider: The bot management component is something that I mentioned earlier. And the idea here is differentiating between human versus not human traffic is another key factor here. Some of the attacks, because they are so legitimate, it's hard to know for sure if this is a valid traffic or not. So going back to the who's making the request becomes a critical piece. And this is exactly what reCAPTCHA is trying to do here. reCAPTCHA, we all use it. It's that challenge that you see when you try to log into a site to check the boxes for pictures of a bus or a car. And the idea here is, are you human or this is bot traffic? So what we did is that we enabled the integration-- native integration between Cloud Armor and our reCAPTCHA Enterprise so that Cloud Armor will take the decision of this traffic looks like it's a high-risk traffic. So let's just makes sure that this is a human traffic before we take a decision. So that's why the integration is really important. And with this launch of this service, we enabled two assessments-- enforcement assessment models. The first one is the frictionless. The frictionless is really amazing because it will look information up from the request-- it will collect information from the request based on the user mouse or based on libraries that are installed on the browser to tell-- to generate a metric like a score. And that score from 0 to 1, with 0 being less trusted, 1 being most trusted. And based on that, you can have control for-- allow everything that's over 0.7, for example, which means that this look as a quick traffic without the user doing anything. You don't have to serve a puzzle. We also have the option of redirect to reCAPTCHA challenge. In this case, as you can see here, you have this challenge where people have to click on pictures. The interesting thing, as well, is that we also-- we have an option, which we call the redemption flow where we use both. So the idea here is if the score generated by reCAPTCHA does not look safe enough, but we want to make sure that we want to give this user another chance. So you can have a condition of-- if the score is less than 0.7, then serve a challenge instead of just blocking that traffic. So that's why this really integration between Cloud Armor and reCAPTCHA is going to make a huge change into making sure that this traffic is not a bot traffic, that's a real user trying to access your application.

### Video - [Named IP Lists](https://www.cloudskillsboost.google/course_templates/502/video/490362)

- [YouTube: Named IP Lists](https://www.youtube.com/watch?v=f3lkzBI0S2g)

Haider: So I think I'm coming-- OK, so one last feature-- a new feature to touch on, the named IP lists. And named IP list is important, because when you use a provider like some of the CDM providers, you may have challenges with-- I want to make sure that only my provider send traffic to the load balancer-- my load balancer. So when you use one of the CDM providers, they will be the entry point of your application. They will do DNS or sometimes they provide the first level of DDoS mitigation. And then, when you want to leverage that second level from us, it becomes challenging knowing the traffic that they will use to source to our Cloud so that we only block access so that traffic is allowed from those providers. This is what named IP lists are going to provide us with is the ability to reference a name list. This list is not maintained by Google. It's maintained by the service provider so that you say only accept traffic from this service provider. And Cloud Armor will block any traffic that's directly generated from other than this network. This network, of course, will be maintained by this provider. And it is going to be for you as easy as a single rule with a single tag, and we will block that traffic when it comes outside of this list. So that's a new feature. We have a list of providers that are currently supported. I think because it's new, we only have three. Information is available on our website, and I'm happy to answer questions if there are specifics about who is supported and who is not yet. So that's another good service to have. I think there was-- I mentioned about what's included as part of the Managed versus Standard. So this slide tried to answer that question. The majority of the advanced features, as you can see, are part of the Managed Protection Plus. So the named IP list, I just explained the data protection, DDoS response support. This is the team of security experts who can assist you in the case of-- take all the analyzed traffic and assist you in the case of an attack. Pull protection as well. So those are part of the Managed Protection Plus. Managed Protection Plus is going to give you these features, but it will need a commitment. One year commitment at least. And then, you will pretty much get everything that you get with a Standard plus these features. And it also comes with a subscription model. Plus you'll pay a flat subscription model per year in addition to the data processing fees. I think there was a question about these features. So hopefully, this slide can answer the question. OK, moving on to the last section.

### Quiz - [Quiz: Cloud Armor Features and Benefits](https://www.cloudskillsboost.google/course_templates/502/quizzes/490363)

#### Quiz 1.

> [!important]
> **What is the bot management feature in Google Cloud Armor used for?**
>
> - [ ] Managing the bots your organization has built.
> - [ ] Differentiating between humans and bots.
> - [ ] Targeting bots.
> - [ ] Building new bots to detect mitigation.

#### Quiz 2.

> [!important]
> **What Google Cloud Armor feature uses machine learning to analyze and give suggestions for blocking potential attacks?**
>
> - [ ] Edge Policies for CDN & Cloud Storage
> - [ ] Custom Rules Language
> - [ ] Adaptive Protection
> - [ ] L3/L4 DDoS Defense

#### Quiz 3.

> [!important]
> **Redemption flow gives users another chance to prove they're not a bot by:**
>
> - [ ] Giving users 10 chances to pass a reCAPTCHA challenge.
> - [ ] Having traffic complete a reCAPTCHA challenge if their reCAPTCHA score isn't safe enough.
> - [ ] Granting the user access if their score was safe enough.
> - [ ] Granting the user access if they pass the initial reCAPTCHA challenge.

#### Quiz 4.

> [!important]
> **You need to make sure that only your provider sends traffic to the Cloud Load Balancer. What should you use?**
>
> - [ ] Edge policies
> - [ ] reCAPTCHA
> - [ ] A services list
> - [ ] A named IP list.

#### Quiz 5.

> [!important]
> **Pre-configured WAF rules provide detection and protection based on what?**
>
> - [ ] Encryption keys
> - [ ] Signatures
> - [ ] Code
> - [ ] Security

#### Quiz 6.

> [!important]
> **You've set up a threshold to throttle traffic in Google Cloud Armor for additional security, and you need to determine whether incoming traffic is human or bot. If your traffic exceeds the threshold you've set, you can redirect the traffic to:**
>
> - [ ] Crowdstrike
> - [ ] reCAPTCHA
> - [ ] Chronicle
> - [ ] Google Cloud Armor

#### Quiz 7.

> [!important]
> **Adaptive Protection analyzes logs and delivers real-time data on possible attacks. What Google Cloud product generates the logs?**
>
> - [ ] Google Cloud Armor
> - [ ] Assured Workloads
> - [ ] Assured Controls
> - [ ] Cloud DNS

#### Quiz 8.

> [!important]
> **What two types of attacks does Adaptive Protection look for?**
>
> - [ ] Traffic attacks and DDoS
> - [ ] Malware and phishing
> - [ ] HTTPS and HTTP
> - [ ] HTTP GET Flood and HTTP POST Flood

### Lab - [Bot Management with Google Cloud Armor and reCAPTCHA](https://www.cloudskillsboost.google/course_templates/502/labs/490364)

Use Google Cloud Armor bot management to mitigate bot risk and to control access from automated clients

- [ ] [Bot Management with Google Cloud Armor and reCAPTCHA](../labs/Bot-Management-with-Google-Cloud-Armor-and-reCAPTCHA.md)

## Cloud Logging, Monitoring, and Telemetry

This module gives an overview of Cloud Logging and Monitoring, and the Security Command Center.

### Video - [Cloud Logging](https://www.cloudskillsboost.google/course_templates/502/video/490365)

- [YouTube: Cloud Logging](https://www.youtube.com/watch?v=mGW338u2yW0)

Haider: Logging and monitoring, as we know, they need security tool viewing and analyzing logs is always key. So Cloud Armor actually send data to three different locations-- Cloud Logging, Monitoring, and our Security Command Center. The Cloud Logging piece, the first one, send you information about what was the package, what was the traffic that get blocked. And as you can see in this example, you're going to see the payload with respect to which policy get matched or was there action taken, so the policy name, the outcome, and the priority of the role. This information is key for you to tune up, to be able to tune up any role. So remember these roles that we said, don't offer at first day one, you need to analyze that first. This is where you need to see, look, for example, for denies. Or you can easily search through logs based on the security policy, and it will give you the exact same signature that it matched for that traffic. So you will be able to see the signature, you'll be able to see the request, and you will take a decision if this traffic should be blocked or there is a need to tune up the role before enforcing it. So that's the first place to find this detail information, the Cloud Logging, this is what you will need to, why you need to view this data.

### Video - [Cloud Monitoring](https://www.cloudskillsboost.google/course_templates/502/video/490366)

- [YouTube: Cloud Monitoring](https://www.youtube.com/watch?v=mYuzBBuJLOM)

Haider: The second place is Cloud Monitoring. And with Cloud Monitoring and alerting, you're going to find information about, real time information about a number of requests, allowed requests, logs. So you could if you want to build diagrams and monitor them, if you want to create alerts where you get notification for email or message or something else, cloud, this is what Cloud Monitoring can be useful, so real time reporting and alerting. John: I had a quick question. So all the logging, it's just done through the normal logging console, correct? Haider: Right, for the cloud log, yes. For the Cloud Logging, the Cloud Logging, with Google Cloud, there's one place for all of the logs. So Cloud Logging is going to have all of the information about what was blocked, what was allowed, et cetera. John: Then you can easily create your filters and your dashboards and monitoring as needed based upon your experience with Cloud Logging, the stack, the old Stackdriver stuff? Haider: Correct. This is where you start to export and import logs from one project or another, put them in one location for archiving, et cetera. Yeah. Monitoring, as we said, real time data about statistics, actions, can be also automated from there with respect to alerting.

### Video - [The Security Command Center](https://www.cloudskillsboost.google/course_templates/502/video/490367)

- [YouTube: The Security Command Center](https://www.youtube.com/watch?v=bhlqpOXJYEs)

Haider: The last place where you can find findings is the Security Command Center. So our Security Command Center, we designed it to be the one place for you to find all of the security-related actions and recommendations and findings. And in this case, Cloud Armor is going to report their findings-- the Adaptive Protection findings and recommendations about possible attacks. You will also find that in the Security Command Center. With the Security Command Center, you're going to have-- there are two primary findings that are being sent that allow traffic spike and increase the deny ratio. And this is important, because if there is a spike in the traffic you are allowing and this spike does not align with your expectation, there is nothing new being launched or you don't expect a spike in requests during normal times, this is-- this can trigger-- this is for you an event to go and double check if you have Adaptive Protection enabled to see if this is a possible attack. In addition, the increase in deny ratio, which can be an attack that was blocked or it could be a false positive that you need to look into for the possibility of tuning up on all of two. So these are reported to Security Command Center.

### Quiz - [Quiz: Logging, monitoring, and telemetry](https://www.cloudskillsboost.google/course_templates/502/quizzes/490368)

#### Quiz 1.

> [!important]
> **Which Google Cloud tool enables you to find real-time information about requests?**
>
> - [ ] Google Cloud Armor
> - [ ] Cloud Logging
> - [ ] Cloud Monitoring
> - [ ] Alerting

#### Quiz 2.

> [!important]
> **The two primary findings being sent to the Security Command Center are:**
>
> - [ ] Allowed and blocked requests.
> - [ ] Assets and tools
> - [ ] DDoS attacks and network security policies
> - [ ] Allowed traffic spike and increasing deny ratio.

#### Quiz 3.

> [!important]
> **Where are Google Cloud Armor findings and assets sent?**
>
> - [ ] Google Cloud
> - [ ] Security Command Center
> - [ ] Google Cloud Security Hub
> - [ ] Google Cloud Armor Security Hub

#### Quiz 4.

> [!important]
> **Cloud Logging provides you with traffic visibility so that you can:**
>
> - [ ] Find assets
> - [ ] Fine-tune rules
> - [ ] Manage bots
> - [ ] Define security metrics

## Course Resources

Student PDF links to all modules

### Document - [Work Safer Slides](https://www.cloudskillsboost.google/course_templates/502/documents/490369)

### Document - [DDos Mitigation and Network Threat Intelligence in Google Cloud Slides](https://www.cloudskillsboost.google/course_templates/502/documents/490370)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
