---
id: 48
name: 'Google Workspace Security'
datePublished: 2025-04-08
topics: []
type: Course
url: https://www.cloudskillsboost.google/course_templates/48
---

# [Google Workspace Security](https://www.cloudskillsboost.google/course_templates/48)

**Description:**

This course empowers learners to secure their Google Workspace environment. Learners will implement strong password policies and two-step verification to govern user access. They will then utilize the security investigation tool to proactively identify and respond to security risks. Next, they will manage third-party app access and mobile devices to ensure security. Finally, learners will enforce email security and compliance measures to protect organizational data.

**Objectives:**

- Configure Google Workspace security settings to enforce strong authentication, manage user access controls, and protect against unauthorized access.
- Use Google Workspace security tools to proactively identify, analyze, and respond to security risks.
- Manage third-party application access and deployment within your Google Workspace environment.
- Manage mobile devices within Google Workspace to ensure security, compliance, and productivity.

## Google Workspace Security

This course empowers learners to secure their Google Workspace environment. Learners will implement strong password policies and two-step verification to govern user access. They will then utilize the security investigation tool to proactively identify and respond to security risks. Next, they will manage third-party app access and mobile devices to ensure security. Finally, learners will enforce email security and compliance measures to protect organizational data.

### Video - [Welcome](https://www.cloudskillsboost.google/course_templates/48/video/529872)

