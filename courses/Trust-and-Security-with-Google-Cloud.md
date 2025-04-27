---
id: 945
name: 'Trust and Security with Google Cloud'
datePublished: 2024-06-17
topics:
- Network Security
- Security
type: Course
url: https://www.cloudskillsboost.google/course_templates/945
---

# [Trust and Security with Google Cloud](https://www.cloudskillsboost.google/course_templates/945)

**Description:**

As organizations move their data and applications to the cloud, they must address new security challenges. The Trust and Security with Google Cloud course explores the basics of cloud security, the value of Google Cloud's multilayered approach to infrastructure security, and how Google earns and maintains customer trust in the cloud.

Part of the Cloud Digital Leader learning path, this course aims to help individuals grow in their role and build the future of their business.

**Objectives:**

- Identify fundamental security concepts.
- Explore the business value of Google’s defense-in-depth multilayered approach to infrastructure security.
- Learn how Google Cloud works to earn and maintain customer trust in the cloud.

## Course Introduction

In this introduction, you explore the course goals and preview each section.

### Video - [Course introduction](https://www.cloudskillsboost.google/course_templates/945/video/487300)

- [YouTube: Course introduction](https://www.youtube.com/watch?v=g8LlQUJ4c_0)

At Google Cloud, we understand the responsibility that comes with hosting, serving, and safeguarding our customers' valuable data. As organizations increasingly migrate their data and applications to the cloud, it becomes crucial to address the emerging security challenges. Trust and security lie at the heart of our product design and development philosophy. We firmly believe that our customers own their data and have complete control over its usage. Although we’ve implemented robust security measures to defend against potential breaches, we also acknowledge that security is a dynamic and ongoing process that demands constant attention and investment. To support you in this journey, we provide a range of security products and services that enable you to detect, investigate, and mitigate cyber threats while aligning with your policy, regulatory, and business objectives. The objective of this course, “Trust and Security with Google Cloud,” is to equip you with the knowledge and skills necessary to discuss fundamental cloud security concepts, explain the business value of Google’s multilayered approach to infrastructure security, and describe how Google Cloud earns and maintains customer trust in the cloud. Throughout the course, you’re presented with graded knowledge assessments. You must pass these assessments to receive course credit. OK, let's get started!

## Trust and Security in the Cloud

In this section of the course, you explore today's top cybersecurity threats and how they impact businesses, differences between cloud security and traditional on-premises security, and key security terms and concepts. 

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/945/video/487301)

