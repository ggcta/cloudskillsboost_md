---
id: 323
name: 'Analyzing and Visualizing Data in Looker'
type: Course
url: https://www.cloudskillsboost.google/course_templates/323
date_published: 2024-12-09
topics:
  - Dashboard
  - Looker
  - Data
---

# [Analyzing and Visualizing Data in Looker](https://www.cloudskillsboost.google/course_templates/323)

**Description:**

In this course, you learn how to do the kind of data exploration and analysis in Looker that would formerly be done primarily by SQL developers or analysts. Upon completion of this course, you will be able to leverage Looker's modern analytics platform to find and explore relevant content in your organization's Looker instance, ask questions of your data, create new metrics as needed, and build and share visualizations and dashboards to facilitate data-driven decision making. 

**Objectives:**

* Define Looker and the capabilities it provides for working with data
* Use dimensions, measures, and filters to analyze and visualize data
* Use dashboards for multiple visualizations and boards to curate Looker content
* Create advanced metrics by pivoting Looker data and writing table and offset calculations
* Create visualizations using Looks and dashboards
* Share Looker content with others

## The Looker platform

This module provides an overview of the Looker user interface and its key components for data explorers.

### Video - [What is Looker?](https://www.cloudskillsboost.google/course_templates/323/video/516790)