- [YouTube: Welcome](https://www.youtube.com/watch?v=gCdxq6qz9xI)

[NO AUDIO]

### Link - [Create your Google Workspace trial account](https://www.cloudskillsboost.google/course_templates/48/documents/529873)

- [Create your Google Workspace trial account](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b4b251061acd7e39cdde9f)

### Video - [Common Google Workspace security setting](https://www.cloudskillsboost.google/course_templates/48/video/529874)

- [YouTube: Common Google Workspace security setting](https://www.youtube.com/watch?v=6jEYSGfBLpY)

[NO AUDIO]

### Link - [Configure common security settings](https://www.cloudskillsboost.google/course_templates/48/documents/529875)

- [Configure common security settings](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b598978e924166c17516c0)

### Link - [Assign Administrator roles](https://www.cloudskillsboost.google/course_templates/48/documents/529876)

- [Assign Administrator roles](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b6fccf8c1a269697c25e8d)

### Link - [Manage access policies](https://www.cloudskillsboost.google/course_templates/48/documents/529877)

- [Manage access policies](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b70621c7c5624eaf2633b1)

### Video - [Use of an exception group](https://www.cloudskillsboost.google/course_templates/48/video/529878)

- [YouTube: Use of an exception group](https://www.youtube.com/watch?v=HmyxcWXWVxo)

SPEAKER: In a previous exercise, you applied a two-step verification enforcement policy to a single Organizational Unit, or OU. Now, consider a situation where you want to apply the policy to only some members of an OU. What do you do? You could move the users who aren't required to enroll in two-step verification into another OU. But then you'd need to manage policies for multiple OUs where previously you had everyone in one place. This isn't ideal, because it adds to the complexity of your organizational structure. A solution would be to use an exception group. Exception groups make it easier to turn two-step verification on or off by OU. To do so, you first create a group and put all the users who are exempt from enrollment into that group. Next, enforce the policy for the OU, and then disable enforcement for the group. The policy settings you give to the group are applied to the intersection of the OU and group, which means users who are members of both. The same approach could be used to enforce enrollment for only a subset of OU members. In that case, you'd enforce for the group, but turn enforcement off for the OU.

### Quiz - [Quiz: Common security settings](https://www.cloudskillsboost.google/course_templates/48/quizzes/529879)

### Video - [Security center](https://www.cloudskillsboost.google/course_templates/48/video/529880)

- [YouTube: Security center](https://www.youtube.com/watch?v=jYGe8wHzIPE)

SPEAKER: An important part of an administrator's toolkit is the security center. Now, access to the security center will vary depending on which edition of Google Workspace that you use. But it's here that you can find security best practice recommendations from Google, analytics, and actionable insights to empower you to protect your organization, data, and users. Let's explore the security center in the Google Admin console. We'll begin with the security health page, which is designed to help you better understand and manage security risks. From this page, you can monitor the configuration of your Google Workspace account. For example, you can check the status of settings like automatic email forwarding, device encryption, Drive sharing settings, and much more. This information can help identify potential account modifications that should be made to your domain settings based on general security guidelines and best practices while weighing your organization's business needs and risk management policy. Next is the security dashboard, which provides an overview of different security reports. It's here, for example, that you can see external file share activity, how many messages are authenticated, suspicious device activities, failed password attempts, and more. The dashboard panels display the percentage change over time of the data. This lets you easily view trends like whether external file sharing has increased or decreased during a specific time period. The underlying reports can be opened from the dashboard panels. There are also options to filter and export data as required. The third and final component in the security center is the security investigation tool. As the administrator, you can use this tool to identify, triage, and act on security and privacy issues in your domain. You might access device log data to get a clear view of the devices and applications being used to access your data, access data about Gmail messages, including message content, access Gmail log data to find and erase malicious emails, mark emails as spam or phishing, or send emails to users' inboxes, or access Drive log data to investigate file sharing in your organization, the creation and deletion of documents, who accessed documents, and more. Once you've used the investigation tool, you can act on the results of your searches. For example, you might conduct a search based on Gmail log events and then use the investigation tool to delete specific messages, mark messages as spam or phishing, send messages to quarantine, or send messages to users' inboxes. Searches made using the investigation tool can be saved and shared with others. You can also add them as a new chart to the security dashboard for quick access.

### Link - [Security center](https://www.cloudskillsboost.google/course_templates/48/documents/529881)

- [Security center](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b721e0b794db8fd8a799c8)

### Video - [Activity rules](https://www.cloudskillsboost.google/course_templates/48/video/529882)

- [YouTube: Activity rules](https://www.youtube.com/watch?v=QH1MtMENRkA)

[NO AUDIO]

### Link - [Create activity rules and alerts](https://www.cloudskillsboost.google/course_templates/48/documents/529883)

- [Create activity rules and alerts](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b71a96b794db8fd8a232a0)

### Quiz - [Quiz: Security tools](https://www.cloudskillsboost.google/course_templates/48/quizzes/529884)

### Video - [Introduction to application security](https://www.cloudskillsboost.google/course_templates/48/video/529885)

- [YouTube: Introduction to application security](https://www.youtube.com/watch?v=Uy377wrEQ3I)

[NO AUDIO]

### Link - [Configure SSO in third-party applications](https://www.cloudskillsboost.google/course_templates/48/documents/529886)

- [Configure SSO in third-party applications](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b811e8b794db8fd8af12ac)

### Link - [Manage connected apps](https://www.cloudskillsboost.google/course_templates/48/documents/529887)

- [Manage connected apps](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b816f8b794db8fd8aff870)

### Link - [The Google Workspace Marketplace](https://www.cloudskillsboost.google/course_templates/48/documents/529888)

- [The Google Workspace Marketplace](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b81af8b794db8fd8b12d70)

### Link - [Automatically install apps and extensions](https://www.cloudskillsboost.google/course_templates/48/documents/529889)

- [Automatically install apps and extensions](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b6f14a36ada5a258605d97)

### Quiz - [Quiz: Application security](https://www.cloudskillsboost.google/course_templates/48/quizzes/529890)

### Video - [Manage mobile devices](https://www.cloudskillsboost.google/course_templates/48/video/529891)

- [YouTube: Manage mobile devices](https://www.youtube.com/watch?v=HYRPqtdpVwc)

[NO AUDIO]

### Link - [Basic mobile management](https://www.cloudskillsboost.google/course_templates/48/documents/529892)

- [Basic mobile management](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b6fb5436ada5a25860de06)

### Link - [Advanced mobile management](https://www.cloudskillsboost.google/course_templates/48/documents/529893)

- [Advanced mobile management](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b81f49b794db8fd8b31af6)

### Video - [Endpoint Verification](https://www.cloudskillsboost.google/course_templates/48/video/529894)

- [YouTube: Endpoint Verification](https://www.youtube.com/watch?v=uygZKeo_KFs)

[NO AUDIO]

### Link - [Chrome browser policies](https://www.cloudskillsboost.google/course_templates/48/documents/529895)

- [Chrome browser policies](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67b727ad762f04d4ccc628e1)

### Link - [Third-party management](https://www.cloudskillsboost.google/course_templates/48/documents/529896)

- [Third-party management](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67bc44d1ae51f04b3edb47e6)

### Quiz - [Quiz: Endpoint security](https://www.cloudskillsboost.google/course_templates/48/quizzes/529897)

### Video - [Email security](https://www.cloudskillsboost.google/course_templates/48/video/529898)

- [YouTube: Email security](https://www.youtube.com/watch?v=dAIA4iXZW2I)

[NO AUDIO]

### Link - [Email security practices](https://www.cloudskillsboost.google/course_templates/48/documents/529899)

- [Email security practices](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67bc5e9556e7e93ea94fea0d)

### Video - [Compliance](https://www.cloudskillsboost.google/course_templates/48/video/529900)

- [YouTube: Compliance](https://www.youtube.com/watch?v=8hzRozK65nk)

[NO AUDIO]

### Link - [Email content filtering](https://www.cloudskillsboost.google/course_templates/48/documents/529901)

- [Email content filtering](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67bc741356e7e93ea957a848)

### Video - [Preventing spam, phishing, and malware](https://www.cloudskillsboost.google/course_templates/48/video/529902)

- [YouTube: Preventing spam, phishing, and malware](https://www.youtube.com/watch?v=dZ8ym7wAB_E)

[NO AUDIO]

### Link - [Advanced email security](https://www.cloudskillsboost.google/course_templates/48/documents/529903)

- [Advanced email security](https://storage.googleapis.com/cloud-training/S-GSAD/T-GSSU-I%20%7C%20Google%20Workspace%20Security/index.html#/page/67bc7f8856e7e93ea95a8324)

### Quiz - [Quiz: Email security](https://www.cloudskillsboost.google/course_templates/48/quizzes/529904)

### Video - [Course recap](https://www.cloudskillsboost.google/course_templates/48/video/529905)

- [YouTube: Course recap](https://www.youtube.com/watch?v=t8qM-sOaxdY)

[NO AUDIO]

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
