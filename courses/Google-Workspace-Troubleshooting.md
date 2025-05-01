---
id: 1280
name: 'Google Workspace Troubleshooting'
type: Course
url: https://www.cloudskillsboost.google/course_templates/1280
date_published: 2025-04-17
topics:

---

# [Google Workspace Troubleshooting](https://www.cloudskillsboost.google/course_templates/1280)

**Description:**

This course was designed to prepare Google Workspace Administrators to troubleshoot common Google Workspace issues. Learners will practice diagnosing and resolving problems in Gmail, Calendar, and Drive, and navigating the Admin console. They will also experience analyzing audit logs to troubleshoot security issues, and gathering information and using available resources to troubleshoot and report technical issues.

**Objectives:**

* Diagnose and resolve common Google Calendar syncing and sharing issues.
* Diagnose and resolve email delivery issues within Google Workspace.
* Resolve common Google Drive access, synchronization, and data recovery issues.
* Analyze audit logs to troubleshoot security-related issues within Google Workspace.

## Google Workspace Troubleshooting

This course was designed to prepare Google Workspace Administrators to troubleshoot common Google Workspace issues. Learners will practice diagnosing and resolving problems in Gmail, Calendar, and Drive, and navigating the Admin console. They will also experience analyzing audit logs to troubleshoot security issues, and gathering information and using available resources to troubleshoot and report technical issues.

### Video - [Welcome](https://www.cloudskillsboost.google/course_templates/1280/video/530796)