- [YouTube: Introduction](https://www.youtube.com/watch?v=_n4an24UAII)

In recent years, the rise of cloud computing has transformed the way that organizations store, process, and manage their data. However, with this increased reliance on the cloud, the need for robust security measures has become essential. Securing data, applications, and infrastructure in the cloud is a complex and ever-evolving challenge. As new threats and vulnerabilities emerge, organizations must stay ahead of the curve and adapt their security strategies to mitigate risks effectively. In this section of the course you’ll define key security terms and concepts, describe the importance of confidentiality, integrity, availability, control, and compliance in a cloud security model, differentiate between cloud security and traditional on-premises security, and describe today's top cybersecurity threats and business implications.

### Video - [Key security terms and concepts](https://www.cloudskillsboost.google/course_templates/945/video/487302)

- [YouTube: Key security terms and concepts](https://www.youtube.com/watch?v=gUUMKdGGQhY)

In the field of cloud security, understanding the terminology is crucial to navigating the landscape effectively. In this lesson, we introduce essential security terms and concepts that are commonly encountered when discussing cloud security. Let's explore these terms and their significance. The first three concepts relate to reducing the risk of unauthorized access to sensitive data. The privileged access security model grants specific users access to a broader set of resources than ordinary users. For example, a system administrator may have privileged access to perform tasks such as troubleshooting and data restoration. However, the misuse of privileged access can pose risks, so it’s essential to manage and monitor such access carefully. The least privilege security principle advocates granting users only the access they need to perform their job responsibilities. By providing the minimum required access, organizations can reduce the risk of unauthorized access to sensitive data. For instance, a sales representative might only need access to a customer relationship management (CRM) system without requiring access to other systems like payroll or finance. The zero-trust architecture security model assumes that no user or device can be trusted by default. Every user and device must be authenticated and authorized before accessing resources. Zero-trust architecture helps ensure robust security by implementing strict access controls and continuously verifying user identities. These next three concepts relate to how an organization can protect itself from cyber threats. Security by default is a principle that emphasizes integrating security measures into systems and applications from the initial stages of development. By prioritizing security throughout the entire process, organizations can establish a strong security foundation in their cloud environments. Security posture refers to the overall security status of a cloud environment. It indicates how well an organization is prepared to defend against cyber attacks by evaluating their security controls, policies, and practices. Cyber resilience refers to an organization's ability to withstand and recover quickly from cyber attacks. It involves identifying, assessing, and mitigating risks, responding to incidents effectively, and recovering from disruptions quickly. Finally, let's explore essential security measures to protect cloud resources from unauthorized access. A firewall is a network device that regulates traffic based on predefined security rules. You can think of a firewall like a security guard for a network. It follows certain rules to decide which traffic is allowed to enter or leave a network. These rules help keep unauthorized people or harmful things away from important cloud resources, such as servers, databases, and applications. Following our previous analogy, a security guard checks everyone who wants to enter and only lets in those who have permission. Similarly, a firewall checks the incoming and outgoing traffic in a network and only allows the ones that are safe and authorized. Encryption is the process of converting data into an unreadable format by using an encryption algorithm. Decryption, however, is the reverse process that uses an encryption key to restore encrypted data back to its original form. Safeguarding the encryption key is crucial, because it holds the secret algorithm necessary for decrypting the data. Another way to think about encryption and decryption is writing a message in a secret language that only you and the person you want to send it to can understand. This way, even if someone intercepts the message, they won't be able to read it, because they don't know the secret language.

### Video - [Cloud security components](https://www.cloudskillsboost.google/course_templates/945/video/487303)

- [YouTube: Cloud security components](https://www.youtube.com/watch?v=b2hMWU2D268)

In this lesson, we learn about the components that make up a cloud security model and discover how they contribute to a robust security posture in today's digital landscape. We’ll first explore three essential aspects of security: Confidentiality, Integrity, and Availability. These three principles form the foundation of the “CIA Triad”, a widely used model for developing effective security systems. The CIA triad emphasizes the importance of protecting sensitive information, ensuring data accuracy and trustworthiness, and maintaining uninterrupted access to resources and services. By understanding and implementing measures to address these aspects, organizations can establish a strong security framework to safeguard their digital assets. Confidentiality is about keeping important information safe and secret. It ensures that only authorized people can access sensitive data, no matter where it's stored or sent. Confidentiality is of utmost importance in the cloud, as sensitive information stored and transmitted across cloud environments must be protected from unauthorized access or disclosure. Encryption plays a crucial role in ensuring confidentiality in the cloud. By using encryption techniques and safeguarding encryption keys, organizations can ensure that only authorized individuals can access and decrypt sensitive data, effectively mitigating the risk of data breaches in the cloud. Integrity means keeping data accurate and trustworthy. It ensures that information doesn't get changed or corrupted, no matter where it's stored or how it's moved around. You can think of it like making sure a message doesn't get altered during delivery. Integrity in the cloud involves ensuring the accuracy and trustworthiness of data throughout its lifecycle. Implementing data integrity controls, such as checksums or digital signatures, enables organizations to verify the authenticity and reliability of their data in the cloud. This helps prevent unauthorized modifications or tampering, ensuring the integrity of critical information stored and processed in cloud environments. Availability is all about making sure that cloud systems and services are always accessible and ready for use by the right people when needed. It's like having a reliable electricity supply that never goes out. Cloud environments must be designed with redundancy, failover mechanisms, and disaster recovery plans to maximize availability and minimize downtime. By implementing these measures, organizations can ensure that their systems and applications in the cloud remain accessible whenever needed, promoting business continuity even in the face of potential disruptions. Control refers to the measures and processes implemented to manage and mitigate security risks. It involves establishing policies, procedures, and technical safeguards to protect against unauthorized access, misuse, and potential threats. Control measures in the cloud include implementing robust authentication mechanisms, access restrictions, and security awareness training. These measures help organizations manage and mitigate security risks associated with cloud-based systems. By ensuring that only authorized individuals have access to sensitive data and systems in the cloud, organizations can reduce the risk of data breaches and unauthorized activities. Finally, compliance relates to adhering to industry regulations, legal requirements, and organizational policies. It involves ensuring that security practices and measures align with established standards and guidelines. Meeting compliance standards in the cloud demonstrates an organization's commitment to data privacy and security, building trust with stakeholders, and minimizing legal and financial risks. Cloud providers often offer compliance frameworks and certifications that organizations can leverage to meet their regulatory obligations. By integrating these principles into a comprehensive cloud security model, organizations can establish a strong foundation for protecting their data, maintaining data integrity, and ensuring continuous access to critical resources.

### Video - [Cloud security versus traditional on-premises security](https://www.cloudskillsboost.google/course_templates/945/video/487304)

- [YouTube: Cloud security versus traditional on-premises security](https://www.youtube.com/watch?v=bxN8gfdp2rc)

In the past, businesses heavily relied on their own infrastructure and local data centers to manage and protect their digital assets. They had complete control over their hardware, software, and network components, fostering a sense of trust within their premises. However, as organizations now connect digitally with customers, partners, and employees worldwide, new risks have emerged that require enhanced security measures. This is where cloud security comes into play by offering a different approach compared to traditional on-premises security. Let's explore these important differences. The first is location. Cloud security involves hosting and managing data and applications in off-site data centers operated by cloud service providers. The responsibility for securing the infrastructure and underlying hardware lies with the cloud provider. Conversely, traditional on-premises security involves hosting and managing data and applications locally on an organization's own servers and infrastructure, granting direct control and responsibility for securing the physical and virtual environment. Next is responsibility. In a cloud model, the cloud service provider is responsible for securing the infrastructure, network, and physical facilities. The customer is typically responsible for securing their data, applications, user access, and configurations. On the other hand, in an on-premises setup, the organization is responsible for securing the entire infrastructure, including hardware, network, operating systems, applications, and data. The next difference is scalability. Cloud security offers scalability and elasticity, which allows organizations to easily scale their resources up or down based on demand. This flexibility is suitable for dynamic workloads and rapid growth. In contrast, on-premises security requires organizations to provision and maintain their own infrastructure, which can be more time-consuming and costly when they scale up or down. Next is maintenance and updates. Cloud service providers handle infrastructure maintenance, including security updates, patching, and software upgrades. Customers can focus on managing their applications and data without worrying about the underlying infrastructure. On-premises environments require organizations to maintain and update their own infrastructure, involving regular tasks such as patching, software updates, and hardware upgrades. The final difference is capital expenditure. Cloud security follows an operational expenditure (OpEx) model, where organizations pay for the services they consume on a subscription basis. This eliminates the need for large upfront capital investments in physical security infrastructure. Traditional on-premises security models involve significant capital expenditure (CapEx), because organizations must purchase and maintain their own security infrastructure. Understanding these differences between cloud security and traditional on-premises security helps organizations make informed decisions about the most suitable approach for their specific needs. Cloud security offers benefits such as offloading infrastructure management, scalability, and cost flexibility. However, traditional on-premises security provides direct control over the entire infrastructure. Organizations must carefully evaluate their requirements and consider factors such as data sensitivity, compliance regulations, and scalability to determine the most effective security strategy for their business.

### Video - [Cybersecurity threats](https://www.cloudskillsboost.google/course_templates/945/video/487305)

- [YouTube: Cybersecurity threats](https://www.youtube.com/watch?v=KLRvrLjCOsc)

In today's fast-paced digital world, we’re bombarded with attention-grabbing headlines. "CEOs Beware: The Perils of Career-Ending Cyberattacks" "Retailer Pays a Hefty $179 Million Due to Data Breach Fallout" "Credit Agency Settles US Data Breach, Facing Up to $700 Million in Penalties" The realm of cyberattacks is evolving rapidly, and these threats can emerge from unexpected sources, even disguised as government entities. So, what are some common cybersecurity threats faced by organizations? First is deceptive social engineering. Imagine that a skilled manipulator is seeking to extract confidential system information from unsuspecting individuals. These cybercriminals employ “phishing attacks,” which collect personal details about you, your employees, or your students. They skillfully craft tailored emails and mimic authenticity to deceive their targets. Therefore, anyone within your organization can be tricked into inadvertently downloading malicious attachments, divulging passwords, or compromising sensitive data. Next is physical damage. Whether it be damage to hardware components, power disruptions, or natural disasters such as floods, fires, and earthquakes, organizations are responsible for safeguarding data even in the face of physical adversity. You can think of this as protecting precious assets amidst nature's unforgiving forces. Another threat is malware, viruses, and ransomware. These digital adversaries architect chaos within the cyber domain. Employing malicious software, they aim to disrupt operations, inflict damage, or gain unauthorized access to computer systems. The most insidious of these is ransomware, where crucial files are held hostage until a considerable ransom is paid. It's like witnessing the digital equivalent of a calculated extortion scheme. The next cybersecurity threat is vulnerable third-party systems. Imagine inviting a trusted ally into your domain, only to discover that they inadvertently compromise your security. Many organizations rely on third-party systems for essential functions such as finance, inventory management, or account operations. However, without adequate security measures and regular evaluations, these systems can transform into potential threats, leaving data security vulnerable. It's like using a tool that unwittingly introduces risks to your own treasured possessions. The final threat is configuration mishaps. Even the most seasoned experts make mistakes. Misconfiguration occurs when errors arise during the setup or configuration of resources, which inadvertently exposes sensitive data and systems to unauthorized access. Surveys consistently identify misconfiguration as the most prominent threat to cloud security. In turn, adopting principles of least privilege and privileged access are imperative, because they allow resource access only when explicitly required and authorized. This is like granting access only to those who have earned your trust. As technology continues to advance at an astonishing pace, organizations must invest in the right expertise to assess, develop, implement, and maintain robust data security plans.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/945/quizzes/487306)

#### Quiz 1.

> [!important]
> **Which is the responsibility of the cloud provider in a cloud security model?**
>
> - [ ] Maintaining the customer's infrastructure.
> - [ ] Managing the customer's user access.
> - [ ] Configuring the customer's applications.
> - [ ] Securing the customer's data.

#### Quiz 2.

> [!important]
> **Which cloud security principle ensures that security practices and measures align with established standards and guidelines?**
>
> - [ ] Integrity
> - [ ] Confidentiality
> - [ ] Control
> - [ ] Compliance

#### Quiz 3.

> [!important]
> **Which cybersecurity threat demands a ransom payment from a victim to regain access to their files and systems.**
>
> - [ ] Spyware
> - [ ] Virus
> - [ ] Trojan
> - [ ] Ransomware

#### Quiz 4.

> [!important]
> **Which is a benefit of cloud security over traditional on-premises security?**
>
> - [ ] Large upfront capital investment.
> - [ ] Increased scalability.
> - [ ] Only having to install security updates on a weekly basis.
> - [ ] Having physical access to hardware.

#### Quiz 5.

> [!important]
> **Which definition best describes a firewall?**
>
> - [ ] A software program that encrypts data to make it unreadable to unauthorized users
> - [ ] A set of security measures designed to protect a computer system or network from cyber attacks
> - [ ] A security model that assumes no user or device can be trusted by default
> - [ ] A network security device that monitors and controls incoming and outgoing network traffic based on predefined security rules

#### Quiz 6.

> [!important]
> **Which cybersecurity threat occurs when errors arise during the setup of resources, inadvertently exposing sensitive data and systems to unauthorized access?**
>
> - [ ] Malware
> - [ ] Virus
> - [ ] Configuration mishaps
> - [ ] Phishing

#### Quiz 7.

> [!important]
> **Which cloud security principle relates to keeping data accurate and trustworthy?**
>
> - [ ] Compliance
> - [ ] Integrity
> - [ ] Control
> - [ ] Confidentiality

#### Quiz 8.

> [!important]
> **Which three essential aspects of cloud security form the foundation of the CIA triad?**
>
> - [ ] Certificates, intelligence, and authentication
> - [ ] Compliance, identity, and access management
> - [ ] Containers, infrastructure, and architecture
> - [ ] Confidentiality, integrity, and availability

#### Quiz 9.

> [!important]
> **What common cybersecurity threat involves tricking users into revealing sensitive information or performing actions that compromise security?**
>
> - [ ] Malware
> - [ ] Ransomware
> - [ ] Phishing
> - [ ] Configuration mishap

#### Quiz 10.

> [!important]
> **Which security principle advocates granting users only the access they need to perform their job responsibilities?**
>
> - [ ] Least privilege
> - [ ] Zero-trust architecture
> - [ ] Privileged access
> - [ ] Security by default

## Google’s Trusted Infrastructure

In this section of the course, you focus on the security benefits of Google's data centers, the role encryption plays in securing data, the difference between authentication, authorization, and auditing, and how Google products can help protect against network attacks.

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/945/video/487307)

- [YouTube: Introduction](https://www.youtube.com/watch?v=ehNS6P-Ucs4)

At Google Cloud, we believe in going beyond reliance on a single technology for security. Our multilayered strategy builds progressive security layers, combining global data centers, purpose-built servers, custom security hardware and software, and two-step authentication. This approach provides true defense-in-depth. In this section of the course, you’ll learn about how Google designs and builds its own data centers by using purpose-built servers, networking, and custom security hardware and software, the role that encryption plays in securing an organization’s data and the ways that it can protect data exposed to risks in different states, the differences between authentication, authorization, and auditing, the benefits of using two-step verification and Identity and Access Management, or IAM, how an organization can protect against network attacks by using Google products, and security operations in the cloud and its related business benefits.

### Video - [Data centers](https://www.cloudskillsboost.google/course_templates/945/video/487308)

- [YouTube: Data centers](https://www.youtube.com/watch?v=iS9ZPZ-Hw7I)

Data centers are more than just facilities filled with computers. They’re the backbone of round-the-clock operations for Google's services, including Search, Gmail, and YouTube. Moreover, they play a crucial role in storing and processing data for all the services provided on Google Cloud. At present, Google operates over 30 state-of-the-art data centers worldwide, with some still under construction. These advanced facilities are meticulously designed to deliver exceptional reliability, top-notch security, and outstanding efficiency, and they ensure that Google's services are always available when you need them. But it doesn't stop there. Google is committed to minimizing the environmental impact of data centers. By using cutting-edge technologies and renewable energy sources, we strive to reduce our ecological footprint. Let's explore the benefits of Google designing and building its own data centers, using purpose-built servers, advanced networking solutions, and custom security hardware and software. One of the greatest advantages of Google's data centers is the implementation of a zero-trust architecture, which ensures enhanced security at every level. Our custom hardware and software are purpose-built with features like tamper-evident hardware, secure boot, and hardware-based encryption, which establish a strong security posture within the data center environment. Physical security is paramount as well, with robust access control measures and biometric authentication in place. By adopting the principle of least privilege, only authorized personnel have access to the data centers, which minimizes the risk of physical breaches and maintains a privileged access framework. Furthermore, our data centers embody the concept of security by default. From the moment you step into a Google data center, you can trust that every aspect has been designed and implemented with your security in mind. With cyber resilience as a core principle, our data centers are equipped to withstand and recover from potential security incidents, and ensure the continuity and integrity of your data. Efficiency is another important aspect of our data center design. Purpose-built servers are optimized for specific tasks, which allows them to perform at great speed and with exceptional efficiency. This reduces energy consumption, cuts down on operating costs, and saves resources and the environment. In fact, we measure our success through the Power Usage Effectiveness (PUE) score. By continually striving for the lowest PUE scores, we ensure maximum efficiency in our data centers, leading to significant cost savings and a reduced carbon footprint. For instance, our data center in Hamina, Finland, stands out as one of the most advanced and efficient facilities in our fleet. Its innovative cooling system, which uses sea water from the Bay of Finland, sets a new standard for energy efficiency worldwide. Scalability is another benefit. Our data centers can quickly and seamlessly accommodate new hardware and servers, which allows us to scale up computing resources on demand. This flexibility is critical for Google to handle massive data volumes and traffic without any disruptions to services. Furthermore, managing our own servers and network provides us with unparalleled customization capabilities. This level of flexibility empowers us to deliver unique services and capabilities that are not available from other providers, giving you access to exclusive features and innovations. Although designing and building data centers requires significant upfront investment, the long-term benefits are substantial. By optimizing resources for efficiency and scalability, Google can significantly reduce energy consumption and operating costs, which results in remarkable savings over time.

### Video - [Secure storage](https://www.cloudskillsboost.google/course_templates/945/video/487309)

- [YouTube: Secure storage](https://www.youtube.com/watch?v=QbZMjnslsco)

Previously, we learned that encryption is like a secret code that transforms data into an unreadable format using special algorithms. This process ensures that only those with the right key or password can make sense of the data. It's like using a secret language to protect your information. By encrypting your data, you can protect it from various risks, such as unauthorized access, loss, or damage. Imagine your data is locked away in a safe. Without the right key, no one can steal, tamper with, or even understand the information inside. Let's take a closer look at how encryption protects your data in different states. When data is at rest, it's stored on physical devices like computers or servers. By encrypting data at rest, even if someone gains physical access to the device, they won't be able to decipher the data without the encryption key. At Google Cloud, we automatically encrypt all customer content at rest, without any effort required from you. It's a free and built-in feature that adds an extra layer of protection to your valuable data. And if you prefer to manage your encryption keys yourself, you can use our Cloud Key Management Service (Cloud KMS) for added control. When data is in transit, it's moving over networks or the internet. Encryption plays a crucial role here by shielding your data from interception by cybercriminals or unauthorized parties. It's like sending your information in a locked box that only the intended recipient can open. At Google Cloud, we employ robust security measures to ensure the authenticity, integrity, and privacy of your data during transit. We encrypt and authenticate data at multiple network layers, especially when it travels outside the physical boundaries we control. This way, your information remains safe and secure as it journeys through the digital world. Data in use refers to data being actively processed by a computer. Encrypting data in use adds another layer of protection, especially against unauthorized users who might physically access the computer. We use a technique called memory encryption, which locks your data inside the computer's memory, making it nearly impossible for unauthorized users to gain access to it. When it comes to encryption algorithms, the Advanced Encryption Standard (AES) takes center stage. AES is a powerful encryption algorithm trusted by governments and businesses worldwide. It's like having a top-secret encryption method that keeps your data safe from prying eyes. So, whether your data is resting, traveling, or actively in use, encryption acts as your loyal guardian, because it ensures its confidentiality and protection. At Google Cloud, we take encryption seriously to provide you with a secure storage solution you can trust.

### Video - [Identity](https://www.cloudskillsboost.google/course_templates/945/video/487310)

- [YouTube: Identity](https://www.youtube.com/watch?v=3EavYtbPiRM)

Often referred to as the three A’s, authentication, authorization, and auditing are important aspects of cloud identity management used to ensure secure access, manage user privileges, and monitor resource usage. Let's begin with the first A, authentication. It serves as the gatekeeper, because it verifies the identity of users or systems that seek access. Authentication involves presenting unique credentials, such as passwords, physical tokens, or biometric data like fingerprints or voice recognition. Think of it as presenting your identification card before entering a restricted area. By validating the credentials provided, the server confirms that you are who you claim to be. Two-step verification, which you may also hear being referred to as two-factor authentication or multi-factor authentication, is a security feature that adds an extra layer of protection to cloud-based systems. With 2SV enabled, users need to provide two different pieces of information to log in. For example, it could be a combination of a password and a code sent to their phone through text message, voice call, or an app like Google Authenticator. This powerful feature makes unauthorized access more difficult, even if someone manages to obtain your password. The second A is authorization. After a user's identity is authenticated, authorization steps in to determine what that user or system is allowed to do within the system. Think of it as the access control mechanism. Different permissions are assigned to individuals or groups based on their roles, responsibilities, and organizational hierarchy. For example, a system administrator might have the authority to create and remove user accounts, whereas a standard user might only be able to view a list of other users. This fine-grained control ensures that each user has the appropriate level of access to perform their tasks while preventing unauthorized actions. The third A, auditing (sometimes referred to as accounting), plays a critical role in monitoring and tracking user activities within a system. By collecting and analyzing logs of user activity, system events, and other data, auditing helps organizations detect anomalies, security breaches, and policy violations. It provides a comprehensive record of actions taken on a system or resource, which proves invaluable during security incident investigations, compliance tracking, and system performance evaluation. Just like the surveillance cameras in a shopping mall, auditing keeps a watchful eye on activities happening within your system. To provide granular control over who has access to Google Cloud resources and what they can do with those resources, organizations can use Identity and Access Management (IAM). With IAM, you can create and manage user accounts, assign roles to users, grant and revoke permissions to resources, audit user activity, and monitor your security position. It provides a centralized and efficient approach to managing access control within your Google Cloud environment. Imagine IAM as your organization's security headquarters, equipped with robust tools to manage and safeguard your digital assets. By integrating IAM into your Google Cloud security strategy, you can ensure fine-grained access control, enhanced visibility, and centralized resource management. This empowers you to protect your organization's sensitive data and resources effectively.

### Video - [Network security](https://www.cloudskillsboost.google/course_templates/945/video/487311)

- [YouTube: Network security](https://www.youtube.com/watch?v=CiSfy-DuZMw)

When you expand your network to include cloud environments, security considerations take on a whole new dimension. Unlike traditional on-premises setups with clear perimeters, the cloud brings new possibilities and challenges. Let's explore some strategies to secure your organization's network and ensure the safety of your valuable data and workloads in Google Cloud. Embrace the power of zero trust networks. In the world of security, trust shouldn't be given freely. With Google Cloud's BeyondCorp Enterprise, you can implement a zero trust security model. It means that every access request is thoroughly verified, and both the user's identity and context are considered. This way, you maintain strict control over who can access your network and resources, both inside and outside your organization. Secure your connections to on-premises and multi-cloud environments. Many organizations have a mix of cloud and on-premises workloads, or they use multiple cloud providers for resiliency. Ensuring secure connectivity across these environments is crucial. Google Cloud provides private access methods through services like Cloud VPN and Cloud Interconnect, which let you establish secure connections between your on-premises networks and Google Cloud resources. Protect your perimeter with Google Cloud's powerful tools. Google Cloud offers various methods to help secure your perimeter, including firewalls and Virtual Private Cloud (VPC) Service Controls, which help you divide your cloud into different sections and keep them secure. You can also utilize Shared VPC, which is like having a large fence that separates each Google Cloud Project, so they can work independently and safely. With these tools, you can keep your cloud environment protected and give different teams their own space to work in. Stay ahead with a web application firewall. External web applications and services are often targeted by cyber threats, including DDoS attacks. DDoS, which stands for distributed denial-of-service, is a cyber attack that uses multiple compromised computer systems to flood a target with more traffic than it can handle, which causes a denial of service to legitimate users. Google Cloud Armor comes to the rescue by providing robust DDoS protection. It’s like a force field that stops harmful attacks and keeps your website or application safe from things that could make it stop working properly. Automate infrastructure provisioning for enhanced security. By adopting automation tools, you can create immutable infrastructure, which means that it can't be changed after provisioning. Think of infrastructure provisioning tools as your personal assistants for setting up and maintaining your cloud environment. When you use tools like Terraform, Jenkins, and Cloud Build, they handle all the behind-the-scenes work to create a secure and reliable cloud environment. It's like having a team of efficient workers who build and organize everything you need to run your environment smoothly. With these tools, your cloud environment becomes like a well-designed workspace where everything has its place and functions perfectly. And the best part is, when it's set up, it stays that way. No unexpected changes or disruptions. If anything does go wrong, these tools are there to quickly identify and fix any issue and ensure that your cloud environment keeps running smoothly. These examples illustrate just a few of the ways organizations use Google Cloud to fortify their networks against attacks. Your specific network setup and security measures will depend on your unique business requirements and risk tolerance.

### Video - [Security operations](https://www.cloudskillsboost.google/course_templates/945/video/487312)

- [YouTube: Security operations](https://www.youtube.com/watch?v=XvD_Z-tmbXU)

SecOps—short for Security Operations—is all about protecting your organization's data and systems in the cloud. It involves a combination of processes and technologies that help reduce the risk of data breaches, system outages, and other security incidents. Think of it as your secret weapon for keeping your valuable data safe. Let's explore some of the essential activities involved in SecOps. Vulnerability management is the process of identifying and fixing security vulnerabilities in cloud infrastructure and applications. It’s like regularly checking your castle walls for weak spots. Google Cloud's Security Command Center (SCC) provides a centralized view of your security posture. It helps to identify and fix vulnerabilities, and it ensures that your infrastructure remains solid and protected. Another crucial activity is log management. It's like having a watchful eye on your castle grounds, looking out for any suspicious activity. Google Cloud offers Cloud Logging, a service to collect and analyze security logs from your entire Google Cloud environment. It helps you detect and respond to any signs of trouble and ensures that you anticipate any potential threats. Of course, being prepared for security incidents is equally important. This is where incident response comes in. Imagine having a team of knights ready to defend your castle at a moment's notice. Google Cloud has expert incident responders across various domains, who are equipped with the knowledge and tools to tackle any security incident swiftly and effectively. Another crucial aspect of SecOps is educating your employees on security best practices. Just like teaching everyone in the castle to be vigilant and lock the gates, security awareness training helps prevent incidents by raising awareness and empowering employees to protect themselves and the organization. Now, you might be wondering, why should your organization implement SecOps? Well, here are the benefits. Reduced risk of data breaches: SecOps helps identify and fix vulnerabilities, which significantly reduces the risk of data breaches. Increased uptime: A swift and effective incident response minimizes the impact of outages on your business operations, which ensures smoother and uninterrupted services. Improved compliance: SecOps helps with meeting security regulations, such as the General Data Protection Regulation (GDPR), and keeps your organization in good standing. Enhanced employee productivity: By educating employees on security best practices, SecOps minimizes the risk of human error and promotes a more secure and productive work environment. SecOps is an integral part of your organization's security strategy. By implementing SecOps practices, you can fortify your defenses, reduce security risks, and protect your data in the ever-changing landscape of cloud security.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/945/quizzes/487313)

#### Quiz 1.

> [!important]
> **What security feature adds an extra layer of protection to cloud-based systems?**
>
> - [ ] Security information and event management (SIEM)
> - [ ] Firewall as a service (FaaS)
> - [ ] Data loss prevention (DLP)
> - [ ] Two-step verification (2SV)

#### Quiz 2.

> [!important]
> **Google Cloud encrypts data at various states. Which state refers to when data is being actively processed by a computer?**
>
> - [ ] Data at rest
> - [ ] Data lake
> - [ ] Data in transit
> - [ ] Data in use

#### Quiz 3.

> [!important]
> **Which aspect of cloud identity management verifies the identity of users or systems?**
>
> - [ ] Authentication
> - [ ] Auditing
> - [ ] Authorization
> - [ ] Accounting

#### Quiz 4.

> [!important]
> **What Google Cloud product provides robust protection from harmful distributed denial-of-service (DDoS) attacks?**
>
> - [ ] IAM
> - [ ] Cloud Load Balancing
> - [ ] Cloud Monitoring
> - [ ] Google Cloud Armor

#### Quiz 5.

> [!important]
> **What metric does Google Cloud use to measure the efficiency of its data centers to achieve cost savings and a reduced carbon footprint?**
>
> - [ ] Data Center Infrastructure Efficiency (DCiE)
> - [ ] Power Usage Effectiveness (PUE)
> - [ ] Total cost of ownership (TCO)
> - [ ] Energy Efficiency Ratio (EER)

#### Quiz 6.

> [!important]
> **Select the correct statement about Identity and Access Management (IAM).**
>
> - [ ] IAM is a cloud security information and event management solution that collects and analyzes log data from cloud security devices and applications.
> - [ ] IAM is a system that detects and prevents malicious traffic from entering a cloud network.
> - [ ] IAM is a cloud service that encrypts cloud-based data at rest and in transit.
> - [ ] IAM provides granular control over who has access to Google Cloud resources and what they can do with those resources.

#### Quiz 7.

> [!important]
> **Which is a powerful encryption algorithm trusted by governments and businesses worldwide?**
>
> - [ ] Isomorphic encryption (IE)
> - [ ] Lattice-Based Cryptography (LBC)
> - [ ] Post-quantum cryptography (PQC)
> - [ ] Advanced Encryption Standard (AES)

#### Quiz 8.

> [!important]
> **Which practice involves a combination of processes and technologies that help reduce the risk of data breaches, system outages, and other security incidents in the cloud?**
>
> - [ ] Cloud security posture management (CSPM)
> - [ ] Site reliability engineering (SRE)
> - [ ] Zero trust security
> - [ ] Security operations (SecOps)

## Google Cloud’s Trust Principles and Compliance

In this section of the course, you learn how Google Cloud's trust principles, transparency reports, and independent third-party audits support customer trust. You also explore the importance of data sovereignty and data residency, and how the Google Cloud compliance resource center and Compliance Reports Manager supports industry and regional compliance needs.

### Video - [Introduction](https://www.cloudskillsboost.google/course_templates/945/video/487314)

- [YouTube: Introduction](https://www.youtube.com/watch?v=zT_97zNbdzo)

At Google, we know that privacy plays a critical role in earning and maintaining trust. Customers need to be sure that their data and applications are safe and secure, and so Google Cloud has a strong set of trust principles and compliance programs in place, which are designed to protect customer data and meet the needs of a wide range of customers, from small businesses to large enterprises. In this final section of the course, you learn about Google’s seven trust principles, data residency and data sovereignty options with Google Cloud, and how the Google Cloud compliance resource center and Compliance Reports Manager support industry and regional compliance needs.

### Video - [The Google Cloud Trust Principles and Transparency Reports](https://www.cloudskillsboost.google/course_templates/945/video/487315)

- [YouTube: The Google Cloud Trust Principles and Transparency Reports](https://www.youtube.com/watch?v=1SX2fD3j0jw)

At Google, we believe in transparency and want you to have complete confidence in our services. Google Cloud’s trust principles are designed to empower you and ensure that the security and control of your business data is not compromised. Let’s review these principles. 1. You own your data, not Google. We prioritize your control and let you access, export, delete, and manage data permissions within Google Cloud. 2. Google does not sell customer data to third parties. We safeguard your data from being used for Google's marketing or advertising purposes. 3. Google Cloud does not use customer data for advertising. Your data remains confidential, because Google Cloud ensures that it’s never utilized to target ads. 4. All customer data is encrypted by default. Your data is protected with robust encryption, because Google Cloud safeguards it even in the unlikely event of unauthorized access. 5. We guard against insider access to your data. We implement stringent security measures to prevent unauthorized employee access to customer data. 6. We never give any government entity "backdoor" access. Your data remains secure, and no government entity can access it without proper authorization. And 7. Our privacy practices are audited against international standards. We undergo regular audits to ensure compliance with rigorous privacy standards. Transparency Reports and Independent Audits Transparency are a core element of our commitment to trust. We provide valuable insights and accountability through our transparency reports, which shed light on government and corporate actions that affect privacy, security, and access to information. These reports let you stay informed and maintain trust in our services. Additionally, Google Cloud undergoes independent, third-party audits and certifications. This verification process ensures that our data protection practices align with our commitments and industry standards. Our participation in initiatives like the EU Cloud Code of Conduct further reinforces our dedication to accountability, compliance support, and robust data protection principles.

### Video - [Data residency and data sovereignty](https://www.cloudskillsboost.google/course_templates/945/video/487316)

- [YouTube: Data residency and data sovereignty](https://www.youtube.com/watch?v=xcJi4SX6lXw)

When it comes to storing data and keeping it secure, data sovereignty and data residency are two important concepts to understand. Data sovereignty refers to the legal concept that data is subject to the laws and regulations of the country where it resides. For example, the General Data Protection Regulation (GDPR) in the European Union requires companies to comply with data protection laws when processing or storing personal data of EU citizens, regardless of their location. This ensures that individuals have control over their personal data and its usage. In contrast, data residency refers to the physical location where data is stored or processed. Some countries or regions have laws or regulations that require data to be stored within their borders. For instance, some countries mandate that personal data of its citizens must be stored on servers within the country. This ensures data remains within the jurisdiction of local laws. Now, let's explore how Google Cloud addresses data residency requirements. We offer a range of options to control the physical location of your data through regions. Each region consists of one or more data centers, which lets you choose where your data resides. For example, within the European Union, you can select regions located in various countries like the UK, Belgium, Germany, Finland, Switzerland, and the Netherlands. By configuring your resources in specific regions, Google ensures that your data is stored only within the selected region, as stated in our Service Specific Terms. Additionally, Google Cloud provides Organization Policy constraints, coupled with IAM configuration, to prevent accidental data storage in the wrong region. These controls offer peace of mind and reinforce your data residency requirements. Furthermore, Google Cloud offers features like VPC Service Controls, which let you restrict network access to data based on defined perimeters. You can limit user access through IP address filtering, even if they have authorization. Google Cloud Armor lets you restrict traffic locations for your external load balancer by adding an extra layer of protection. By using these capabilities, organizations can adhere to data residency and data sovereignty requirements, ensure compliance, and maintain control over their valuable data within the Google Cloud ecosystem.

### Video - [Industry and regional compliance](https://www.cloudskillsboost.google/course_templates/945/video/487317)

- [YouTube: Industry and regional compliance](https://www.youtube.com/watch?v=UylDMleaGE4)

As organizations migrate to the cloud, it becomes essential to protect sensitive workloads while ensuring compliance with diverse regulatory requirements and guidelines. Compliance is a critical aspect of the cloud journey, because not meeting regulatory obligations can have far-reaching consequences. To assist you in achieving compliance, Google Cloud offers robust resources and tools tailored to support your specific needs. First, let's explore the Google Cloud compliance resource center. This comprehensive hub provides detailed information on the certifications and compliance standards we satisfy. You can find mappings of our security, privacy, and compliance controls to global standards. This transparency lets you validate our adherence to industry-leading practices. The resource center also offers valuable documentation on regional and sector-specific regulations, and empowers you to navigate complex compliance landscapes. Imagine you're a healthcare organization subject to HIPAA regulations, which protect sensitive patient health information from being disclosed without the patient's consent or knowledge. The resource center equips you with the necessary insights and documentation to align your compliance efforts with HIPAA requirements. Similarly, if you operate within the financial sector, you'll find guidance on meeting regulations like PCI DSS, which stands for Payment Card Industry Data Security Standard. Google Cloud's compliance resource center is your go-to source for actionable information and support. In addition to the resource center, we provide the Compliance Reports Manager, a powerful tool at your disposal. This intuitive platform offers easy, on-demand access to critical compliance resources at no extra cost. Within the Compliance Reports Manager, you'll discover our latest ISO/IEC certificates, SOC reports, and self-assessments. These resources provide evidence of our adherence to rigorous compliance standards and help streamline your own reporting and compliance efforts. Imagine you're an enterprise seeking ISO/IEC 27001 certification. The Compliance Reports Manager lets you access the necessary documentation efficiently, and it saves you time and effort in the certification process. With this tool, we aim to simplify your compliance journey and empower you to meet your regulatory obligations effectively. By using the Google Cloud compliance resource center and the Compliance Reports Manager, you can navigate the complex realm of industry and regional compliance with confidence. Our dedicated teams of engineers and compliance experts work hand in hand with you to address your specific regulatory needs. Together, we create an integrated controls and governance framework, while we ensure a robust compliance posture. You can visit the compliance resource center at cloud.google.com/security/compliance and explore the Compliance Reports Manager at cloud.google.com/security/compliance/compliance-reports-manager.

### Quiz - [Quiz](https://www.cloudskillsboost.google/course_templates/945/quizzes/487318)

#### Quiz 1.

> [!important]
> **Which is one of Google Cloud's seven trust principles?**
>
> - [ ] Google Cloud uses customer data for advertising.
> - [ ] We give "backdoor" access to government entities when requested.
> - [ ] All customer data is encrypted by default.
> - [ ] Google sells customer data to third parties.

#### Quiz 2.

> [!important]
> **Which report provides a way for Google Cloud to share data about how the policies and actions of governments and corporations affect privacy, security, and access to information?**
>
> - [ ] Billing reports
> - [ ] Compliance reports
> - [ ] Security reports
> - [ ] Transparency reports

#### Quiz 3.

> [!important]
> **Where can you find details about certifications and compliance standards met by Google Cloud?**
>
> - [ ] Google Cloud console
> - [ ] Cloud Storage client libraries
> - [ ] Marketplace
> - [ ] Compliance resource center

#### Quiz 4.

> [!important]
> **Which term describes the concept that data is subject to the laws and regulations of the country where it resides?**
>
> - [ ] Data consistency
> - [ ] Data redundancy
> - [ ] Data residency
> - [ ] Data sovereignty

#### Quiz 5.

> [!important]
> **Which Google Cloud feature allows users to control their data's physical location?**
>
> - [ ] Places
> - [ ] Districts
> - [ ] Areas
> - [ ] Regions

## Course Summary

The course closes with a summary of the main points covered in each section and next steps to continue learning.

### Video - [Course summary](https://www.cloudskillsboost.google/course_templates/945/video/487319)

- [YouTube: Course summary](https://www.youtube.com/watch?v=leWsaLAyePU)

This brings us to the end of the “Trust and Security with Google Cloud” course. Let’s do a quick recap. In the first section of the course titled, “Trust and security in the cloud,” you explored important security terms and concepts, the difference between cloud security and traditional on-premises security, today’s top cybersecurity threats and business implications, and the importance of control, compliance, confidentiality, integrity, and availability in a cloud security model. In the second section of the course, titled “Google’s trusted infrastructure,” you learned about how Google designs and builds data centers, the role encryption plays in securing an organization’s data, the differences between authentication, authorization, and auditing, the benefits of using two-step verification and IAM, ways to protect against network attacks by using Google products, and security operations in the cloud and its related business benefits. And finally, in the third section of the course, titled “Google Cloud’s trust principles and compliance,” you examined Google’s seven trust principles, data residency and data sovereignty options with Google Cloud, and how the Google Cloud compliance resource center and Compliance Reports Manager support industry and regional compliance needs. Now that you had a comprehensive introduction to trust and security on Google Cloud, you can move on to the final course in the Cloud Digital Leader series, “Scaling with Google Cloud Operations,” where you’ll learn about how Google Cloud supports an organization's financial governance and ability to control their cloud costs, the basic concepts of modern operations, reliability, and resilience in the cloud, and how Google Cloud helps organizations meet sustainability goals and reduce environmental impact. We’ll see you next time!

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