* [YouTube: What is Looker?](https://www.youtube.com/watch?v=X0FKTOhCHkY)

SPEAKER: Hello. Welcome to what is Looker, a lesson in the Looker platform module. Let us discuss what the Looker platform is and how it empowers people who collect and leverage data. Specifically, Looker is a powerful enterprise scale data platform that allows business users to see consistent data through their preferred method, enabling them to analyze the most current data to make data-based business decisions immediately. To consider how Looker can support your data workflows, let's examine the overall data analysis process and the role of Looker in this process. When working with data, it's important to have clear objectives. We suggest a data analysis process that includes the following components. First, define questions. Identify what questions need to be answered using your data. Next, identify required data. Determine the specific dimensions and measures you will need to answer those questions. Third, analyze data. Explore the dimension and/or measure relationships via tables and visualizations. This exploration of your data should empower you to take some kind of action or make some kind of decision with regard to your work. Finally, interpret the results. Glean actionable insights from your analyzed data. Looker can support you throughout this process. For example, you can explore your data in Looker to help you define questions and identify necessary data sets. Then you can use Looker to analyze and visualize data to answer your questions. Last, you can share visualizations and dashboards with your stakeholders to facilitate discussion on the results and identify next steps. Independent of the data sets used, this data analysis process is transferable and can provide a useful framework for thinking about how Looker can be integrated into your existing workflows.

### Video - [Looker user interface](https://www.cloudskillsboost.google/course_templates/323/video/516791)

* [YouTube: Looker user interface](https://www.youtube.com/watch?v=gasO5CheJms)

SPEAKER: Looker is an enterprise platform for data experiences. Let's review how to navigate the Looker platform and how you can use it to explore your organization's data. Looker is a browser-based cloud application, which means you access it by opening an internet browser, like Chrome or Firefox, going to a URL, and logging in. For example, the URL for a company's Looker instance might be companyname.looker.com. Typically, you can log in to an instance with an email and password combination, though your company might have single sign-on enabled. In that case, you would click on an authenticate button to get in without the need to remember or store separate credentials. Tip-- if you're using a trusted device, check the "Stay Logged In" box to reduce the frequency that you'll need to re-authenticate. When you first log in to the Looker platform, your homepage may vary depending on what your company's Looker administrator has configured. In this example instance, we are seeing the Shared Folders. Folders in Looker are where content lives, just as files in your computer or Google Drive are stored in folders. Folders may contain subfolders, which help to organize and secure content. Content, in Looker terminology, refers to looks and dashboards. Looks are standalone reports or visualizations, while dashboards contain more than one visualization. We'll dive deeper into all this as we explore this example Looker instance. Let's review the navigation options available to different types of users in Looker. First, the left-side panel provides the content navigation options for users that have been added to the Looker instance as data viewers, which are users who need to find existing information quickly and easily. Data viewers do not create their own reports and visualizations. Now, if you have been added as a data explorer to a Looker instance, you will also see the explorer section of the left-side navigation panel of the Looker user interface. As a data explorer, you use explorers to ask questions of your data and create visualizations and reports that can be shared with others, such as data viewers. For example, if you wanted to learn specifics about Citi Bike trips in your city, you choose the Citi Bike Trips Explorer. Explorers are curated by Looker developers in a proprietary templating language called LookML. The explorers that you have been given access to will be listed under this explore section. The Explorer section of Looker is where we'll be spending the majority of our time in this walkthrough. Next, the Develop menu is used by LookML developers to curate the explorers that are accessible to data explorers via the Explorer section. Within the develop environment, developers can specify which fields are available in each explorer, how each field appears, and the logic or behavior for each field. Developers can use the toggle button at the bottom left side of the user interface to enter development mode to make and test changes to LookML code before sending the changes to production. At your organization, you may not see a develop menu if that is not part of your role. We will not review the options in the develop environment in this walkthrough, as we will work with explorers that have already been created by LookML developers. Finally, Looker administrators use the Admin menu to configure the users, permissions, and other settings for the Looker instance, such as database connections. Again, in your organization's Looker instance, you may not see an admin menu if that is not part of your role. We will not be using the options in the Admin menu in this walkthrough either. In this walkthrough, we will focus on resources available through the Shared Folders and Explore menus, which provide the key options for data explorers to access, analyze, visualize, and share data. From the left-side navigation panel of the Looker user interface, you can access your recent Looker content, browsing history, and recently viewed. This might be useful if you need to access a report from a day or two ago but can't remember what it's called or aren't sure where to look for it. When you do find something that you want to save for future reference, you can add it as a favorite and then access your list of favorites from here. This section will contain all of your favorited dashboards and looks. A useful feature that you can toggle is the menu icon in the top-left corner of the page to collapse or expand the left-side navigation panel any time. Moving on, boards serve as a useful way of organizing and curating content, such as saving multiple looks and dashboards onto one board that you can share with others. Finally, if your Looker administrator has installed any applications or blocks, which are prebuilt data models from the Looker marketplace, they would also show up in the left-side navigation panel. Applications are not in the scope of this walkthrough. Each user has a personal folder with their name on it. In the current view, it is labeled as My Folder. For you as a Looker user, this is your own scratch space for works in progress, as well as a storage space for content that is only meaningful to you or your role. Expanding the folder's menu allows you to see additional folders beyond the Shared Folders. For example, you can go to the People folder under all folders to see other users' personal folders. If you have LookML dashboards created in your Looker instance, you will see a LookML Dashboards folder. These dashboards are defined in LookML, which is different to user-defined dashboards, which are created using the Looker web interface. Now, in the top-right corner, you'll see up to five icons. The book being read leads to specific Looker education and in-application tutorials. The magnifying glass allows you to search across the Looker instance by keyword and also links you back to Looker Connect for learning assistance. The Looker Marketplace, if enabled, is where you can find applications and tools to get more out of your data. The help icon provides links to chat support, docs, a user guide, and more. And the user icon is where you'll find access to information associated with your Looker account. Let's shift our focus to the Shared Folders page and explore folders and content. Folders contain looks and dashboards for specific groups of people. You can copy, move, or save looks and dashboards to a folder. Folders can also contain subfolders. The Dashboard section shows various pieces of data in one location, like the Business Pulse Dashboard, for example. Each section of a dashboard is referred to as a single visualization, or tile. OK, let's examine a dashboard. In our e-commerce company, we want to see how business is going at our company. So we can click on the example Business Pulse 21 Dashboard. Dashboards in business intelligence show you various pieces of information about some overall topic or domain, similar to how a dashboard on a car shows you various aspects of your car's performance, how quickly you are going, how much gas you have left in the tank, whether your headlights are on, and so on. So in dashboards like Business Pulse 21, you can see some key metrics that a typical e-commerce company would care about, the number of users, average amount they spend per order, average amount each spends in their lifetime, number of orders so far this year, and how that compares to the same point in time last year. We call these single value visualizations. Scrolling down the dashboard, you can see some other visualization types Looker supports out of the box, including area and line charts, maps, tables, donut multiples, and column charts. Now, let's say you work in marketing, and you want to see some more information about the average spender per user in 2018, maybe because you want to understand more about why they're spending as much as they are and also seek opportunities to connect them with more products they might want to purchase. In Looker, you can click on any visualization to drill down, meaning you can see a more detailed breakdown of the data. Clicking on the number for average spender per user shows you details. In this case, we're starting at a high level with just the order IDs for those purchases. But what if you want to know more about these customers, like their ages and locations? If you have permission to access the underlying data, you will usually find an option to explore or explore from here to drill down into additional information. Clicking on this option takes you out of the dashboard and into a separate interface called the Explorer. Yes, this is a different part of Looker. From this point on, you can work with the underlying data through the Explorer without affecting the Business Pulse 21 Dashboard that you were just viewing. We've mentioned explorers a few times, so you may be wondering, what exactly is an explorer? Well, an explorer is a report builder interface as well as a portal to ask questions of your data. To the left of the screen is the field picker. Fields are bundled in these expand-collapse menus called views. Each view is a related concept. Since you are in the Order Items Explorer, you have a view for order information, such as when an order was created, its ID, its status, and so on. However, orders do not exist in a vacuum. They are ordered by people or users. The goods come from inventories. The goods have product information such as brand and category. And they come from distribution centers. As you explore order data or assemble a report about orders, you may need to include fields from some or all of these other views. That is why they are all offered together in this Order Items Explorer. Let's expand the user's view. Each view has dimensions at the top, which are attributes of the data and measures at the bottom, which are aggregations of the data attributes. For now, let's continue our narrative as a marketer looking for those additional opportunities to connect customers with products they will love. Maybe you'd like to view average spend by user by product brand. You could filter on brand and make it one of your company's leading brands, brand A, after adding, removing, or modifying fields in the explorer. You always need to click the Run button in the top right corner. Just like that, you have asked a question of the data, what is the average spend by user for brand A, and received your results. But how do you share this view of your data with others? If you click on the gear menu next to the Run button in the higher right-hand corner of the application, you can save and share this new data-driven insight a few different ways. From the save expander menu, you can choose to save it to either a new or existing dashboard to which you have previous access or to a new look. You could also open this data in Looker Studio for more advanced visualization design. If you just want to share this data as is, you can choose to send it one time. However, if you wanted to send data more than once, you can create a schedule for that and define how often that occurs. Or you could even just share the URL for the explorer as you see it now for others to work with. Back on the Shared Folders page, you can also see a list of available looks. Unlike a dashboard, a look is a single report. For example, a look called Yearly Revenue is a standalone report of yearly revenue for 2018 to 2021 displayed in a single visualization. Now, after this brief overview of the Looker user interface, we hope that you are excited to explore Looker some more to analyze and visualize your data.

### Video - [Organizing content with folders](https://www.cloudskillsboost.google/course_templates/323/video/516792)

* [YouTube: Organizing content with folders](https://www.youtube.com/watch?v=OAEYLkTY0sg)

Now, a common challenge that organizations face is that people struggle to find relevant content that already exists, so they make their own, causing duplicates and confusion. To help you address this challenge, Looker provides many ways to organize content to make it more discoverable to others at your organization, including the ability to create and share folders within your Looker instance. To see the organizational structure of folders in your Looker instance, you can expand the Folders menu on the left-side navigation panel of the Looker user interface. Under Folders, you will typically see Shared folders (which contains all folders shared across an organization), My folder (which is your personal folder), and All folders (which shows all folders that you have access to in your Looker instance). Now, depending on the settings configured by your Looker administrator, it is common for the Shared folders page to be set as the home page for users (as shown in this example), but it doesn’t have to be. All shared folders that are accessible to you will appear at the top of the Shared folders page under the header called Folders. Of course, if you have been granted the permission to create new folders in your Looker instance, you can create a new shared folder by clicking on New button in the top right-hand corner next to the gear menu icon. A new window will open for you to name the new folder. The new shared folder will be visible to all users within your Looker instance that can access items within Shared folders. A best practice when creating a new shared folder is try to ensure the overall folder structure remains clear and intuitive. In this example, there is a folder for each business team or unit, so if you need to know more about Professional Services’ current projects, it is clear where you need to go. Of course, the appropriate folder names and structure will differ by organization, but the objective of promoting discoverability and ease of use is key for all organizations. Remember, the goal of the shared folder is to make the content stored there as easy to find and use as possible. Be sure to take a moment to review the existing Shared folders structure as you decide when and where to create new folders and their appropriate names. The next folder type under Folders is labeled My folder. In Looker, all users are provided with their own personal folder as a scratch location to work with content. Within your My folder, you will see items that you have created and stored in your personal folder, including Looks and dashboards, as well as subfolders that you may have created. While your personal folder is intended to be your own space for works in progress, and other items that you may not need to share, other users within a Looker instance can be granted access to your personal folder, if needed, by Looker administrators. Just like in the shared folders, you can click on New within My folder to create a new folder, if you have the permission to do so. Again, a new window will open for you to name the new folder. Last, the option for the drop-down People folder list is useful to easily and quickly see all of the folders that you have access to within your Looker instance. So, in summary, with these various folder options, Looker makes it easy for you to manage your content, so that it is readily discoverable and usable by others at your organization. Have fun exploring the folders in your Looker instance!

### Quiz - [Module 1 Quiz](https://www.cloudskillsboost.google/course_templates/323/quizzes/516793)

#### Quiz 1.

> [!important]
> **You can access all Looker content contained within the "All folders" folder.**
>
> * [ ] False
> * [ ] True

#### Quiz 2.

> [!important]
> **What folder type does NOT exist in the Looker platform end user interface? Please choose the best answer.**
>
> * [ ] The "Shared folders" folder.
> * [ ] The "People" folder.
> * [ ] The "My folder" folder.
> * [ ] The "Recently Viewed" folder.

#### Quiz 3.

> [!important]
> **Boards are the primary content type available in the Looker platform.**
>
> * [ ] True
> * [ ] False

#### Quiz 4.

> [!important]
> **The Looker platform empowers you with options to share with others your data analyses or visualizations.**
>
> * [ ] True
> * [ ] False

#### Quiz 5.

> [!important]
> **Who can create their own Looks and dashboards in Looker? Please choose the best answer.**
>
> * [ ] Data viewer end users only.
> * [ ] Both data explorer and data viewer end users.
> * [ ] Neither data explorer nor data viewer end users.
> * [ ] Data explorer end users only.

#### Quiz 6.

> [!important]
> **Which of the following services is provided by the Looker platform? Please choose the best answer.**
>
> * [ ] None of these services relate to the Looker platform.
> * [ ] Data analysis only.
> * [ ] Data analysis and data visualization.
> * [ ] Data visualization only.

## Data analysis building blocks

This module reviews three data analysis building blocks - dimensions, measures, and filters.

### Video - [Dimensions in Looker](https://www.cloudskillsboost.google/course_templates/323/video/516794)

* [YouTube: Dimensions in Looker](https://www.youtube.com/watch?v=yg_5_6iMwGU)

Dimensions are attributes or characteristics of your data. Specifically, each column in a database table is a dimension in Looker. For example, this is a basic 12-row dataset that describes the fruit basket in the image on the left. Each piece of fruit is represented as a row in the table, with each column describing a different attribute or aspect of the fruit. Each fruit has a type and a color, either is or is not round, and has a price per pound, weight, and unit price. In Looker, all of these columns are dimensions. Using this dataset, you can ask a question like, “What types of fruit are in the basket?” What is the dimension you need here? Fruit Type! When you select a dimension in Looker, only the unique possible values are displayed. As such, the Fruit Type dimension returns 5 rows for the 12 fruits: one each for oranges, apples, bananas, lemons, and limes. Even though you can see in the basket there are 3 lemons, 2 bananas, and so on, you don’t get multiple rows for them; you have only one row for each. Now, you may also want to know, “What colors of fruit are in the basket?” This would require the Color dimension in Looker. Again, only the unique possible values are returned. Instead of getting 12 rows of data, you only get 4—one for each for yellow, red, orange, and green. Okay, but what if you want to know the combinations of fruit types and colors in the fruit basket? Now this would require choosing two dimensions in Looker. Notice that you now have 6 rows. Selecting two or more dimensions returns all unique combinations of the values. For example, the “apple” type is displayed twice, once for the red apples and again for the green. Be aware that selecting multiple dimensions may result in more rows or different groupings than you may have initially expected. In analytical queries, the dimensions are grouped by the different unique ways in which they can be combined, such as both fruit type and color. A different example might be a reporting of metrics by different cities. In this case, selecting only the city dimension may not give you what you want, as all cities with the same name would group together, regardless of their state, province, or territory. To separate the cities with the same name, you would need to add the state, province, or territory, and you will then get the individual cities broken out as expected. In summary, dimensions help you to identify and select data attributes that you need to answer your questions in Looker. Each column in a database table is a dimension in Looker, and you can combine dimensions to return all of the unique combinations of the values.

### Video - [Measures in Looker](https://www.cloudskillsboost.google/course_templates/323/video/516795)

* [YouTube: Measures in Looker](https://www.youtube.com/watch?v=uV6RG4LFMdo)

So, what are measures, anyway? Measures are calculations performed across multiple rows of data. As such, measures are aggregates of data attributes, or dimensions. In summary, dimensions help you to identify and select data attributes that you need to answer your questions in Looker. Each column in a database table is a dimension in Looker, and you can combine dimensions to return all of the unique combinations of the values. Now, one question you might have is “How many pieces of fruit are in the basket?” Any time you have a question like “how many,” you probably want to look for a measure with the word Count or Number in it. In this case, you need the Count measure, which tells you that the basket has 12 pieces of fruit. Another question might be “How much does the basket of fruit weigh?” Well, in this case, you want to know the sum or total of all these fruits’ weights, without the basket. An existing measure in the dataset might be called something like Total Weight, which aggregates the weights of all of individual fruit in the dataset. In summary, as highlighted in these examples, measures are useful for aggregating dimensions (or data attributes), so that you can easily calculate values such as count, sum, or even averages across your data.

### Video - [Example: Exploring measures using customer data](https://www.cloudskillsboost.google/course_templates/323/video/516796)

* [YouTube: Example: Exploring measures using customer data](https://www.youtube.com/watch?v=CFRmgoq6OW4)

In this example, we’ll explore how to start using measures to analyze and visualize data. Specifically, we’ll use the Users data within the Explore called Order Items to determine the number of total users, and then display that number as a single value visualization. To begin, to access the Users data, we will click on the Explore section in the left-side navigation panel, and locate Order Items under the E-Commerce heading. The goal is to determine how many users there are in total, and show that number as a single-value visualization. Any time you have a question with the words “how many,” you probably want a count measure. Within the Users view of the Order Items Explore, there is a measure called Count. Click the Count measure, and then the Run button. Expand the Visualization bar to see and adjust the visualization. Looker tries to guess the right type of visualization based on the data in your results set, and in this case it’s right—you do want a single-value visualization, since your results set only contains a single value. You can click on these other icons to change the visualization, including the three-dot menu that will highlight many other visualization types. Looker will tell you if something isn’t appropriate for your data. So the column chart is technically valid, even if it would look pretty silly. A pie chart, on the other hand, “requires one dimension and one numerical measure,” so you can’t make one with this results set. The single-value visualization is what you want, so click on the 6 icon to display the single-value visualization. You can also change the text to your favorite color. In the visualization gear menu, navigate to Style > Value Color and choose a color from either a style palette or a custom color. You can also set the title of the visualization to a more descriptive title such as “Total Number of Users”. In the visualization gear menu, type “Total Number of Users” into Title Override box in the Style tab. And with that, the single value visualization for Total Number of Users is now complete!

### Video - [Using dimensions and measures](https://www.cloudskillsboost.google/course_templates/323/video/516797)

* [YouTube: Using dimensions and measures](https://www.youtube.com/watch?v=JiXYfXaoUT0)

In real-life analytics, you often need to combine dimensions and measures, in order to answer your data questions. For example, in this basic 12-row dataset, each piece of fruit is represented as a row in the table, with each column describing a different attribute or aspect of the fruit, such as type and color. You can also think about which measures might be useful to aggregate the dimensions, such as a total weight or total price. Now, by combining dimensions and measures, you can ask, “How many pieces of each fruit type are in the basket?” Let’s break down this question. “How many pieces” suggests that you need the Count measure, while “of each fruit type” means you need the Fruit Type dimension. Putting these two together, you get the five rows because Looker grabs only the unique possible values of the dimension. You also see the overall count of 12, split out across those five rows: 3 apples, 3 lemons, and so on. As another example, you may want to know “What is the total cost of each type of fruit?” Again, let’s think about what this means in terms of dimensions and measures. In this case, you need the Fruit Type dimension and the Total Price measure. This results in these five rows because Looker grabs only the unique possible values of the dimension, and the total price is being calculated for each value. In summary, by combining the necessary dimensions and measures, you can answer more complex questions by fully leveraging datasets that have many available attributes and aggregations.

### Video - [Example: Combining dimensions and measures](https://www.cloudskillsboost.google/course_templates/323/video/516798)

* [YouTube: Example: Combining dimensions and measures](https://www.youtube.com/watch?v=iuFgMraaJwA)

In this example, we combine dimensions and measures to start answering more complex questions. Specifically, we’ll work with the Users data in the Order Items Explore to identify the top 10 cities that have the most users. Then, we’ll display the results as a column chart. To begin, to access the Users data, we will click on the Explore section in the left-side navigation panel, and locate Order Items under the E-Commerce heading. In the Users data, notice that the dimensions on the left-side panel are listed alphabetically, and some dimensions are grouped like Created Date. If you can’t find the dimension you’re looking for at a glance, you can use the search function to quickly find what you’re looking for. The goal is to identify which cities have the most users, so start by selecting the City dimension and then scroll down and select the Count measure to see how many users are in each city. Since you only want the top 10 cities, set the row limit to 10. Once that’s all set, click Run to display the top 10 cities based on the number of users. Next, click on a column header to sort the results. A single click sorts the data from the largest value to the smallest. A second click will sort the data value from smallest to largest. You can display the results as a column chart by selecting Visualization, then the option for the column chart. You can also add labels to the side of each bar, showing the total bar value. Click on the visualization gear menu, and turn on Value Labels under the Values tab. Each column in the chart will now have its value displayed above the bar. Now, the column chart showing the top 10 cities with the most users is complete.

### Video - [Filtering dimensions](https://www.cloudskillsboost.google/course_templates/323/video/516799)

* [YouTube: Filtering dimensions](https://www.youtube.com/watch?v=JWWqyJ265ME)

In Looker, filters are ways to reduce or narrow down the results returned based on specific criteria. In this way, filters allow you to hone in on a subset of your data based on desired characteristics. A key feature of filters is that they don’t delete anything from the database; they’re only applied to the data that Looker displays on your screen. For example, in this basic 12-row dataset, each piece of fruit is represented as a row in the table, with each column describing a different attribute of the fruit, such as type and color. How might you want to filter this fruit basket? Well, maybe you want to see only fruits that are round. You can apply a filter on the Is Round dimension, and set it equal to “yes”. This is called applying a dimension filter, and what Looker does behind the scenes is to figure out which rows of data need to be included or excluded right from the start. Now, using this filter, you can ask a question such as, “How many pieces of each fruit type are there if only round fruits are included?” Behind the scenes, your database first skips over or ignores the fruits that aren’t round, since they don’t meet the criterion of our dimension filter. Then, Looker takes what’s left—apples and oranges—and performs the aggregation, so we get 3 apples and 2 oranges. Of course, you may also want to know, “How many pieces of each fruit type are in the basket if I only include red and orange fruits?” To answer this question, you can apply a filter on the Color dimension and set it equal to “orange” or “red”. So you get 2 oranges and 2 red apples. This demonstrates that you can make a filter equal to more than one value. In summary, you can use dimension filters to select only the data you want to see in your results, such as round fruit only, without affecting the underlying data tables. You can also select more than value for a particular dimension filter, such as fruit that are either orange or red. Based on the values you provide in the dimension filter, Looker knows which data rows to include or exclude in the results, making it easy to get the results you want.

### Video - [Filtering measures](https://www.cloudskillsboost.google/course_templates/323/video/516800)

* [YouTube: Filtering measures](https://www.youtube.com/watch?v=xcpzs_I83f8)

In Looker, you can filter on both dimensions and measures to select only the data you want to see or include in your results. In either case, the underlying data is not affected, and Looker knows which data to include or exclude based on the filter. Specifically, Looker will ignore any rows that do not meet the filters provided before returning the results. For example, in this basic 12-row dataset, each piece of fruit is represented as a row in the table, with each column describing a different attribute of the fruit, such as type and color. Notice that there are three apples in this dataset: 2 red and 1 green. If a dimension such as color is used a filter, then Looker will apply that filter first and then aggregate data based on the measure that has been selected. In this example filter, only fruit that are orange or red are selected, which means that the green apple in the dataset is not returned in the results. For this reason, the number of apples has decreased from 3 to 2. Again, this is because the dimension filter removed one apple that was green. But, what if you want to know, “Which types of fruit have exactly two pieces in the basket?” In this case, you would need to apply a filter on the Count measure, setting it to equal 2. Notice that in this dataset, only the banana, lime, and orange fruit types have a count of two. Both apple and lemon have a count of three, so they should not be returned as part of the results. With this example, you can see that the key difference between filtering dimensions versus measures lies in when Looker decides to exclude data. With dimension filters, Looker excludes the rows that do not meet the filter at the very beginning, such as excluding fruit that are not red or orange. With measure filters, Looker first gets all the possible rows and calculates all of the potential aggregations. Then, Looker discards the undesired results at the end, before returning the results. In this specific example, Looker did not return the fruit types that are apple or lemon because they both have a count of three, not two as specified in the measure filter. Let’s consider another example. Maybe you want to know “Which types of fruit have an average price that is less than $0.50?” First, you need to set a filter on Average Price being less than 0.5. Looker gets all the unique possible fruit types and calculates the average price for each. Then, it removes the results with an average price of fifty cents or more as the last step, so you are left with only the results that meet the filter logic. In summary, you can filter on either dimensions or measures in Looker to select only the data that you want to see or include in the results. When you use a dimension filter, Looker will exclude the rows that do not meet the criteria at the very beginning of the analysis. When you use a measure filter, Looker first calculates all of the potential aggregations and then excludes the results that do not meet the desired criteria at the end of the analysis, before returning the results. In either case, Looker handles the inclusion and exclusion of data for you and returns only the data results that you want.

### Video - [Example: Filtering with measures](https://www.cloudskillsboost.google/course_templates/323/video/516801)

* [YouTube: Example: Filtering with measures](https://www.youtube.com/watch?v=G_D2rzJ9Xt0)

In this example, we’ll work with the Created Date data in the Order Items Explore to identify the total number of items sold each month in 2019. Then, we’ll display the results as a line chart. To begin, to access the Created Date data, we will click on the Explore section in the left-side navigation panel, and locate Order Items under the E-Commerce heading. “Total number” suggests that you probably want a count, so first expand the Order Items view to look for a count measure of ordered items. Click on the Order Item Count measure. “Each month” means you want a monthly report, so you need to choose one of the date dimension groups. Since you’re looking for items “sold,” Created Date would be best, as an order is “created” in the system when the transaction is made—in other words, when the items are sold to a customer. Now, expand Created Date and click on the Month dimension in the Created Date group to get your monthly report. Recall that you only want to look at the year 2019, so you can click on the Filter button next to Year to specify this. Set the operator to “is in the year”, and type 2019 in the text box. Then, click Run. Now, open the visualization pane, and make sure the type is set to line chart. Next, change the style of the data points within the line chart. In the Series tab of the visualization settings, you can choose a Point Style of “None”, “Filled”, or “Outline”. This examples uses Filled. Finally, you can add in a reference line that shows the average profit across the year. In the “Y” tab of the visualization settings, scroll down to the bottom, and click on the Add Reference Line button. Then, set the type to Line and the value to Average (Mean). The final line chart is now ready and displays the total number of items sold each month in 2019 with the yearly average as a reference line.

### Lab - [Analyzing and Visualizing Data in Looker](https://www.cloudskillsboost.google/course_templates/323/labs/516802)

In this lab, you will use dimensions, measures, filters, and pivots to create a series of visualizations from the Federal Aviation Administration (FAA) airports and flights datasets and save them to dashboards in Looker.

* [ ] [Analyzing and Visualizing Data in Looker](../labs/Analyzing-and-Visualizing-Data-in-Looker.md)

### Quiz - [Module 2 Quiz](https://www.cloudskillsboost.google/course_templates/323/quizzes/516803)

#### Quiz 1.

> [!important]
> **In what order are filters applied to your data in Looker during data analysis? Please choose the best answer.**
>
> * [ ] Dimensions and measures filters at the same time.
> * [ ] Dimensions filter first, then measures filter.
> * [ ] None of the order options suggested apply to filtering.
> * [ ] Measures filter first, then dimensions filter.

#### Quiz 2.

> [!important]
> **A dimension corresponds to what part of a data source? Please choose the best answer.**
>
> * [ ] None of these data sources relate to dimensions.
> * [ ] A data table.
> * [ ] A data row.
> * [ ] A data column.

#### Quiz 3.

> [!important]
> **From our previous fruit basket example, the component "Is Round?" is classified as a measure, not a dimension.**
>
> * [ ] True
> * [ ] False

#### Quiz 4.

> [!important]
> **A measure corresponds to what part of a data source? Please choose the best answer.**
>
> * [ ] Data rows.
> * [ ] SQL aggregation functions.
> * [ ] Data columns.
> * [ ] Data tables.

#### Quiz 5.

> [!important]
> **When using Looker for data analysis, only one dimension and measure combination can be selected at a time.**
>
> * [ ] False
> * [ ] True

#### Quiz 6.

> [!important]
> **End users can only apply one dimension filter at a time during data analysis.**
>
> * [ ] False
> * [ ] True

#### Quiz 7.

> [!important]
> **After the measure filter is applied, Looker discards all of the irrelevant data and only presents data that meets all current filter criteria.**
>
> * [ ] True
> * [ ] False

## Working with Looker content

This module explores the use of dashboards for multiple visualizations and boards to curate Looker content.  

### Video - [Filtering Looks](https://www.cloudskillsboost.google/course_templates/323/video/516804)

* [YouTube: Filtering Looks](https://www.youtube.com/watch?v=repFSSMM6NU)

Throughout your data analysis and visualization workflows in Looker, you will likely work with Looks that you have already made or that were made by others. One of the most common and powerful ways to modify an existing Look is to apply filters to it, so that users can limit the results returned based on specified criteria. To apply filters to a Look, you need to first enter Edit mode in the Look by clicking on the Edit button in the top right of the screen. Now that you are in edit mode, you can add filters in the same way that you apply filters in an Explore, by using the field picker in the left-side panel to choose filters from dimensions and measures. To apply a filter, click the inverted pyramid icon for the desired dimension or measure to activate the filter. This example adds a filter to the total revenue data using the Brand dimension from the Products view. This filter will allow users to see only the revenue by month for this one specific brand. Next, you must decide whether to pre-populate the filter field. Keeping it empty is a perfectly valid choice, as it allows users of the Look to choose if and how to apply the filter. This example pre-populates the filter with one filter variable based on a single brand called Example Brand 1. After you have chosen the filter logic and variables, click on the Run button next to the gear menu icon in the top right corner of the screen to refresh the data. By refreshing the data presented in the Look, you can ensure the filter worked as you intended, or modify the filter as needed. At this point, you can add additional filters or adjust any other component of the Look. We recommend that you make one change at a time and then refresh the Look to validate your results before making your next change. This way, you can check that the Look reflects your desired outcomes each time before applying more changes. Last, all that is left to do is to save the changes to your Look by clicking the Save button in the top right corner of the screen, in the blue bar. And here is the new filter saved and integrated thoughtfully into your Look.

### Video - [Introducing dashboards](https://www.cloudskillsboost.google/course_templates/323/video/516805)

* [YouTube: Introducing dashboards](https://www.youtube.com/watch?v=w-EgoTllEZ0)

Working with dashboards to look for insights, trends and to answer data-related questions is very powerful, and Looker makes it easy. Unlike a Look, which focuses on a single visualization to answer a single data-related question, dashboards in Looker are designed to contain multiple visualizations, to answer multiple questions. It can provide both deep and broad visibility into your data, empowering you to very easily surface problems, insights and opportunities in your business. Any end user, including data viewers, can work with existing dashboards to which they’ve been granted access for data analysis, but only data explorers can use Explores to create their own dashboards, or dashboards for others. But what about working with an already-created dashboard? Editing dashboards to add new content or revise the existing layout is also very easy. Start by clicking on the three vertical dots icon for Dashboard Actions at the top right of the page, and select Edit Dashboard. In edit mode, you’ll see options to add tiles and filters to the dashboard, as well as modify its settings to configure how the dashboard runs and refreshes. To add new content to a dashboard, you can click on Add Tile to add a new visualization (of which there are many types), a text tile for instructions or additional context, or even a button. Selecting a new visualization tile will display the Choose an Explore window for you to build the visualization, which you can then save to the dashboard. Selecting a new text tile will open a popup for you to write your desired text. Text tiles can be useful as section dividers or commentary for your dashboard viewers. You can also choose to write in plain text or in the Markdown language to use more advanced formatting features. You can even include a button in your dashboards, allowing you to provide hyperlinks to related internal project content, or external resources. Options for styling your new button exist as well! Once in edit mode, you can also rearrange the tiles by clicking on the top left corner of a tile and dragging it around to the desired location. You can also resize a tile by clicking on the bottom right corner and dragging to the desired size. Last, when you are done editing your dashboard, don’t forget to click Save to save your changes!

### Video - [Filtering dashboards](https://www.cloudskillsboost.google/course_templates/323/video/516806)

* [YouTube: Filtering dashboards](https://www.youtube.com/watch?v=ZNN4_rIYZY4)

In Looker, dashboard filters, sometimes called global dashboard filters, behave similarly to dimension and measure filters in that they allow users to limit the results based on a specified criteria. Let us begin with this dashboard, New York Taxi. It’s a dashboard containing no filters. So, how can we add them? Let us start by clicking on the three vertical dots icon for Dashboard Actions at the top right of the page, and select Edit Dashboard. Then, click on Filters in the top menu bar, followed by Add Filter. Next, you need to select the dimension and/or measure that you want to use as the filter, such as Passenger Count from the Nyc Taxi Explore. You can also use the search bar to find the field name you’d like to filter on, such as searching for other filter options. After you have chosen a dimension or measure, you will be redirected to the Settings tab of the filter, where you need to provide a few more details for the filter. Specifically, you need to give your filter a name or title, choose how the user interacts with the filter, determine the layout and whether they can select single or multiple values, and if desired, configure a default value for the filter. You can also expand the Additional options to require a filter value or select other filters to be updated when this filter changes. This last option is useful if you want what we call a “faceted filter.” A common example would be if you have one filter for State and one for City, and you want to make sure that when someone selects a state the list of available cities updates to offer only the cities in the selected state. On the Tiles To Update tab, you can identify the tiles that you want to update with the new filter. Looker even starts you off with some suggested tiles. In this example, Looker identifies any tiles that use data from the Nyc Taxi view in the Nyc Taxi Explore, so the new filter can automatically be applied to those tiles. An important thing to keep in mind about dashboards is that you can add tiles from different Explores—in fact, that flexibility is what makes them so powerful and valuable. So sometimes, you may find that only some, but not all, of the tiles get automatically identified to be populated with your new filter because the other tiles aren’t based on the same Explore. Sometimes you might not want filters to apply to all tiles. Again, it’s a question of what you’re trying to achieve with the filter; it’s more about design than any scientific rule. For example, imagine that you have a tile that shows passengers per ride for the current year. If someone else were to change the Passenger Count filter value to greater than 20, then the tile would only display 0 results for the entire year, since taxis do not carry that many people at one time. Any time you have a tile like this that is supposed to show data for all time, all regions, all something—you might want to head back to the Tiles To Update tab and select the Field to Filter option to “Do not filter”. Finally, when you are adding filters to your dashboard, be sure to click Save to save your changes!

### Video - [Curating Looker content in boards](https://www.cloudskillsboost.google/course_templates/323/video/516807)

* [YouTube: Curating Looker content in boards](https://www.youtube.com/watch?v=eNKlZaAr1lI)

Boards are a great way to centralize relevant content that lives in different folders within your organization’s Looker instance. The great thing about boards is that they simply link to a content item such as a Look or dashboard, which remains in its original location. So boards do not store the actual content, and the original content remains unaffected. With boards, you also don’t have to worry about permissions or data privacy because users still need access to the folder containing the item, in order to access that content from a board. For example, the Favorites menu shows all your own bookmarks, but creating a board allows you to share those bookmarks with other users and teams. Any Looks and dashboards added to the board will still live in their original folders; the board merely links to them and serves as a centralized page to easily find the content. In Looker, creating your own boards is very easy. First, on the Looker home page, click on the plus sign (+) icon next to Boards in the left-side navigation panel, and select Create a new board. Notice that you also see an option to browse all boards, which we will discuss later in this section. Next, give your new board a clear, descriptive name. For example, if you are creating a board to contain several business analysis related items, then an appropriate name could be Business Analysis. Now, once you have created your new board, you can configure it as little or as much as you like. You can add Looks and dashboards by clicking on the “Add content (+) . A drop down menu will appear giving you the choice of adding Saved content (in the form of Looks and dashboards), or a URL link for other content, including pre-configured Explores. Looker also provides the ability to group content by adding new sections, and you can write a description for the entire board itself, as well as for each individual section, to aid others in using the board efficiently. If you choose the Saved content menu option, a new window will appear where you can choose the Looks and dashboards you want to add to your new board. How you choose to group your content is entirely up to you: by team, by customer, by project, by product, by data question, and more. Once you have created new sections, you can continue adding content to a section by hovering over the section and clicking on the blue plus sign (+) for Add Content. Looker also makes it easy to pin a Look or dashboard to a board when you are viewing the content in its original location. For example, from a Look, click on the gear menu at the top right of the screen, and choose Add to a board. A window will open for you to choose on which board (and section) this new Look should be pinned for easier discovery and sharing. You can follow a similar process to pin a dashboard when viewing it in its original location. From a dashboard, click on the three vertical dots icon for Dashboard Actions at the top right of the page, and select Add to a board. You can select both the board and optionally, the section of a board for a dashboard. When you are happy with your choices, select Add. Looker also makes it easy to explicitly share access to your board with others. Simply click on the share icon at the top right of the page, and select the users that you want to access the board as well as their level of access such as view or edit. Remember, boards can be for your own benefit, for people you invite, or even for your entire team or organization. Don’t worry, though. Even if a user is given access to the board, they cannot view a particular content item on a board if they don’t already have access to see it. In addition to creating your own boards, you can also browse all boards that you have access to within your organization. On the Looker home page, click on the plus sign (+) icon next to Boards in the left-side navigation panel, and select Browse all boards. In the browse window, you will be shown every board to which you have access within your organization’s Looker instance. Remember, though, while you may have access to a board, you may not have access to all or any of the content curated on that board. To get access to the underlying content, you can reach out to your Looker administrator. In summary, boards are a great way to centralize and share content that lives in different folders within your organization’s Looker instance. Boards link to content such as Looks and dashboards in their original location, so the pinned content is not affected by being added to a board or by user actions on a board. Any previously assigned access to a content item is also maintained, so you never have to worry about users accessing content that they have not been previously given access to. Given these great benefits, we hope that you take full advantage of boards in your organization’s Looker instance!

### Video - [Example: Board creation](https://www.cloudskillsboost.google/course_templates/323/video/516808)

* [YouTube: Example: Board creation](https://www.youtube.com/watch?v=kol2ayq_EWA)

In this example, we’ll make our own board and then we’ll see how to share it with other users. In the Browse menu, click on the plus (+) icon next to Boards. Give it a name like Ecommerce Marketing. Next, create a section called Overall business by clicking on the pencil icon next to the first New section. Now we’re going to add a dashboard to this board section: the Business Pulse dashboard, by clicking on the Add content area, selecting Saved content and browsing to the Business Pulse dashboard. Let’s explore how you can share the board and manage other people’s access to it. You can share the board with specific individuals or groups managed by your organization. You can also specify the type of access that you want to provide such as view and edit access. Do you think boards would be useful for your role, team, or organization?

### Quiz - [Module 3 Quiz](https://www.cloudskillsboost.google/course_templates/323/quizzes/516809)

#### Quiz 1.

> [!important]
> **A data explorer end user must enter a dashboard-specific edit mode to add, remove or modify filters for a dashboard.**
>
> * [ ] True
> * [ ] False

#### Quiz 2.

> [!important]
> **A data explorer end user must enter a Look-specific edit mode to add or edit a filter in a Look.**
>
> * [ ] False
> * [ ] True

#### Quiz 3.

> [!important]
> **Any content added to a board moves to the location of that content in the board directory structure.**
>
> * [ ] True
> * [ ] False

#### Quiz 4.

> [!important]
> **What field types can data explorer end users select as filter criteria in a Looker dashboard? Please choose the best answer.**
>
> * [ ] Neither dimensions nor measures.
> * [ ] Both dimensions and measures.
> * [ ] Dimensions only.
> * [ ] Measures only.

#### Quiz 5.

> [!important]
> **What is one change a data explorer end user CANNOT make to a dashboard? Please choose the best answer.**
>
> * [ ] Resize tiles.
> * [ ] Export individual tiles.
> * [ ] Rename tiles.
> * [ ] Add / remove tiles.

#### Quiz 6.

> [!important]
> **What field types can data explorer end users select as filter criteria in a Look? Please choose the best answer.**
>
> * [ ] Both dimensions and measures.
> * [ ] Dimensions only.
> * [ ] Neither dimensions nor measures.
> * [ ] Measures only.

#### Quiz 7.

> [!important]
> **What content CANNOT be added to a board? Please choose the best answer.**
>
> * [ ] Dashboards.
> * [ ] Explores.
> * [ ] URLs.
> * [ ] Looks.

## Customizing Explores

This module explores pivoting data in Looker to turn a selected dimension into several columns. The module also covers the writing of table calculations to instantaneously create new metrics and offset calculations to programmatically reference values from other rows or columns in your query results to calculate new values.

### Video - [Pivoting data in Looker](https://www.cloudskillsboost.google/course_templates/323/video/516810)

* [YouTube: Pivoting data in Looker](https://www.youtube.com/watch?v=f7rbD39tGqM)

In Looker, pivots allow you to turn a selected dimension into several columns, which creates a matrix of your data similar to a pivot table in spreadsheet software. This is very useful for analyzing metrics by different groupings of your data, such as getting counts for category or label in your dataset. For example, from this basic 5-row dataset, you can ask something like, How many pieces of fruit do I have for each color, and is the fruit round or not? While this display is adequate to see that you have 5 fruits that are yellow and not round, 2 that are orange and round, etc, it’s not easy to compare all the colors against each other, or just the ones that are round against each other. Applying a pivot to the Is Round dimension transforms the display of the data into a format that is more meaningful and easy to interpret. When you pivot on a dimension, each unique possible value of that dimension becomes its own column header. Any measures are then repeated under each column header. In this case, you have one column for Is Round being “yes” and another for “no”. It becomes much easier to compare just the counts of round fruit across colors, and the counts of not-round fruit. It also shows you gaps in your data, where you don’t have any round or not-round fruit for a particular color. In summary, pivots allow you to create and display a matrix of your data, similar to a pivot table in spreadsheet software. Specifically, pivots turn a selected dimension into several columns and are applied only to the visual display of your results. With pivots, Looker allows you to regroup your data, so that you can easily compare results by different groupings and identify potential gaps, all while leaving your underlying data unaffected.

### Video - [Example: Working with pivots](https://www.cloudskillsboost.google/course_templates/323/video/516811)

* [YouTube: Example: Working with pivots](https://www.youtube.com/watch?v=8bvQ4Bi8sBk)

Whenever you have a question involving one dimension “by” another dimension, that’s a clue that a pivot might come in handy. Let’s run through a pivot example to find the total revenue from each product category by product department, and then display the results as a stacked bar chart. First, from the Explore section, locate Order Items under the E-Commerce heading. Next, select the Total Revenue measure from the Order Items view. Next, you need the product category. Where is that again? Don’t forget, any time you feel overwhelmed by all the views and fields, you can use the field picker’s search bar to surface keywords: there’s Product Category in the Inventory Items view and Category in the Products view. Go with Product Category in the Inventory Items view. You may see multiple options while searching in real Explores in your company’s Looker instance as well. Depending on how your data is structured, the same field may appear under multiple views. We recommend trying both if you’re worried about the accuracy of the results—and, when in doubt, seek help from your company’s LookML developer team. A search for “department” also yields fields under both the Inventory Items and Products views, so again, go with the one in the Inventory Items view. However, you’ll want to pivot on this item, so you need to click on the Pivot button. Click Run to see the results. Note that if you simply clicked on the field name to add it to your result set without pivoting first, you can still pivot later by clicking on the gear icon for the column header and then clicking Pivot. In the the visualization pane, you can click on the bar icon to make it a column chart. Overall, this visualization is a good start, but it doesn’t give a clear idea of how the various categories compare for overall revenue across both men’s and women’s departments. For example, which category made more revenue from men’s and women’s products combined? Thanks to the pivot, you can edit this to be a stacked bar chart by selecting Stacked under the Plot tab of the visualization settings. The stacked bar chart allows you to see that there is more overall combined revenue from Jeans than for any other category. And with that, the visualization of total revenue from each product category by department is now complete!

### Video - [Introduction to table calculations](https://www.cloudskillsboost.google/course_templates/323/video/516812)

* [YouTube: Introduction to table calculations](https://www.youtube.com/watch?v=k1A1CEcjgJA)

SPEAKER: Typically, in Looker, data explorers are given access to one or more explorers predefined by LookML developers. At your own company, that would likely mean your data and analytics team, data engineers, or data analysts. But sometimes, you'll find you need particular logic for which they haven't provided a dimension or measure, maybe because you have a new kind of question or use case. This is when you might need a table calculation. Table calculations are used to define what we call on-the-fly metrics, because they run on your query results instead of your whole database. You'll need to start by generating results with at least one dimension or measure, and then you can incorporate these fields into spreadsheet software like formulas to calculate a new metric. With table calculations, you can also set up a custom field that isn't included in the set of dimensions and measures provided by your LookML developers. For example, you can use a table calculation to create a new measure for percent of flights canceled from existing measures, on number of flights completed, and number of flights canceled. Table calculations are really cool and convenient. However, because they run after the query has been set up and are written on the fly, they can introduce differences across an organization. And they need to be recreated manually if they are not saved to a Look or dashboard. There are a few use cases where you should consider developing a table calculation. The first is to prototype a field or query, like if you want to validate whether it's useful enough to reuse. Similarly, if you need to answer a one-off question, then a table calculation is useful. If you find yourself needing the same logic repeatedly, you should work with your LookML developer team to have that logic added to the data model as dimensions or measures that everybody can use. Another scenario that might call for a table calculation is if you need to create something based purely on the results set and not on the overall data. A specific example would be if you want to create a specific kind of visualization, like one not available in your current Looker version, or for which you don't have the right types of fields in your data model. In this case, you can use a table calculation to translate your data or visualization into the form you want.

### Video - [Types of table calculations](https://www.cloudskillsboost.google/course_templates/323/video/516813)

* [YouTube: Types of table calculations](https://www.youtube.com/watch?v=NetoqSk4BXo)

In Looker, table calculations provide you with the ability to define new metrics instantaneously using custom formulas. With table calculations, you can prototype new metrics or create one-off visualizations from your query results, without having to wait for a LookML developer to modify the options available in a particular Explore. There are four basic types of table calculations in Looker: string, mathematical, logical, and date & time. String functions operate on query results that are text. For example, they can be used to capitalize letters and words, extract parts of a phrase, check to see if a word or letter is in a phrase, or replace elements of a word or phrase. In this example table, there are dimensions for Aircraft Category and Country, and a Count measure. For some people, this table may not be very easy to read or understand. To make the table easier to interpret, you can concatenate the values from these three fields with some additional text, and create a nice, user-friendly sentence in a new field called Accident report. In your final visualization, you could then hide Aircraft Category, Country, and Count, and simply display the user-friendly sentence in the Accident report field that you created with a table calculation. With mathematical functions in Looker, you can apply any kind of math on numeric values, such as arithmetic, averages, sums—even running totals and standard deviations. In this example, the Order Amount Rounded table calculation is rounding the Amount measure to the nearest decimal with 0 places (in other words, the nearest integer), while the Average Order Amount table calculation is calculating the mean of all the Amount values. With logical functions, you can check one or more conditions and execute different paths of logic, depending on the value. For example, if-conditions are very popular for displaying different results depending on whether our particular condition is met. In this example, there is a Title dimension referring to box-office films and measures for Total Revenue and Total Budget. The Profit Outcome table calculation evaluates whether the Total Revenue amount for each Title is greater than the Total Budget. If it is, the displayed value is the word “Profitable”. However, if Total Revenue is less than or equal to Total Budget, the displayed value is “Lost Money”. Finally, date and time functions operate on datetime results and allow you to extract time periods and calculate date differences and additions. You can also get the current date, time, or date and time, and create arbitrary date fields as needed. In this example, there is a Created Date dimension showing when each user registered on our site. The Months a Customer table calculation calculates the difference in months between a user’s Created Date and today’s date using the diff_months and now functions. The Join Month table calculation extracts the month from the Created Date using extract_months and then applies logic to label the month name using an if-condition. For example, if the number extracted for month is 8, then the output is “August”; if it is 9, then the output is “September”; and so on. These examples demonstrate how easy it is to combine different types of functions in one table calculation. In summary, table calculations allow you to create new metrics instantaneously and are incredibly useful for prototyping new metrics or creating one-off visualizations. There are four main types of table calculations in Looker: string, mathematical, logical, and date & time. String functions operate on text results, while mathematical functions operate on numeric results. Data & time functions operate on datetime results, and logical functions can be used to check one or more conditions and execute different paths of logic, depending on the value. Last, you can combine different types of functions in one table calculation to customize your results even further and achieve your desired outcomes.

### Video - [Writing table calculations](https://www.cloudskillsboost.google/course_templates/323/video/516814)

* [YouTube: Writing table calculations](https://www.youtube.com/watch?v=DyEqTVdUo4w)

SPEAKER: Writing and visualizing table calculations to instantaneously create new metrics should follow very familiar logical guidelines and therefore offer only a reasonable challenge to learn. In this lesson, we will work in the Order Items Explorer to determine what percentage of revenue per US state is from completed orders out of revenue from all orders for that state in the past one year. Then we'll create a map of the results. Since table calculations only operate on the results of your explore query, you first need to bring in one or more dimensions or measures by selecting the fields you need to calculate the desired metric. For example, imagine that you want to calculate the percent of flights canceled over a period of time. To begin, we have selected the dimension for depart date and the measures for flight count and canceled count and clicking Run. After you select the dimensions and measures and run the initial results, you can now create a new table calculation from the results. Next to Custom Fields, click the Add button, and select Table Calculation. A new popup window will appear in which to enter your formula. Now, one thing to be aware of here is that because administrators must enable this feature for end users, you might not have the Custom Fields view in the explorer of your organization's Looker instance, even if you do have permission to use table calculations. In that case, you would see a Calculations button at the top of the data table. Assuming custom fields are available to you, in the table calculation popover, you will need to select a calculation type or leave the selected option for Custom expression to write ad hoc expressions. Next, give your new table calculation a name, such as Percent of Flights Canceled. This name will show up as the column header and in the legend of the visualization. If using a custom expression for the table calculation, enter the formula you'd like to apply. For example, you can calculate the percentage of canceled flights by dividing the canceled flight count by the overall count of flights. Note that Looker strives for parity with commonly used spreadsheet software. So if you simply type the letter A, you can see all the various functions that Looker supports. You can get the absolute value of a number, add time intervals to a date, concatenate multiple values, right of conditions, and so on. If you want to see the full list of supported functions and some more information about them, you can click on the Help Plus Syntax Reference icon above the top right of the window, which takes you to our documentation. An important thing for people very familiar with spreadsheet software to know is that with Looker table calculations, you do not start the formula with an equals sign. That might feel a bit weird. But you'll get used to it. Next, specify the format of the results if you'd like decimals, percent, and so on. Finally, click Save to save your table calculation. You will now see table calculations appear in your data table in green. The values will show up right away, since you have already run your query with the dimensions and measures. Table calculations also get displayed in the visualization. If you don't want a specific field or table calculation in your visualization, you can click on the gear icon in the column header and select Hide from Visualization. More often than not, the table calculation is the thing you actually want to visualize. It might be the foundational dimensions or measures that you don't want, such as the flight count, because you want the visualization to show only the percent of canceled flights. An icon of an eye with a line crossing over it will appear to indicate that the column is hidden. So here's how the final line chart would look if you keep the dimension and table calculation but hide the two measures used in the table calculation formula. In addition to writing custom expressions for table calculations, you can choose from some predefined options, such as calculating the percent of column total, percent change from a previous row, running totals, and more. With options for both predefined and custom expressions, Looker gives you the power to customize your visualizations and reports as needed. In summary, table calculations allow you to instantaneously create new metrics and fields without needing to wait for a LookML developer to create them for you. Enjoy using table calculations. Just remember that since they run after the query has been set up and are written on the fly, they can introduce differences across an organization. And they need to be re-created manually if they are not saved to a Looker dashboard. For these reasons, table calculations are most useful for prototyping new metrics, answering one-off questions, or creating visualizations based purely on query results. And with this knowledge, we hope you now look forward to playing around with table calculations in Looker.

### Video - [Example: Writing and visualizing table calculations](https://www.cloudskillsboost.google/course_templates/323/video/516815)

* [YouTube: Example: Writing and visualizing table calculations](https://www.youtube.com/watch?v=G5khqyH3RhU)

SPEAKER: In this example, we will review how to write and visualize table calculations to instantaneously create new metrics. We'll work in the order items explorer to determine what percentage of revenue per US state is from completed orders out of revenue from all orders for that state in the past one year. Then we'll create a map of the results. Begin by opening the order items explorer under the e-commerce heading. From the order items view, select the total revenue and total revenue from completed orders measures. Click on the filter button next to the date dimension in the created date group. Then set the created date filter to is in the past one complete years. Next, in the users view, select the state dimension. Then click on the filter button next to the country dimension and set the filter to is equal to USA. Click Run. Now that you have the initial query results, you can add a table calculation from the custom fields section. Click add next to custom fields and then select table calculation. Use the custom expression option and the following syntax for the expression-- dollar symbol, open curly brace, order, underscore, items dot total underscore, revenue underscore from underscore, completed underscore, orders, close curly brace, forward slash, dollar symbol, open curly brace, order underscore, items dot total underscore, revenue, close curly brace. Next, change the format to percent and decimals to 1. Name the table calculation percent revenue from completed orders and then save the table calculation. Next, hide the total revenue measure and the total revenue from completed orders measure from the visualization by clicking on each measure's gear menu and selecting hide from visualization. Last, change the visualization type to Google Maps. You can also change the default color order in the legend by selecting reverse color scale in the values tab of the visualization settings so that higher values are green and lower values are red. You now have a map visualization of percentage of revenue per US state from completed orders in the past one complete year.

### Video - [Example: Percent of total table calculations](https://www.cloudskillsboost.google/course_templates/323/video/516816)

* [YouTube: Example: Percent of total table calculations](https://www.youtube.com/watch?v=rPSu_aedlWE)

SPEAKER: Percent of total calculations can be useful for analyzing a portfolio or market share in your data. In this example, we'll work with the order items explored to create a table calculation that shows the percentage of orders coming from each traffic source, such as email or search, out of the total number of orders. First, from the Explore tab, locate Order Items under the E-Commerce heading. Begin your analysis by getting the raw number of orders per traffic source. Navigate to the Order Items view, and select the Order Count measure. Next, select the Traffic Source dimension in the Users view so that you can get order counts by traffic source. How do we know the total number of orders? Did you spot the Totals checkbox next to Row Limit? Select it, and click Run. A Total line will appear under the five rows of data, with the number 286,183. Sometimes the total row won't match the number if you manually add the rows above it. Looker is counting unique objects, not the numbers shown in each row. For example, consider an order attributed to more than one traffic source. It will appear in the order count for each relevant source's row, but it won't double or triple count in the total row. In another example, count the number of users in each month making an order. It's possible that the same user could order every month, but they would still only total as one user versus 12 different people in a single year. Or if you wanted to know the average sale price by traffic source, the total row would show the average sale price for all traffic sources, rather than a total of the average sale prices added together. Now, next to Custom Fields, click Add, and select Table Calculation. For Calculation, choose Percent of Column and select Order Items Order Count as the source field. For Format, choose Percent and select 1 for Decimals. Don't forget to give your table calculation a clear, descriptive name, such as Percent of Total Order and click Save. You want the percent of each traffic source's order count out of the total order count. So you need dollar symbol, open curly brace, order_items.order_count, close curly brace, followed by a forward slash to divide by the appropriate total order count field. Begin typing order, and then select the suggestion for Order Count Total. Order Count Total has a LookML variable that looks very similar to the Order Count, except it has a colon and the word "total" at the end. Dollar symbol, open curly brace, order_items.order_count, close curly brace, forward slash, dollar symbol, open curly brace, order_items.order_count, count, colon, total, close curly brace. Don't forget to give your table calculation a name, such as Percent of Total Order. And choose a format. You can select Percent and 1 for Decimals and then click Save. Next, change the visualization type to bar chart and hide the order count measure by clicking on the column's gear menu and selecting Hide from Visualization. Using the Visualization settings, under Values, turn on the Value Labels to add a label for each bar. Looks nice, right? Using table calculations, you are able to show the percentage of orders coming from each traffic source out of the total number of orders. Since Looker provides many different visualization options, why don't we review some others? If you'd like to see the data as a pie chart instead, click on the pie icon from the Visualization menu. Using the Visualization settings, you can customize the labels and colors. For example, you can change the individual colors or the color palette under Series, then Collection. You can also add and customize the labels. Under Plot for Value Labels, select Labels. In the same menu for Plot, for Label Type, select Label, Value, and for Start Angle, type 90. And now the pie chart of percentage of orders coming from each traffic source out of the total number of orders is complete. You can see that with just a few simple option changes, Looker gives you the power to create multiple types of visualizations from one set of query results. Enjoy exploring all of the visualization options in Looker.

### Video - [Introducing offset functions](https://www.cloudskillsboost.google/course_templates/323/video/516817)

* [YouTube: Introducing offset functions](https://www.youtube.com/watch?v=V5igUB-2jCo)

SPEAKER: Offset functions are a subset of table calculation functions. They allow you to programmatically reference values from other rows or columns in your query results to calculate new values. There are three main types of offset functions-- regular offset, offset_list, and pivot_offset. A regular offset function is used when you want to reference a value from a higher or lower row of your results. Note that changing the order of the rows by sorting your results can turn the previous row into the subsequent row, and vice versa. In this example, there are results for a series of months in descending order-- October, September, and so on-- with the total revenue for each month. The previous month total is a table calculation that offsets the total revenue column by 1. The calculation starts with October, which is in row 1. Then it adds 1 to its row number and captures the total revenue from row 2, which is September. The subsequent month total is a table calculation that offsets in the other direction. It does a negative 1 offset. So it captures the value from the previous row. There isn't a value for October, since that is already the first row of our result set. For September, it goes back from row 2 to row 1 and gets October's total revenue. For August, it goes back from row 3 to row 2 and gets September's total revenue. As you can imagine, the sort order of your data is critical here. If you are sorting your data from newest to oldest, as seen here, you need to do a positive offset to get the previous month's data. But if you were sorting from oldest to newest, you need to do a negative offset to get the previous month's data. With these new values, you can create yet another table calculation to calculate the percent difference from one month to the next to see if business is improving or not. The pivot_offset function is used to reference values from a column to the left or the right when you have a pivot table. In this example, there is a created month number dimension with a pivot on created year. From these results, maybe you want to know, how did revenue from January 2013 compare against revenue from January 2012? How did February 2013 compare to February 2012? To determine this, the last_year_revenue table calculation looks to the minus 1 column, or one pivot column to the left, and pulls the total revenue from there. It is blank for 2012, since that is the very first pivot column in the results. The sort order matters here too, to determine whether you should be offsetting by a positive or negative value. Once again, you could create yet another table calculation to calculate the percent difference from one year to the next to see if business is improving or not. The offset_list function moves up or down a column of rows defined by a first provided value and then grabs a number of rows worth of data defined by a second provided value. The two numbers can be the same or different, depending on the results you want. In this example, the table calculation using offset_list references three rows back, or minus 3 rows, and starting at that point, gets the order count for next three rows. This means the first row where it's possible to get a full string of values is now row 4, where we can go back to row 1 and, starting there, grab the three values of 391, 359, and 388 for rows 1, 2, and 3. While this type of offset is not used as often as the first two types, it's perfect for calculating rolling averages. You may want to know, what is the rolling average number of users over the past seven days? Or what is the rolling average number of purchases over the past 30 days? That's where it might be useful to create one table calculation with the offset_list and another table calculation to determine something new, like the mean of that resulting list. In summary, offsets are a subset of table calculation functions and allow you to programmatically reference values from other rows or columns in your query results to calculate new values. There are three main types of offset functions-- regular offset for referencing rows higher or lower in a column, pivot_offset for referencing values in a column to the left or right, and offset_list for referencing multiple rows and combining their values into one new value. With these new values, you can create even more table calculations to calculate new metrics, such as the percent difference from one month to the next, one year to the next, or even a rolling average. Very powerful features.

### Video - [Writing offset calculations](https://www.cloudskillsboost.google/course_templates/323/video/516818)

* [YouTube: Writing offset calculations](https://www.youtube.com/watch?v=8vkdE6u1fxk)

In Looker, offset functions are a subset of table calculations that you can use to programmatically reference values from other rows or columns to calculate new values. In this lesson, we’ll use an offset function to calculate changes in values from one row to the next row. Specifically, we’ll apply the offset function in the Order Items Explore to find the percent change in the number of users created month over month in the year 2018. Writing offset calculations is nearly identical to other table calculations, so we’ll demonstrate writing an offset function to calculate changes in values from one row to the next row. To begin, from the Explore tab, locate Order Items under the E-Commerce heading. Using the Order Items Explore, you want to know the number of users created month over month. So begin by expanding the Users view, and selecting Month under the Created Date dimension group. Then, you need to create a filter on the Year dimension using “is in the year” 2018. You want the number of users, so you need to select the Users Count measure. Then, click Run. Although you can choose to add table calculations before or after clicking the Run button, we recommend clicking Run first when working with offsets. That way, you can see or decide on the data sort order before writing your offset function. This is important because the decision to offset by a positive or negative number depends on the sort order of your results set. Next, select column chart for the visualization type. Notice that by default Looker is sorting by the Created Month descending, which is appropriate for our upcoming calculations. To ensure accurate table calculations, be sure to not sort these results manually. Next, you can create a new table calculation. Next to Custom Fields, click Add, and select Table Calculation. When you write your table calculation, you need to use the following expression: offset(${users.count},1) This translates to: Get the count of users from each current row number +1. Don’t forget to give it a meaningful name, such as Users last month, and click Save. Now you need a second table calculation to calculate the percent change from the prior month to this one. Next to Custom Fields, click Add, and select Table Calculation. For this table calculation, you can use ${users.count} to get the current number of users, add the forward slash to divide, and then select the name of your first table calculation Users last month from the suggestions drop-down, minus one. The formula will look like this: ${users.count}/${users_last_month}-1 Give your table calculation a name such as Diff from last month, apply a Percent (0) format, and click Save. To finalize your visualization, hide the Count measure and the first table calculation for Users last month by clicking on the column’s gear menu, and selecting Hide from Visualization. Now you can see why we recommend the column chart for percent change visualizations like this one. Notice that it clearly shows you which months were above or below 0, meaning which months resulted in gains or losses of users from the previous month. And with that, your visualization of percent change in the number of users created month over month in the year 2018 is now complete!

### Video - [Example: Writing offset calculations](https://www.cloudskillsboost.google/course_templates/323/video/516819)

* [YouTube: Example: Writing offset calculations](https://www.youtube.com/watch?v=VL5b7XcLb9s)

In this example, we will review how to write and visualize table calculations to instantaneously create new metrics. We’ll work in the Order Items Explore to determine what percentage of revenue per US state is from completed orders (out of revenue from all orders for that state) in the past one (1) year. Then, we’ll create a map of the results. To begin, from the Explore section, locate Order Items under the E-Commerce heading. In the Order Items view, click on the Order Item Count measure. Then, click on the Week dimension in the Delivered Date group. Next, click on the Filter button next to Delivered Date > Date, and set the filter to “is in range” “2018-12-31” until (before) “2019-12-30”. Click Run to see the results. Your results will show the order item count by each delivery week within the window of December 31, 2018 to December 29, 2019. Now, next to Custom Fields, click Add, and select Table Calculation. For calculation, choose % change from previous row, and select Order Items Order Item Count as the source field. For format, choose Percent, and select 1 for Decimals. Don’t forget to give your table calculation a clear, descriptive name such as Percent change from previous week, and click Save. The new table calculation will now appear in the data area. Last, select column chart for the visualization type, and hide Order Item Count by clicking on the column’s gear menu, and selecting Hide from Visualization. The final visualization is now complete and clearly shows the week-over-week percentage change in the number of items delivered from December 31, 2018, to December 29, 2019!

### Lab - [Getting Started with Table Calculations and Offsets in Looker](https://www.cloudskillsboost.google/course_templates/323/labs/516820)

In this lab, you will use table calculations and offsets to create a series of visualizations from a simulated ecommerce dataset and save them to dashboards in Looker.

* [ ] [Getting Started with Table Calculations and Offsets in Looker](../labs/Getting-Started-with-Table-Calculations-and-Offsets-in-Looker.md)

### Quiz - [Module 4 Quiz](https://www.cloudskillsboost.google/course_templates/323/quizzes/516821)

#### Quiz 1.

> [!important]
> **If you want to write an offset calculation to reference the values in a column to the left or right of a particular column for a rolling average when using a pivot table, which offset calculation type should you choose? Please choose the best answer.**
>
> * [ ] None of the suggested offset calculation types apply to this scenario.
> * [ ] offset_list()
> * [ ] offset()
> * [ ] pivot_offset()

#### Quiz 2.

> [!important]
> **What are the recommended Looker best practices on when to click the "Run" button, with respect to adding an offset calculation? Please choose the best answer.**
>
> * [ ] Do not click the "Run" button at all.
> * [ ] Click the "Run" button after.
> * [ ] There is no "Run" button when adding an offset calculation.
> * [ ] Click the "Run" button before.

#### Quiz 3.

> [!important]
> **To write a table calculation, you find the "Custom Fields" section of the field picker in an Explore, click on the "Add" menu popup, and then choose the "Table calculation" menu option.**
>
> * [ ] False
> * [ ] True

#### Quiz 4.

> [!important]
> **An offset calculation is a totally independent function type compared to a table calculation.**
>
> * [ ] True
> * [ ] False

#### Quiz 5.

> [!important]
> **If you pivoted your data by a dimension in Looker, what data in turn would be displayed? Please choose the best answer.**
>
> * [ ] Data by filter criteria.
> * [ ] None of the suggested data options will be displayed.
> * [ ] Another dimension.
> * [ ] Data by active measure.

#### Quiz 6.

> [!important]
> **In the Edit table calculations dialog box, in which field will you actually write the coding for your new table calculation? Please choose the best answer.**
>
> * [ ] Expression.
> * [ ] None of the suggested fields apply to the Edit table calculations dialog box.
> * [ ] Format.
> * [ ] Calculation.

#### Quiz 7.

> [!important]
> **What are the general use cases for choosing to write a table calculation? Please choose the best answer.**
>
> * [ ] None of the suggested options are use cases for choosing to write a table calculation.
> * [ ] To prototype a new dimension or measure.
> * [ ] To support a results set only.
> * [ ] To prototype a new dimension or measure, and/or to support a results set.

#### Quiz 8.

> [!important]
> **What type of table calculation would contain the substring() function in its coding? Please choose the best answer.**
>
> * [ ] Date and time.
> * [ ] Mathematical.
> * [ ] Logical.
> * [ ] String.

#### Quiz 9.

> [!important]
> **Which is a key characteristic of table calculations? Please choose the best answer.**
>
> * [ ] They run only on your query results.
> * [ ] They cannot be saved to a Look or dashboard.
> * [ ] They are stored permanently in your underlying database.
> * [ ] They run directly on data in your underlying database.

#### Quiz 10.

> [!important]
> **To write an offset calculation in Looker, you select the "Offset calculation" menu option from the "Add" menu popup in the Custom Fields section of the field picker in your Explore.**
>
> * [ ] False
> * [ ] True

#### Quiz 11.

> [!important]
> **The four primary types of table calculations are: string, mathematical, logical, and date and time.**
>
> * [ ] True
> * [ ] False

#### Quiz 12.

> [!important]
> **You can pivot your data using either dimensions or measures in Looker.**
>
> * [ ] True
> * [ ] False

## Creating new Looker content

This module explores the creation of single, stand-alone reports (Looks) and dashboards, which can be used to combine individual visualizations.

### Video - [Creating new Looks](https://www.cloudskillsboost.google/course_templates/323/video/516822)

* [YouTube: Creating new Looks](https://www.youtube.com/watch?v=agayeqHWRCM)

SPEAKER: Looker provides many ways for you to analyze, visualize, and share your data. If you're looking to create a report that answers one specific question of your data, you should consider creating a Look, which is a single standalone report in Looker. A Look is a single visualization designed to answer one specific data-related question, which is different from a dashboard, which generally contain multiple visualizations and can answer many questions. Looks are built from the results of a query in an explorer by data explorers, not data viewers. Once created, a Look can be saved, favorited, shared, or even scheduled for regular delivery. You can also drill down into the data presented in any Look by clicking on Explorer from here, which will take you back to the underlying explorer where you can modify the Look as desired. Creating a Look using your data is very easy, as long as you understand the components of an explorer and how they work. That's really the key here. If you understand how to work with dimensions, measures, filters, pivots, as well as table and offset calculations within Looker, you already understand how to assemble a Look. Let's walk through an example of assembling a Look in Looker together. First, you should always start with the question that you have of your data. To get the most value and clarity from your Looks, ensure you are asking a clear, straightforward, and, most importantly, measurable question. For example, you may want to know, what were the yearly revenue values for each month in my data? With this question in mind, let's assemble the components for this Look within the explorer. Next, to begin assembling your look, start with the explorer that contains the most appropriate data for your analysis and visualization, and select the dimensions and measures needed to answer your question. Then click Run. For example, selecting the month name dimension and total revenue measure in the Order Items explorer will show you the revenue for all order months in all years for which you have data, for example, January 2018, January 2019, et cetera. This doesn't yet answer your question, but this presentation of your data gets you well on your way. For this example, if you want the revenue totals for each month within the time frame you've specified, you need to pivot your data by the order items created here. Pivoting this data will create a matrix in which each year will now be a column that can be easily represented in the visualization. When you apply the pivot, you can see revenue totals for each month of each year between 2018 and 2021. If you only wanted to see particular years or dates, you could apply a filter to date to limit the results returned by the query. In this case, you want all years of data, so no filters needed. The pivoted result answers your question, so you can now turn your attention to finding the best visualization for this view of your data. Looker provides a number of different visualization options depending on the data you are analyzing and the question you are asking. For this Look, a single line chart can clearly highlight the changes in monthly revenue by year. You can further refine and customize this visualization to improve clarity for viewers. To see options for formatting and presenting data within the visualization, click on the Edit menu at the far right of the Visualization Bar, also referred to as the Visualization Settings. Depending on the type of visualization, you will see different options for positioning, coloring, labeling, and more. For us, we will change the line interpolation from linear to monotone. So now that the explorer is configured like you want, you can click on the Gear Menu in the top right of the screen next to the Run button and see the many options available for saving and sharing these results. For example, you can save your explorer results and visualization to a look or a dashboard, download, or send it, save and schedule it for delivery to others, share a URL to share this configured explorer with others, or even send this data to Looker Studio for more advanced visualization configuration. For now, though, to save your visualization and explorer results as a Look, select the Save menu and then as a Look. Finally, in the Save Look dialog box, you will be asked to provide a name for your look, as well as an optional description field. You can also decide where to save this Look, either just for yourself in your personal folder or within the shared folder for easy access and discoverability by others in your organization. Once you've configured those items, click on Save to save your Look or Save and View Look to save and see your finalized Look. And with that, you've now created a new Look. Wasn't that easy?

### Video - [Creating new dashboards](https://www.cloudskillsboost.google/course_templates/323/video/516823)

* [YouTube: Creating new dashboards](https://www.youtube.com/watch?v=sD5jLUMnahY)

SPEAKER: In Looker, dashboards can be used to combine individual visualizations, which are referred to as tiles on the dashboard. Let's dive into creating and editing dashboards to understand how they can be used to serve up multiple visualizations. Just like a look is a single visualization designed to answer one specific data-related question, a dashboard usually contains multiple visualizations and is designed to answer multiple data-related questions. If you have data explorer access in your Looker instance, you can create new dashboards by saving visualizations from an explorer or an existing look to a new dashboard. And to make it easy, the process is the same for both in an explorer or look, simply click on the settings gear on the top right, and you will see the Save fanout menu providing you with options. From an explorer, you can save to a new look or to either an existing or new dashboard. From a look, you can save to either an existing or a new dashboard. For our example here, let's save this look to a new dashboard so click on the gear menu, select the Save fanout menu, and then choose as a new dashboard. Additionally, you can also save a look to a dashboard directly from the details panel at the extreme right of the look by clicking on the Add to dashboard link. But back to our previous example. First, let us give the dashboard a new name, in our case Business Revenue. Then select the folder where you want to create your new dashboard. For example, Shared Folders is a good location if you want others at your organization to easily find your new dashboard. We could also choose to add global dashboard filters during this initial dashboard creation, but we cover filtering dashboards elsewhere. When you've given the dashboard a name and selected the folder where it will live, click on the save button to create the dashboard. Your new dashboard will be listed under the folder that you previously selected. The process to save to an existing dashboard is almost entirely the same except you choose the dashboard from the folder list. You can now create your own dashboards in Looker from explores and looks.

### Quiz - [Module 5 Quiz](https://www.cloudskillsboost.google/course_templates/323/quizzes/516824)

#### Quiz 1.

> [!important]
> **A data explorer end user can create a dashboard in two ways from an Explore: the Save fanout menu option from the top right-hand gear menu in Explores and Looks, and the "Add to dashboard" link at the extreme right of a Look in the Details panel.**
>
> * [ ] True
> * [ ] False

#### Quiz 2.

> [!important]
> **Who can create new dashboards in Looker? Please choose the best answer.**
>
> * [ ] Data viewers.
> * [ ] Data explorers.
> * [ ] Neither data viewers nor data explorers.
> * [ ] Both data viewers and data explorers.

#### Quiz 3.

> [!important]
> **Data explorer end users create Looks from what part of the Looker platform? Please choose the best answer.**
>
> * [ ] Folders.
> * [ ] Explores.
> * [ ] Boards.
> * [ ] Dashboards.

#### Quiz 4.

> [!important]
> **A Look is essentially a visual data report designed to answer one specific question of your data.**
>
> * [ ] False
> * [ ] True

## Sharing Looker data with others

This module explores how you can share or export content from Looker.

### Video - [Sharing and scheduling Looks](https://www.cloudskillsboost.google/course_templates/323/video/516825)

* [YouTube: Sharing and scheduling Looks](https://www.youtube.com/watch?v=HC-YFnFV8V8)

Anytime you want to share or export content from Looker, we call that “data delivery.” Let’s explore the various ways you can accomplish this and why you might choose one method over another. To deliver data from Looks in Looker, you can click the gear icon in the top right corner of a Look to review the data delivery options, which can vary slightly depending on which object you want to deliver. Dashboards have their own options that are covered elsewhere. Let’s review the data delivery options for Looks. To find the best option for your current use case, you’ll want to think about your desired delivery frequency. If you’d like to export data on a one-time basis, you can download or send it. Downloading extracts the data to your own computer. Looks support downloading in a different file formats, including a CSV, a zip file of one or more CSVs. You can also select PDF, or PNG, which behave as a screenshot image. Sending allows you to deliver the data somewhere else. The most popular destination is email; for example, you could email the dashboard to yourself and your manager. Depending on your permissions and what your Looker administrator has configured in your own Looker instance, you might see other available destinations such as Amazon S3 or Google Drive. Looks and dashboards can each have different options for delivery destinations, so don’t be alarmed if your Looker instance lets you send a Look to specific different places but a dashboard to different places. Now, if you or other users need to review changes in the Look on a recurring basis, you can schedule to be sent to them. This is basically the same as sending it, except you can set a delivery frequency such as daily or weekly. This is useful if you’d like to have a spreadsheet of the Look’s data automatically delivered to your inbox, say every Friday afternoon at 3:00pm local time. Let’s explore how to accomplish that. When you select the option to schedule a look, you will need to specify some details, including where the Look is going and when. First, give your schedule a title, and then identify where the Look should be delivered, such as email or another tool. Also, depending on what your Looker administrator configures and adds, you may see other types of data destinations. Next, if delivering by email, then enter the email address or addresses. You can also send a Look to any email alias to which you have the permission to send email. You can also include an optional message, if you’d like, to give your recipients a heads-up on what they’re going to see in this data. Then, choose the desired file format. This is the actual file type or presentation the Look will have for recipients. For our example, let’s choose a simple Data Table. Next, specify the type of file you wish to send, in this case, a . csv file. Because you want to send this Look on a regular schedule, select the Repeating interval option and then choose Weekly, Friday and 3:00pm date and time options. Additionally, you could also choose the Datagroup update trigger, which would deliver data when change thresholds in your data are met or exceeded. We will not be doing that here. So, finally, save your changes, in order for Looker to commit to this scheduled delivery. Now, every Friday afternoon at 3:00pm local time for the recipients, they’ll receive this Look as a . csv file via email. It’s really that easy with Looker! And now our final delivery option for Looks - if you want to send others the most recent data, instead of something like a snapshot, you can simply click Share. … and then copy the URL of the Look, and send it to the people who need to see it. As long as they have the right permissions to view the Look, they can view it that easily!

### Video - [Sharing and scheduling dashboards](https://www.cloudskillsboost.google/course_templates/323/video/516826)

* [YouTube: Sharing and scheduling dashboards](https://www.youtube.com/watch?v=SQhsNB37uEU)

In Looker, data delivery is when you want to share or export content with others. You can deliver data from Looks, Explores, or dashboards, and to make it easy for you, the process for each is very similar. In this lesson, we will focus on delivering data from dashboards. Note that everything in this next section also applies to individual dashboard tiles, so you don’t need to download, send, or schedule an entire dashboard if you only need to share a single tile or a few tiles. To deliver data from dashboard in Looker, you can click the three dot icon in the top right corner of the dashboard to review the data delivery options, which can vary slightly depending on which object you want to deliver. Looks have their own options that are covered elsewhere. Let’s review the data delivery options for dashboards. If you’d like to export data on a one-time basis, you can choose to either Download or Send it. Downloading extracts the data to your own computer. There are a number of output formats you can choose from. If you choose PDF, you have options to select the paper size, expand tables to show all rows, and/or arrange the tiles in a single column. The last option is useful if you expect that people will need to view the PDF on a mobile device, as it stacks all the tiles up and makes it easier to view them on a smaller screen. If you choose CSV, Looker exports a CSV file for each tile that contains data on your dashboard and packages them together in a ZIP archive. Now, sending the data one-time is an option available under Schedule Delivery. Scheduling a delivery allows you to deliver the data somewhere else, outside of Looker. The most popular destination is email; for example, you could email the dashboard to yourself and your manager. Depending on your permissions and what your Looker administrator has configured in your own Looker instance, you might see other available destinations such as Amazon S3 or Google Drive. If you need to ensure that someone will always be able to view updated data when they need it, the best approach would be simply to send them the link to the dashboard itself. That way, they can open it directly in Looker where they can ensure that they will always be looking at the most current data. You can easily get the URL for a dashboard by copying it from the Get link menu option. From here, you can copy the dashboard link into your clipboard by clicking the Copy to Clipboard link, and you can also choose whether to include the current filter values, depending on the recipient’s data needs. However, if you or other users need the dashboard on a recurring basis, you can schedule it for regular delivery. This is basically the same as sending it, except you can define a frequency, such as daily or weekly. This is useful if you’d like to have the dashboard PDF automatically delivered to your inbox, for example, every Monday morning before you start your work week. Let’s take a closer look at the options for scheduling a dashboard. There are a few key pieces of information that you need to provide, in order to send a dashboard either one time or on a recurring basis. First, consider how frequently you want to schedule the dashboard. Under Recurrence, you could choose daily, weekly, etc, or choose Send now to send it just this one time. We wanted to schedule this dashboard for delivery every Monday at the beginning of the work day, so we defined our frequency as Weekly > Monday > 8:00am local time. Next, where should the dashboard go? Email is the most commonly used destination. Based on your choice on the delivery destination (email, Google Drive, Amazon S3, etc), you would need to configure specifics for that destination. In choosing Email for the destination, we need to enter one or more email addresses or aliases. Last, in which file format should the dashboard be sent? In addition to PDF, you can send a PNG image snapshot, or a ZIP file containing one or more CSV files. The dashboard you wish to share may have global filters already applied to it, so you could decide which filters to activate or deactivate, depending on the audience. In our example dashboard, there are no filters included yet, so we won’t do anything here. Before you send the dashboard, you can use the Advanced options section to include a custom message, perhaps letting the recipient know what this data is and why they’re receiving it. You can also set the delivery timezone for the recipient or recipients in question, so that time-sensitive data is properly contextualized and presented to the recipient. With everything configured, you can now click Save to commit your new dashboard delivery schedule. And with that, Looker makes it easy for you to share dashboards with anyone you want, as often or as little as you want!

### Video - [Tile-level dashboard alerts](https://www.cloudskillsboost.google/course_templates/323/video/516827)

* [YouTube: Tile-level dashboard alerts](https://www.youtube.com/watch?v=9zjpgXDklWg)

In this lesson, we will focus on understanding and configuring the conditions for alerts that indicate data changes to individual tiles in your dashboards, or other dashboards to which you already have access. Alerts in Looker enable you to specify data conditions that, when met or exceeded, trigger a notification to be sent to specific recipients at a desired frequency. Alerts are created on dashboard tiles that have at least one numeric measure or table calculation in the tile’s visualization. Each alert captures the dashboard and tile settings in place when created. With enhanced alerts enabled, many of the changes made to dashboard filters or tile content will sync to the alert, with some exceptions. The bell icon on a dashboard tile indicates the number of alerts set on that tile (that you are permitted to view), and provided that your Looker administrator has turned on access to this feature. Depending on the dashboard tile’s visualization type and the kinds of fields that are present in the visualization, Looker checks your data in different ways. When you create an alert, it will be one of these types: Single value alerts (used only with single value visualizations) — Looker checks the data based on the value that is used in the visualization, which is the first row of the results table. Time series alerts (used when there is a date or time dimension in the tile query results) — Looker checks all new rows that have not been seen before (based on the date or time dimension in the query). and Categorical alerts (neither single value nor time series) — Looker checks all rows and pivot values unless a specific row or pivot value was selected when the alert was created. When you receive an alert notification via email, the message will include: A link to the dashboard for the tile on which the alert is based. The value that triggered the alert. The visualization for the tile on which the alert is based. and Options to unfollow or, depending on your permissions and who owns the alert, to edit the alert. To create your own tile-level dashboard alert, start by clicking on the alert bell icon on a tile in a dashboard you own, or have access to. If there are alerts already set on that tile, Looker displays a list of the alerts that you are permitted to see. From the list, click New. However, if there are no previous alerts set on that tile, Looker will automatically display the alert creation window. There are a series of configuration items and opportunities for customization in the alert creation popup. First, give your new alert a title. Something logical and easy to understand by others. Looker automatically suggests such a title by default, but you can change it to whatever you like. Next, you will configure the logic that will trigger your alert. You will provide a single field to review, a single condition and a single threshold value. If you need more than this, configure additional alerts as needed. The next configuration option involves how Looker will send the alert to recipients. Without additional integrations configured and enabled by your Looker administrator, you can only choose Email. Enter in the email addresses or group aliases for the alert as needed. The frequency section provides a great deal of flexibility in when and how often alerts are sent to recipients. For our example use case, we’ll configure the alert will send every Wednesday at noon. It will include all instances within the past week where the logic conditions were met, not triggering an alert every time the conditions met. Finally, you must decide if you want this alert to be visible to every user of the dashboard (public), or restrict it for use only by yourself (Private). For our example use case, let’s keep it public, and click Save Alert to commit the alert. As previously mentioned, you can also follow public alerts created by others for dashboards to which you already have access. Clicking on an alert’s Follow button will allow you to receive the alert notification, exactly how it was configured. You can also review the global list of alerts for all of the alerts you’ve either created yourself, or have chosen to follow. Simply click on the user profile icon in the top-right corner of the application, and select the Alerts menu option. You can review, follow or unfollow, view, edit or disable an alert. Additionally, if your Looker administrator has enabled Enhanced Alerts, you can also filter your alerts by certain criteria and view additional details about it, such as run history, visualizations, and whether it remains synchronized to its parent dashboard. You should now be ready to configure and follow tile-level dashboard alerts in Looker!

### Quiz - [Module 6 Quiz](https://www.cloudskillsboost.google/course_templates/323/quizzes/516828)

#### Quiz 1.

> [!important]
> **Which of these options is NOT a sharing and scheduling method for dashboards? Please choose the best answer.**
>
> * [ ] None of the suggested options are sharing and scheduling methods for dashboards.
> * [ ] Schedule delivery.
> * [ ] Share via URL.
> * [ ] Send.

#### Quiz 2.

> [!important]
> **All end users can see and follow all tile-level dashboard alerts if they so choose.**
>
> * [ ] False
> * [ ] True

#### Quiz 3.

> [!important]
> **End users can download a dashboard to their local computer as .csv, .zip, .pdf or .png file formats.**
>
> * [ ] False
> * [ ] True

#### Quiz 4.

> [!important]
> **Which of these options is NOT a sharing and scheduling method for Looks? Please choose the best answer.**
>
> * [ ] Share.
> * [ ] Send.
> * [ ] Schedule.
> * [ ] Pin to a board.

#### Quiz 5.

> [!important]
> **What is the minimum number of numeric measures or table calculations in a tile's visualization needed to support a tile-level dashboard alert? Please choose the best answer.**
>
> * [ ] Zero (0).
> * [ ] Two (2).
> * [ ] Three (3).
> * [ ] One (1).

#### Quiz 6.

> [!important]
> **End users can download a Look to their local computer as .csv, .zip, .pdf or .png file formats.**
>
> * [ ] False
> * [ ] True

## Course Resources

PDF links to all modules

### Document - [Course Resources](https://www.cloudskillsboost.google/course_templates/323/documents/516829)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