* [YouTube: Welcome](https://www.youtube.com/watch?v=Lt9Tbittfw0)

SPEAKER: Welcome to the Google Workspace Troubleshooting course. In this course, you'll focus on diagnosing and resolving common issues with Google Workspace. To start, you'll learn how to troubleshoot and investigate security-related issues using audit logs. Next, you'll resolve common issues in Google Calendar, Gmail, and Drive. And finally, you'll explore available support resources for troubleshooting technical issues in Google Workspace. Lessons include a mix of videos, hands-on exercises, links to Help Center articles, and quizzes to help you evaluate what you've learned. This is the fifth course in the Google Workspace administration series. So before starting this course, please be sure to complete the courses titled Google Workspace User and Resource Management, Google Workspace Core Services, Google Workspace Data Governance, and Google Workspace Security. If you've previously completed those courses but no longer have your trial domain, please be sure to complete the exercise that follows this video. However, if your trial domain is still valid, you can skip that exercise.

### Link - [Create your Google Workspace trial account](https://www.cloudskillsboost.google/course_templates/1280/documents/530797)

* [Create your Google Workspace trial account](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67dabfd398bd62c1806cc475)

### Video - [Audit logs](https://www.cloudskillsboost.google/course_templates/1280/video/530798)

* [YouTube: Audit logs](https://www.youtube.com/watch?v=izukc17Cx9s)

SPEAKER: When investigating your users' problems, you might want to know who did what, where, and when. Google Cloud Services write audit logs to help you answer those exact questions. You can share your Google Workspace audit logs with Google Cloud to store, analyze, monitor, and alert you about your Google Workspace data. Google Workspace provides the following audit logs at the Google Cloud organization level, access transparency logs, admin audit logs, enterprise groups audit logs, login audit logs, OAuth token audit logs, and SAML audit logs. Let's explore these audit logs in a little more detail. Access transparency logs provide a record of actions when Google personnel access user content in your Google Workspace resources. This includes text that users have entered into Gmail, Google Docs, Google Sheets, Google Slides, and other Google Workspace apps. These logs can help identify unusual activity and potential security risks within your workspace environment. Admin audit logs provide a record of actions performed in your Google Admin Console. For example, you can see when an administrator added a user or turned on a Google Workspace service. Enterprise groups audit logs provide a record of actions performed on groups and group memberships. For example, you can see when an administrator added a user or when a group owner deleted their group. Login audit logs track user sign-in to your domain. These logs only record the login event and not the system used to perform the login action. Login audit logs can help identify suspicious sign-in attempts. OAuth token audit logs track which users are using which third-party mobile or web applications in your domain. For example, when a user opens a Google Workspace Marketplace app, the log records the name of the app and the person using it. The log also records each time a third-party application is authorized to access Google account data, such as Google Contacts, Calendar, and Drive files. And finally, SAML audit logs track user successful and failed sign-ins to SAML applications. SAML stands for Security Assertion Markup Language. Entries usually appear within an hour of the user action.

### Link - [Collect and analyze logs](https://www.cloudskillsboost.google/course_templates/1280/documents/530799)

* [Collect and analyze logs](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67dd02fc57a13185b17fd2c7)

### Quiz - [Quiz: Audit logs](https://www.cloudskillsboost.google/course_templates/1280/quizzes/530800)

#### Quiz 1.

> [!important]
> **Where in the Google Admin console can you find audit logs of Admin and user actions?**
>
> * [ ] The Security section
> * [ ] The System tools section
> * [ ] The Reporting section
> * [ ] The User management tools section

#### Quiz 2.

> [!important]
> **What tool can be used to view a record of actions performed in the Google Workspace Admin console?**
>
> * [ ] The Audit and investigation tool
> * [ ] The Security health page
> * [ ] The Security alert center
> * [ ] App reports

#### Quiz 3.

> [!important]
> **You need to determine which user in your organization recently modified the visibility settings for their scheduled meetings, specifically regarding who can view the details of those events. Which data source in the Audit and investigation tool would provide the most relevant log files for this investigation?**
>
> * [ ] Google Meet logs
> * [ ] Google Chat logs
> * [ ] The User log
> * [ ] Google Calendar logs

### Video - [Troubleshooting Google Calendar issues](https://www.cloudskillsboost.google/course_templates/1280/video/530801)

* [YouTube: Troubleshooting Google Calendar issues](https://www.youtube.com/watch?v=2gUm4slNglg)

SPEAKER: As an administrator, it's critical to ensure that Google Calendar runs smoothly to facilitate efficient collaboration and scheduling within your organization. When users have issues with their Google Calendar, such as events not syncing, difficulty managing sharing permissions, or trouble sharing their availability, they'll rely on you to help diagnose and resolve them. Let's explore some common issues your users might face with Google Calendar. Sometimes users run into problems where their event invitations don't sync properly between their Google Calendar and another email provider, like Microsoft Outlook. One reason this might happen is that the user has chosen an unlimited mailbox size limit in the Google Workspace sync for Microsoft Outlook. This setting can sometimes interfere with how Calendar events are synced. Another thing that can cause problems is if the user has reorganized their mailbox by dragging folders to different locations. This can disrupt the sync process as well. To figure out exactly what's going wrong, you can use a Workspace admin tool called Log Analyzer. By submitting the user's trace logs, Log Analyzer can usually pinpoint the sync issue within minutes. If you need more advanced analysis, you can submit their uncompressed files to Log Analyzer 2. Sometimes a user might contact you because they can't share their calendar, even though they should have the necessary permissions. This can be frustrating for them and you. If you've double checked their individual settings and everything looks correct, the problem might lie in the broader sharing settings for your organization. To fix this, you might need to adjust the external sharing options for the entire organization or just for the specific organizational unit that the user belongs to. And finally, let's say a user reports that they can't see the availability, free or busy information for resources, like meeting rooms or equipment, when they're trying to schedule something. Often, this happens because the user isn't signed in to the Google Workspace account where the resources and their availability are managed. Another possibility is that, even with a Workspace account, the user might not have the correct settings configured in their calendar to view resource availability. So if you come across this situation, it's worth checking those two things first.

### Link - [Calendar issues](https://www.cloudskillsboost.google/course_templates/1280/documents/530802)

* [Calendar issues](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67dd078557a13185b180499a)

### Quiz - [Quiz: Troubleshooting Google Calendar issues](https://www.cloudskillsboost.google/course_templates/1280/quizzes/530803)

#### Quiz 1.

> [!important]
> **A user reports colleagues can't see their free/busy information in Google Calendar when they schedule meetings. Which troubleshooting step directly addresses this issue?**
>
> * [ ] Confirm that the user's calendar is checked for visibility in their colleagues' calendar list.
> * [ ] Ensure the user has updated their Google Calendar app and cleared their cache.
> * [ ] Inspect the settings related to the user's Google Calendar visibility options.
> * [ ] Verify the user's general calendar sharing permissions for event details are correctly configured.

#### Quiz 2.

> [!important]
> **A user reports a colleague they shared their Google Calendar with can only see that the calendar is shared, not event details. Which troubleshooting step can resolve this issue?**
>
> * [ ] Check the sharing permission settings for the calendar.
> * [ ] Check if Google Calendar is experiencing a service outage.
> * [ ] Clear the browser's cache and cookies.
> * [ ] Restart the user's computer or mobile device.

#### Quiz 3.

> [!important]
> **A user reports that changes made in the Calendar application available through Apple are not consistently syncing to their Google Calendar, even though they should. Which troubleshooting step would best address this synchronization issue?**
>
> * [ ] Ensure that the user's Google Calendar app is updated to the latest version.
> * [ ] Verify that the user's internet connection is stable.
> * [ ] Confirm that the user has checked the visibility of their Google Calendar within the app menu of Google Calendar.
> * [ ] Ensure the user is selecting the correct Google Calendar account within the Calendar application available through Apple when creating new events.

### Video - [Troubleshooting mail issues](https://www.cloudskillsboost.google/course_templates/1280/video/530804)

* [YouTube: Troubleshooting mail issues](https://www.youtube.com/watch?v=tCFKQf5xCyg)

SPEAKER: When your users run into issues with sending and receiving mail, it's important that how to diagnose and resolve these issues as well as recommend policy changes to prevent future issues. Let's explore some common problems your users might encounter with Gmail. At times, users run into problems with their Gmail accounts, which can range from something as simple as being unable to sign in to more serious issues like missing emails or seeing incorrect information. When these situations arise, your role will be to guide the user towards a solution. Sometimes you might need to directly access their account and manually update their settings to resolve a problem. Other times, the fix might be something the user can handle themselves, like resetting their password or updating their profile information. You'll need to assess each situation and determine the best course of action. A common type of issue users might have is with sending or receiving emails in Gmail. For example, messages might not be delivered or forwarded correctly. Or they might bounce back due to a policy violation. To uncover email delivery and routing issues, you can use the Messageheader tool in the Google Admin Toolbox. If the issue is related to DNS record, you can also use the Check MX tool to ensure that the records are configured correctly. And finally, if your users are receiving spam messages or having legitimate messages marked as spam, you might need to recommend a mail policy change for your organization, such as setting up SPF, DKIM, or DMARC. Sender Policy Framework, or SPF, helps prevent senders from impersonating you. It blocks spammers and other attackers from sending emails that appear to be from your organization. DomainKeys Identified Mail, or DKIM, prevents the contents of your message from being changed during transit. And Domain-based Message Authentication, Reporting, and Conformance, or DMARC, lets you tell receiving mail servers what to do when they get a message that doesn't pass SPF or DKIM authentication checks. You can also get reports that help you identify possible authentication issues and malicious activity for messages sent from your domain. In general, it's recommended to always set up all three of these email authentication methods for the domain that hosts your public website.

### Link - [Email delivery issues](https://www.cloudskillsboost.google/course_templates/1280/documents/530805)

* [Email delivery issues](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67dd0c3257a13185b180cf1b)

### Link - [Email audit investigation](https://www.cloudskillsboost.google/course_templates/1280/documents/530806)

* [Email audit investigation](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67dd0ee457a13185b181255c)

### Link - [Implementing mail policy changes](https://www.cloudskillsboost.google/course_templates/1280/documents/530807)

* [Implementing mail policy changes](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67dd2b0d57a13185b1828edf)

### Quiz - [Quiz: Troubleshooting mail issues](https://www.cloudskillsboost.google/course_templates/1280/quizzes/530808)

#### Quiz 1.

> [!important]
> **One of your users has reported they haven't been receiving emails from an external client. Which step should you take to diagnose the issue?**
>
> * [ ] Use Email Log Search (ELS) to track the delivery status of the specific email.
> * [ ] Review the spam filter report in the Security Dashboard for general trends.
> * [ ] Add the client's domain to the spam bypass filter.
> * [ ] Encourage the recipient to mark future emails from that client as "Not Spam."

#### Quiz 2.

> [!important]
> **A user reports that emails with a specific keyword are consistently given an unexpected Gmail label. Which troubleshooting step can be used to diagnose this issue?**
>
> * [ ] Analyze the message header of an affected email using Google's Messageheader tool.
> * [ ] Verify automatic forwarding is enabled in the Google Admin console.
> * [ ] Use Email Log Search to review the delivery status of the affected emails.
> * [ ] Review the user's Gmail filter criteria for rules related to the keyword.

#### Quiz 3.

> [!important]
> **Your organization is experiencing an increase in suspected phishing emails. To verify the authentication of incoming emails and identify potentially spoofed senders (using SPF, DMARC, and DKIM), which Google Workspace tool would you use?**
>
> * [ ] Filter settings in Gmail
> * [ ] Forwarding settings in the Google Admin consoles
> * [ ] Email Log Search
> * [ ] Messageheader in the Google Admin Toolbox

#### Quiz 4.

> [!important]
> **Your organization's security team has identified a recurring issue of unauthorized external domains sending emails that appear to originate from internal user accounts. To mitigate this risk, which mail policy change would you recommend implementing?**
>
> * [ ] Restrict delivery to only authorized addresses and domains.
> * [ ] Adjust Gmail filter settings for individual users.
> * [ ] Enable the SMTP Relay Service and designate "Any addresses" as allowed senders.
> * [ ] Set up an Outbound Gateway.

### Video - [Troubleshooting Google Drive issues](https://www.cloudskillsboost.google/course_templates/1280/video/530809)

* [YouTube: Troubleshooting Google Drive issues](https://www.youtube.com/watch?v=i9oGixEn0YU)

SPEAKER: As an administrator, your users might have issues with sharing and managing permissions within Google Drive. They'll be looking to you for guidance on how to fix these problems. Let's explore some common issues that users face with shared drives and how they can be solved. First, users sometimes have issues creating and managing shared drives. Common problems a user experiences are that they can't create a shared drive, can't add a member to a shared drive, can't delete a shared drive, can't share a file or folder in a shared drive, or can't move a folder from My Drive to a shared drive. These issues typically occur because the user doesn't have the right permissions to perform the action or because the shared drive itself has been set up in a way that prevents the action. For instance, a user might not be able to add a member to a shared drive if the organization's sharing policies restrict external users and that user is trying to add someone outside of the organization. Second, your users might encounter issues with file syncing or unexpected crashes when using Drive for desktop. For example, changes made to a file on their computer aren't reflected in the cloud. This might be caused by a variety of factors, such as a poor internet connection or a conflict with other software. For this case, collect log files and submit them to the Log Analyzer to help diagnose the cause. Third, it's not uncommon for users to accidentally delete files in Drive. When this happens, they'll likely turn to you for help with recovering them. Fortunately, as an administrator, you can often recover deleted files. But it depends on a few factors. The files must have been deleted within 25 days. The file can't be a Google My Maps or a Fusion Table file. The user can't have met their Drive storage quota. And the file can't be in the user's trash. In this case, the user must recover the file themselves within 30 days of deletion. There's one important thing to keep in mind about restoring files in Google Drive. You can only have one restoration project running at of time. So you can only work on getting back files from one date range at a time. You can't restore individual files or folders. Finally, your users might have trouble accessing files in Drive when they're offline. This usually happens for one of two reasons. Either they haven't turned on the offline access feature in Drive, or they've used up all their storage space on their device.

### Link - [Shared drive errors](https://www.cloudskillsboost.google/course_templates/1280/documents/530810)

* [Shared drive errors](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67e12163fae88dcad1af7018)

### Link - [Drive for Desktop errors](https://www.cloudskillsboost.google/course_templates/1280/documents/530811)

* [Drive for Desktop errors](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67e12538fae88dcad1b00029)

### Link - [Accidentally deleted files](https://www.cloudskillsboost.google/course_templates/1280/documents/530812)

* [Accidentally deleted files](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67e12a42fae88dcad1b0cfa5)

### Link - [Drive offline access issues](https://www.cloudskillsboost.google/course_templates/1280/documents/530813)

* [Drive offline access issues](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67e12cb9fae88dcad1b18492)

### Quiz - [Quiz: Troubleshooting Google Drive issues](https://www.cloudskillsboost.google/course_templates/1280/quizzes/530814)

#### Quiz 1.

> [!important]
> **A user accidentally deleted a critical file from their Google Drive and emptied their trash. As a Google Workspace Administrator, what is the maximum number of days you have to recover the file after the user emptied their trash?**
>
> * [ ] 14 days
> * [ ] 30 days
> * [ ] 7 days
> * [ ] 25 days

#### Quiz 2.

> [!important]
> **A user reports they can't access their Google Drive files offline, despite enabling offline access. What's the first troubleshooting step you should recommend?**
>
> * [ ] Check the internet connection.
> * [ ] Temporarily disable antivirus/firewall software.
> * [ ] Try accessing Google Drive offline on another device.
> * [ ] Clear the browser cache and cookies.

#### Quiz 3.

> [!important]
> **A user reports that Drive for Desktop is not syncing a specific folder on their macOS computer. After verifying their internet connection and restarting the application, what should you advise the user to do next?**
>
> * [ ] Reset their Google Account user preferences.
> * [ ] Reinstall Drive for Desktop.
> * [ ] Update their macOS operating system.
> * [ ] Verify the folder has "Read & Write" permissions in Finder.

#### Quiz 4.

> [!important]
> **A user reports they can't move a specific folder into a shared drive. What's a possible reason for this issue?**
>
> * [ ] The user's Google Workspace license doesn't support shared drives.
> * [ ] The user is not a member of the shared drive.
> * [ ] The ability to create a shared drive has been disabled by the user's organizational unit.
> * [ ] The folder contains too many files that can't be moved or exceeds shared drive limits.

### Video - [Support resources](https://www.cloudskillsboost.google/course_templates/1280/video/530815)

* [YouTube: Support resources](https://www.youtube.com/watch?v=l9yfqiTDoQI)

SPEAKER: In addition to understanding how to monitor and troubleshoot problems that users in your organization may face, as the administrator, you should also know how to obtain support from Google. Google offers several ways to help. The first is the Google Workspace Status Dashboard, which shows the status of Google Workspace services. This dashboard displays any incidents that have occurred during the last week. You can click into any incident to find out more and track its resolution. From there, you can also view the full history of incidents for an individual service. Second, you can use the Support card in the Admin Console to connect with the Help Assistant, view important alerts, search for help, and contact Google support. The Admin Help Center includes detailed information on how to contact support and fix known problems. We encourage you to bookmark the contact support page that you'll find at support.google.com/a. For super administrators and custom administrators with the support privilege, the Customer Care Portal can be used to create and manage support cases. The portal includes a system status section, which shows a summary of recent Google Workspace issues. To learn more about filing support tickets with the customer care team, check out the Google Cloud Customer Care Fundamentals course on Google Cloud Skills Boost at cloudskillsboost.google. Now let's explore the Google Admin Toolbox, which includes several easy to use tools to help you troubleshoot problems. These tools can also be used to collect information that may be needed by Google support as they help to identify and resolve problems. The browser debugger can be used to determine if your browser has any connectivity issues. With this tool, you can collect important browser parameters, detect installed plugins, and check connectivity to Google services. Next, the Check MX tool can be used to verify your DNS settings and establish the status of your domain. Checks carried out by Check MX include general DNS sanity checks and Google Workspace-related issues. Questions related to general DNS sanity checks might include, is there more than one name server? Are the domains all reachable? Do they know about each other? And are they synchronized? And questions related to Google Workspace-related issues might include, do MX records for the domain match the recommended setup? Are there any misconfigurations? And are there servers that aren't part of a normal configuration? Finally, the HAR Analyzer can be used to analyze HTTP Archive, or HAR files. HAR files are JSON-formatted archives that record the communication between a web browser and a website, tracking all exchanged messages. The HAR analyzer uses the HAR file to play detective. It checks if any messages had errors, got lost along the way, or had weird responses. Basically, it uses the HAR file to figure out why something might have gone wrong on a website. Google support will often ask for the HAR file to help troubleshoot issues.

### Link - [Report an issue](https://www.cloudskillsboost.google/course_templates/1280/documents/530816)

* [Report an issue](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67e12f1afae88dcad1b2aaa0)

### Link - [Service down](https://www.cloudskillsboost.google/course_templates/1280/documents/530817)

* [Service down](https://storage.googleapis.com/cloud-training/S-GSAD/T-TSGW-B%20%7C%20Google%20Workspace%20Troubleshooting/index.html#/page/67e13356fae88dcad1b370f1)

### Quiz - [Quiz: Support resources](https://www.cloudskillsboost.google/course_templates/1280/quizzes/530818)

#### Quiz 1.

> [!important]
> **Where can you find information about Google Meet service disruptions from three years ago?**
>
> * [ ] The Google Workspace support ticket archive, searching for relevant incidents.
> * [ ] The extended service history section of the Google Workspace Status Dashboard.
> * [ ] The Alert center in the Security investigation tool of the Google Admin console, filtering by service.
> * [ ] The Reports section of the Google Admin console, filtering by service and date.

#### Quiz 2.

> [!important]
> **During a potential Google Workspace outage, including a possible Gmail disruption, which notification method is most reliable?**
>
> * [ ] Reviewing the Status Dashboard history for past incidents.
> * [ ] Subscribing to the Status Dashboard RSS feed.
> * [ ] Checking the Google Workspace Status Dashboard website.
> * [ ] Setting up email alerts via Google Admin console.

#### Quiz 3.

> [!important]
> **A user says they sometimes get an error in Google Sheets, but not consistently. What information should you gather from the user to start troubleshooting the issue?**
>
> * [ ] The user's username and password.
> * [ ] The user's browser version and a list of all installed extensions.
> * [ ] A detailed description of the error with relevant screenshots.
> * [ ] The user's complete browsing history and an HTTP Archive (HAR) file capturing all network traffic.

### Video - [Course recap](https://www.cloudskillsboost.google/course_templates/1280/video/530819)

* [YouTube: Course recap](https://www.youtube.com/watch?v=7J38oGPZeSQ)

SPEAKER: This brings us to the end of the Google Workspace Troubleshooting course. Thanks for following along. The goal of this course was to help you diagnose and resolve common issues your users might face in Google Workspace. First, you learned how to troubleshoot and investigate security-related issues within Google Workspace. Next, you learned about the various approaches to address issues with Calendar, Gmail, and Drive. And finally, you explored the technical support resources that are available to you as an administrator. At the beginning of the course, you might have signed up for a trial Google Workspace account. If you did, it's important to remember that the trial period lasts for 14 days. At which time, your credit card will be charged unless you've canceled your subscription. If you don't plan to take any other courses in the Google Workspace administration series or if your trial period is about to expire and you want to avoid charges, be sure to cancel your subscription now. For detailed instructions, visit support.google.com/a and search cancel a subscription. If you're looking to demonstrate your knowledge of the topics presented in the Google Workspace administration courses, you're encouraged to take the Google Workspace Associate Administrator certification exam. For more information about the exam, including additional resources to help continue your preparation, please visit cloud.google.com /certification/a ssociate-google- workspace-administrator. Thank you for completing this course. We'll see you next time.

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
