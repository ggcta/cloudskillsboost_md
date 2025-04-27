---
id: 518
name: 'Planetary Scale Earth Observation with Google Earth Engine'
datePublished: 2023-03-15
topics:
- Image Processing
- JavaScript
- Google Earth Engine
type: Course
url: https://www.cloudskillsboost.google/course_templates/518
---

# [Planetary Scale Earth Observation with Google Earth Engine](https://www.cloudskillsboost.google/course_templates/518)

**Description:**

Learn how public sector agencies and academic researchers leverage Google Earth Engine to distill meaningful insights from petabytes of Earth Observation at planetary scale. Google Earth Engine is a fully managed geospatial platform that has enabled research for more than a decade in environmental areas such as forestry, agriculture, water, and sustainability.

**Objectives:**

- Summarize Google Earth Engine use cases, features, and benefits.
- Create composites in Google Earth Engine.
- Analyze the planet and turn data into actionable insights.
- Use Google Earth Engine for commercial purposes.

## Introduction to Google Earth Engine

This module explores the various use cases, features, and benefits of Google Earth Engine.

### Video - [Presenter introductions](https://www.cloudskillsboost.google/course_templates/518/video/369035)

- [YouTube: Presenter introductions](https://www.youtube.com/watch?v=NxyutdfOdbk)

Hi, everyone. I am a recent member of the Global Public Sector Customer engineering team and I am specializing alongside Sean Wohltman with Earth Engine. So we're so excited today to be able to talk through what we do and how we can learn about it. And hi everyone. Yeah. Sean Wohltman I've been to Google for about 13 and a half years and they've always been focused on our geospatial technologies from Google Earth to Google Maps and most recently have been focused on Earth Engine, which is our analytical platform for petabytes and petabytes of geospatial Earth observation data. So thank you so much for joining. Look forward to today's session and answering any questions that you may have. Hey Dani how about you starts off with an example Application of Earth Engine.

### Video - [Demo: Earth Engine application](https://www.cloudskillsboost.google/course_templates/518/video/369036)

- [YouTube: Demo: Earth Engine application](https://www.youtube.com/watch?v=wKLmKXM5OFE)

So before Sean goes into more details about what Earth Engine is exactly and everything about it, I just wanted to show a brief little demo about the one really cool application that one of our users have done with Earth Engine before. So here, go Golberg. She's a scientist in our scientist, and she created this application to follow mangrove loss in different parts of the world. And so what she was able to do was gather imagery, process it in a very innovative way, and follow whether or not these mangroves were lost to wet soil, dry soil or water, and which specific loss drivers were the main culprits like erosion, commodity settlement, etc.. And so I just wanted to go ahead and share the actual application here and go and see can everyone see the screen? Yes. Okay. So here we are in Bangladesh. She was able to follow see the mangrove loss throughout different periods of time. For example, from 2000 to 2 out of five and the next couple of ranges of five years. And she was able to create this really, really, really cool application. So I'm from Florida myself, and the Everglades are the biggest restoration project, for example, that the United States has ever taken. So she was able to follow all the locks throughout the years and the lost drivers as well. So, for example, here we can see that most of the Everglades mangrove erosion is due to erosion. And so this is just one tiny little example of the different kinds of applications that Earth Engine can help users build. And we, of course, provide this for individual researchers like Goldberg, but we also provide this for commercial use. And so Sean will be able to explain a little bit more about that.

### Video - [Introduction to Earth Engine](https://www.cloudskillsboost.google/course_templates/518/video/369037)

- [YouTube: Introduction to Earth Engine](https://www.youtube.com/watch?v=F95jfJVVlKA)

That was actually Eliza Goldberg was a high schooler when she built that application. So she's a fantastic scientist. She's at Stanford right now, and she was interning at NASA when she started to build that monitoring, global monitoring of mangroves. Pretty ambitious for a high schooler. But she was able to do that because of the platform that we've built here with Google Earth Engine. We built Earth Engine about a decade ago. So we started building this this this platform for doing this, because Google saw a very common pattern in the GIS or remote sensing space where very little time is actually available to scientists to do their analysis or, you know, test their hypothesis. Most of their time is spent doing all the things that might be familiar to a lot of you, especially if you're in this space. It's provisioning and getting access to virtual machines or physical hardware. It's downloading data, it's unzipping data, it's getting all the data ready and all that data prep. And so everybody goes and does the exact same thing over and over and over again. There's got to be a better way. And so Google thought, well, there probably could be a better way if we did that once and we made a massive amount of data available and we built a purpose built platform that had access to Google's compute, we could probably allow users to change this pie chart dynamic so they could spend most of their time working on their science, not their infrastructure. It really did start with the data. About a decade ago, a little bit longer. The way that users were able to access the investment that the United States made in our program called Landsat changed dramatically. It used to be that you had to pay anywhere from $50 to a couple hundred dollars, in some case thousands of dollars for a scene for the access to this data. And if you didn't have to pay for it, you might have to pay for somebody to go and take it off of tape, rehydrate it, and then make it available to you. You'd get like an email in a day that, Hey, this is ready for you to go download. And so that all just added to that whole part of the pie that was like really annoying and blocked a lot of science. So Google worked with Arrow's data Center and we were able to get all of the Landsat mission going back to the 1970s and bring all of this data back online and put it into Google's data centers. And importantly, it's not just putting it online and saying, Great, now you come in, unzip it and use it. We made it analysis ready. So when you look at this data, you know, it's not what you see When you open up Google Maps, you open up Google Maps and everything's beautiful when you're taking pictures of the Earth every single day. It's a wet planet, right? Over 70% water. That means a lot of times are going to be clouds in the areas that you're looking. But the important thing is I mentioned the time range and these sensors collect multiple times day. They're painting the earth essentially as they're collecting data. So for any given spot on Earth, based on the revisit rate of the sensor, you're going to have a very, very, you know, deep stack of imagery. So in a simple example, for any given place on earth, if you have enough pictures of it, we can run anything from a very simple algorithm, like looking at the median pixel value to something more complex that might take a look at some key data that you might have of the cloud cover, etc.. And what we can do is compress that down then into a mosaic of a cloud free area. So you take that cloudy picture of Scotland that I just showed you and it becomes this. All right. So you have a Time series that's allowing you to create this synthetic mosaic of that area, which allows now to do analysis over that entire area. We worked on a pretty cool project and continue to work on it with time called Google Timelapse. This is an interactive, you know, VCR or DVR of the world. And there's a lot of very interesting climate examples. You saw the change that Eliza was able to point out in the Mangrove application that Danny showed some of the interesting ones here, like Glacier Retreat in the top left. The bottom left is showing Las Vegas expanding, the Metro center expanding as Lake Mead is contracting. And on the top right, you have a what was a very successful TerraForm Ming operation in the middle of Saudi Arabia until they tapped out the aquifer and then that project failed. So this gives us a way to be able to look at the planet and understand what's happening over time. There's three main components of Earth engine. The first one being the data catalog that I mentioned. I'll talk a little bit more about that. The second is the computational platform, and it's not a download desktop, just software. It's open up a web browser and start coding. It's completely serverless and fully managed environments. And then the final piece is our users. We have over 50,000 active monthly users, our listserv, our Google Group, which spans a decade, is full of the best researchers in the remote sensing space that are using this platform to study change on the on the planet. The catalog is now north of 800 datasets. This is a both primary and secondary data sets, meaning that our users contribute back to this data catalog by watching. By utilizing that the data that we have and then creating new things like crop classifications or or meteorological data. It's about 50 petabytes at this point and it grows out a petabyte a month right now. A lot of that's coming from the additional datasets that we have from the European Space Agency. So we're getting all the sentinel missions in there as well. And as we look to the future, this is going to grow maybe 50 petabytes a month in not too long. There's a massive radar mission called Nissar, but nascent in India. We're working on to be launched in the next couple of years, and it's just going to be a tremendous amount of Earth observation data coming online. The computation piece is really, really interesting. Now, we learned a lot from the way that Google Maps changed the world. You know, it didn't. It used to be you'd go to like MapQuest and you'd say, I want a picture of Falls Church, Virginia, and you'd wait and wait, and a server would come back right with that one image. And we said, Wow, we can make that a lot faster if we pre tiled the map tiles. So that rather than calling one big image, you were calling little tiny 256 pixel images. Same approach can be done if you take GIS data, which typically is these large, you know, multi gigabyte or tens of gigabyte files got tips and used to have to load them in a desktop software. If you wanted to calculate slope, you had to go pixel by pixel, you know, bit by bit to be able to calculate slope. And that takes a lot of resources. And we said, well, what if we did the same thing we do with the map tiles? What if we pre style this and then we write our algorithms so that they work just on those little pieces? Well, now we could shard that off. And being a geographic problem, it's embarrassingly parallel, right? You can just put that across multiple machines, you know, and do the do the analysis. The tricky part is what happens when it comes across the edges and how do you handle your slope as it goes across two different tiles. But that's what our attention does, does for us. This is the code editor, and this is where the majority of our users in Earth engine spend their day. I said, I'll show you a couple of examples of this live. Nothing to install. It's just a website and it's a an IEEE that allows them to load the data from a catalog or write an algorithm and then map that algorithm over the imagery in the data that they have and then create some sort of statistic, some sort of indices that they're interested in calculating, or maybe they're interested in just generating a new graphic product that kind of interactive compute. Then we also have a set like an idea where, okay, I've tested my algorithm. I'm happy with how it's working now. I want to run it for the entire world. Maybe I'm looking at global or global surface water or global forest extent, and I want to now map that over the entire world. This takes millions and millions of hours of compute sometimes. So we do this in a batch mode, which is equivalent to somewhat using a preemptive VMs. These jobs could be interrupted and restarted, but allows us to access like massive resources like Google to do these computations. We don't lock you into just our software, though. Everything at Google starts with an API and the APIs for Earth Engine. We have a Python SDK, plus we just have a rest API. So we have a lot of users that are building applications on top of Earth Engine that reach in and use these APIs to access the data, do analyzes and then publish their, you know, update their front ends or dashboards.

### Video - [Common Earth Engine use cases](https://www.cloudskillsboost.google/course_templates/518/video/369038)

- [YouTube: Common Earth Engine use cases](https://www.youtube.com/watch?v=-Q9k_CL7xLM)

So that's enough about the history. I want to jump. Into some of the use cases, how people are using this, especially in public. Sector. And also demo the platform. I think the. The first groundbreaking moment for us. You know, once we launched. Earth. Engine was seeing it adopted in the scientific community and 2013. Dr. Hansen at the University of Maryland. Said, wow, finally a man blocked. From what I've. Always wanted to do, which is to look at. The world and understand. The extent of our. Forests. And do. So at 30 meters. You know, we had other maps previous to. That, but at that high resolution and look at the. Time series. It's not just to know where the. Forests are now. I want to. Go back 30 years where the forest, where are we losing forests? Where are we gaining forests? What is. Responsible forestry. Management look like? What is. Irresponsible forestry management. Look like? So he did that and when they went to batch mode, there was 1000000 hours of computation. You know, back. In 2013 that was quite. A bit and took about four days to complete. This. But previously this was not possible. Nobody would have been able to do this in the lifetime of. Of their traditional. GIs. So it was really cool because. It was the first time. That something like that was generated and Google helped do it. And our researchers actually. Helped Dr. Hansen do this, and they published in the Journal of Science. And since then it's just been off to the races. It is literally exponential growth in terms of the number of papers that are published each year that use Earth Engine. As the core foundation. So science. Nature, remote. Sensing. These major journals, Earth Engine is extraordinarily popular. Inside of them. But in the public sector. What's really, really been. Cool is to see how agencies who have. A remit over forests or water or agriculture. Take the science and operationalize it. What I mean by that is Dr. Hansen did this. Initial research, generated this. Dataset. Then we had folks up in Oregon State University in partnership with the U.S. Forest Service, take that implement. Land, surrender. On top of it. And today. That powers a system. Called land Change management. Monitoring system for the U.S. Forest Service. Which allows them to. Monitor over 200 million acres of the. U.S. national. Forests. And they're looking for disease. They're looking. For forest maintenance. Management. Indicators in terms of. Where they may need to do controlled. Burns or where they may. Need to help. You know, the greening process. And we also see at the state and local level up in the. Alberta Biodiversity Monitoring. Institute. They're looking at ecological change for the entire province of Alberta. And also. Monitoring forestry industry in that province, which is very prevalent. Here's an example. That I think is pretty powerful. This is LCMS, and the top is showing you the hundreds. Of terabytes. Of data for these two national. Forests. And they do this for all the national forests. Right? And you can see some changes occurring. You're seeing. Gain these. Like green. Spots, which are showing. That the forest is coming back. Maybe there was a forest fire there. Previously and then they want to categorize loss. Do the. Trees suffer like a catastrophic. Loss in one season or are they slowly dying? And in Colorado, you might be. Aware a lot of our Western states, there's. This. Pine boring beetle. Infestation. And so what you're seeing here, distilled is is. How the forest changes over time. And for a decision maker. To not have to sit and. Sift through tens or hundreds of terabytes. Of data, but instead have a graph that's showing them how these things change, can help them set warnings and automate processes and decisions based on what they're seeing. In the forest. We also allow you to bring third party datasets to the party, so we have our own. You know, public domain data sets, but we have. Customers that want to bring in higher resolution. Data. So this is a quick little application to show you an agricultural. Customer. Who's looking at Planet Planet is a smallsat provider, and this customer. Gets a three meter base map. Of the United States. For all the agricultural growing regions from planet every two weeks. So what I'm. Showing here is. The visual component, the visualization on the left hand side, and this little swipe map is just one of our UI elements to allow you to take a look at an API or the vegetation index. So because this is a. Four band. Product, I can see where the healthy vegetation is and I can step. Through multiple years. Multiple weeks. Of the summer and I'll. Start to see more and more vegetation start to. Sprout out here. In the Texas west Texas. Desert. And you can see places that have, for instance, center pivot irrigation. Where they're actually cultivating crops. Out in the middle of the desert. So they're able to look at this and see how that changes and able to do so again. At three meters, which is, you know, more than appropriate for this type of agricultural. Use case. But it's not just about visualization, right? We can make all the pretty graphics we want, just like the forest example. They want to actually extract data here. So an example of this, that same planet data can be used to look at individual fields and different crop types. So there's. A data layer in earth. Engine called the crop. Data layer. It's provided by the Natural Agricultural. Statistical Service of the USDA. And what they can do is they can click on any one of these fields. And if you have access to that. Three meter base. Map, you can now look at a crop like alfalfa and look at how. That crop is progressing, you know, throughout the summer, throughout the growing. Season. And you see these peaks and valleys which are showing that the vegetation and health, well, alfalfa is a crop that is. Grown and. Then cut. And then grown. And cut multiple times in the season. And that's what you're seeing. In that graph. And this type of interactive use. I can click around. And I can go run that analysis. It's a great tool because I can write it once and then I can share this tool and somebody else can use it. But it is a little bit slow because I have to. Do this for each. Individual field. That's where batch mode comes in. So a great nonprofit that. Google and the Environmental Defense Fund are working with, it's called Open ITI. It stands. For evapotranspiration. And what they're doing is they're looking to see how much water is being utilized by all of these fields, millions and millions of fields in the western United States and the western United States. You know, they're, you know, severely impacted by drought right now. And so you have this. Disparity where. You have some of these fields that are showing the yellow. Or brown. Which indicates that they indicate that. Are just relying probably on on the natural rainfall. Which is not all that much compared to these center. Pivot irrigation. Fields that are bright blue, which is telling us that there's a lot of water coming off of those fields relative to the fields around them. But how is that possible? While the only way it's possible. Is they're being. Supplemented in some way, right? They're being supplemented by probably an. Aquifer or some other sort of source of water maybe is coming from a river. And so this allows. Managers to be able to understand which farmers and which fields are utilizing water in an area and. Potentially doing so in a way that's maybe not equitable. But I want to point out you saw how slow it was for me to click on each one of those polygons and get that analysis open. It is running this data constantly and so. I can move around here and you can see. How quickly this is updating. They're doing these batch analysis every single night populating a non relational database to be able to have this slick interface on top of Earth engine. So just to give you an idea of what design possibilities. There are, another really interesting. Use case comes from like climate. Monitoring. This is from the National Geospatial Intelligence Intelligence Agency, and actually the Columbia. University Capstone project. Where they're looking at coal, coal. Fired power. Plants. Now, this one's not using. Standard. Visual imagery. Instead, it's relying on Sentinel one, which is a SLR or synthetic aperture. Radar. Satellite. And it's very, very. Interesting because with certain countries making certain climate pledges that, okay, we're going to cut down our carbon output, you wouldn't expect them necessarily to be building a. A brand new coal fired power plant. But sure enough, this red indicates disturbance. So that no one is looking at this area multiple times and we're looking at the disturbed backscatter disturbance of the changes in height. And it's very, very. Telling when this. Particular area. Started doing some some construction. Right. And so we can pinpoint when construction happened by using these types of sensors.

### Quiz - [Quiz: Introduction to Google Earth Engine](https://www.cloudskillsboost.google/course_templates/518/quizzes/369039)

#### Quiz 1.

> [!important]
> **Google Earth Engine enables users to:**
>
> - [ ] Design their own remote sensing data and infrastructure solutions.
> - [ ] Spend less time setting up infrastructure and more time on data science.
> - [ ] Secure their geo spatial data.
> - [ ] Create data pipelines.

#### Quiz 2.

> [!important]
> **The Earth Engine Data Catalog includes which of the following data types?**
>
> - [ ] Socioeconomic
> - [ ] Air quality
> - [ ] Imagery & Radar
> - [ ] All of the Above

#### Quiz 3.

> [!important]
> **How does Google Earth Engine improve the speed of computation?**
>
> - [ ] Google Earth Engine features better compute instances.
> - [ ] There are more maps available.
> - [ ] Google Earth Engine analyzes the data.
> - [ ] Map tiles are pre-tiled.

#### Quiz 4.

> [!important]
> **Which of the following is not a main component of Google Earth Engine?**
>
> - [ ] Data Catalog
> - [ ] Data Processor
> - [ ] Collaborative Ecosystem
> - [ ] Computation Platform

#### Quiz 5.

> [!important]
> **What is a benefit of using Google Earth Engine for imagery with large amounts of cloud cover?**
>
> - [ ] Google Earth Engine can read through the cloud cover.
> - [ ] Google Earth Engine provides metadata on the cloud cover.
> - [ ] Google Earth Engine identifies the different types of clouds.
> - [ ] Imagery can be compressed into a cloud free mosaic.

## Use Google Earth Engine to Distill Meaningful Insights

This module shows how to use Googe Earth Engine, at a high level, including using the code editor, creating composites, filtering and masking, and time series analysis.

### Video - [Demo: Using the code editor to create a standard composite](https://www.cloudskillsboost.google/course_templates/518/video/369040)

- [YouTube: Demo: Using the code editor to create a standard composite](https://www.youtube.com/watch?v=886SIOZ35zw)

I wanted to show you. Okay. Showing you a couple of examples now, but I want to kind of show you the code editor and then what this looks like. So I've got a couple of demos here. The first one, again, this is the website that you'll come to and you have your scripts, your various scripts. You have assets which is data that you have uploaded and stored by a GCP project. So everything's stored, you know, by Google Cloud Platform project. And then we have documentation. So if you forget it, for instance, oh yeah, what does an and filter have to be? We have the documentation built right into this, into this code editor. Now this is a just in time compiler environment. So I'm getting all these red things that are saying, Hey Sean, this script is not going to work because certain things aren't defined. But what I want to point out is this is the majority of the logic, these couple of lines of code for what I'm going to show you, What I'm going to show you is how to take an object, a Landsat seven collection. So all the images of Landsat seven ever and I'm going to I'm going to create a composite for a particular state. So the first thing I need is Landsat seven. So I'll search for Landsat seven up here. This can be used. It's a universal search box. I can search for locations or I can also search for datasets. And I have a number of different Landsat seven options. Each one of these sources has various different products, different tiers of refinement, and then the USGS just reprocessed collection two, which means that there's an upgraded version of this, not this library available for any one of these data sets. I can open up the metadata for those of you who geek out on metadata, and I've got all the image properties which basically tells me all the different bands, what type of fields I'm looking at. And this is not Google Earth where it's just the visualization. This is the full multispectral product. So we're talking about, you know, dozens or potentially hundreds of bands in the hyperspectral space. When you start looking at data sets like neon from the National Science Foundation and I'm able to bring all this data set in. And again, Landsat collection seven, it's a single line of code, so I'm going to import this. And now I have this object called image collection, which is all of Landsat seven. Now that's more than I need to create a composite of a particular state. But to get a state, I'm going to grab something from the U.S. Census called Tiger, and I'm going to grab the states and bring that in. This is basically census data. So we have these pre-defined geographies and somebody quickly put a state, a U.S. state in the chat and we'll or we'll use that as the as the region of interest. And if nobody does, I'll pick one myself. All right. Well, you had to pick Alaska. Now I'm I'm going to do Ohio just because Alaska has issues with the polar region. Okay. So Ohio. All right. So what I'm saying is I want to filter that state collection to Ohio, and then I'm going to filter the data. So I'm going to look for all the images between January 1st and March 30th. So this is going to be wintery in Ohio, and I'm just going to do a median. So remember when I showed you that big stack of images and I was looking for, you know, the median pixel value against all the stacks. So I would expect in the winter I'm going to have a lot of things like snow and clouds in this image. And then I'm going to clip it to the state. So when I run this now, you'll see very, very quickly I've got my clipped mosaic of Ohio and it doesn't look great. Landsat seven has got some sensor issues, but it's also a pretty small aperture in terms of time. If I open this up to the end of October, I can do that exact same thing again. And now I would expect I got more images for more pixels to be in that median. So what I'm getting now is a clearer picture of Ohio. And if I take the winter months out, I can probably even get this a little bit nicer looking. But I think you get the idea right. Nothing has to be downloaded. I'm able to just create these composites, which if you worked with geospatial data before and you haven't used Earth Engine, there should be somewhat revealing for you.

### Video - [Demo: Mapping algorithms over a collection](https://www.cloudskillsboost.google/course_templates/518/video/369041)

- [YouTube: Demo: Mapping algorithms over a collection](https://www.youtube.com/watch?v=WaowWuXycBA)

So that's the basic median composite. But I mentioned the ability to map more complicated algorithms over the collection. So this one, I won't spend as much time on the code. Just know that I have a function here called Masque Sentinel Two Clouds, and that looks at the quality band of Sentinel two, and that allows me to mask based on the clouds themselves. So for each image, I don't do this client side, but on the server side I say for each image, do something and it's going to go look. It's going to filter out the cloudy images and then when there is still a cloud in there, it's going to actually mask them. And that allows me to create a really, really nice cloud free mosaic using Sentinel two.

### Video - [Demo: Using a time series analysis](https://www.cloudskillsboost.google/course_templates/518/video/369042)

- [YouTube: Demo: Using a time series analysis](https://www.youtube.com/watch?v=UuDukZnB_wE)

Again, it's not just about visualization. This demo is going to look at creating a series of time series analysis. In this particular instance, I'm looking in Iowa and I'm using a data source called Soil Moisture or SAP from NASA. And so what this field is doing is is taking this bounding box and it's asking us to look at this soil moisture and product, and it should be generating a graph for us. There we go, generating a graph of soil moisture over time based on the time series. So this is the reduction phase. I've mapped this algorithm and now I'm saying, great, now we have this stack of multiple soil moisture readings for this entire area. Give me a geometry in this case this, this rectangle, and then chart the soil moisture so I can actually see what that value is. So we have a, you know, a wet season here and then the soil moisture goes down, you know, going into the summer. So that's what's really, really valuable, is being able to pull that data out and generate that time series in the water space. I just look at this example. We can take a look at Sentinel two imagery for harmful algal blooms. So these are these are algal blooms that are problematic in Florida and a lot of parts of the world where upstream you have fertilizers and other other contributing to the water source that take a what should be a nice clear lake and result in a horrible bloom of algae, which is dangerous for humans, it's dangerous for livestock and I can look and filter and basically look at the RGV image and I may not be able to see all that much right just in the visual space. But if I do a chlorophyl index, I can actually detect that there is a bloom of algae in here. The water should be blue, it shouldn't be green or red in this in this particular industry. We want to see that on the ground, not in the water. Okay, so I can do that. But how do I then make that into intelligence? How do I run that and help that power dashboard? But a quick little video here of what that looks like, where I'm going to use Sentinel two. Again, same imagery source and I may not get a complete image, you know, every day, but with about five day revisit with Sentinel two in middle latitudes I might get something right And they have ground controls here in the lake that we can use to to do some correction and make sure that we're getting accurate readings and and do some ground control with the actual the value that we're getting from space compared to what they're seeing in the lake. But we can also just draw arbitrary polygons. And so every time that I get just a little bit of data from the satellite, this is like information that the world is telling us, right? That's what these sensors were built for. And I could set warnings. I could kick off a pub sub topic and I could start to set these thresholds. And that every time I monitor this area, I'm getting the signal that otherwise is being lost. Right? So this is our opportunity to listen to the planet, watch the planet, and turn this into actionable data.

### Quiz - [Quiz: Use Google Earth Engine to Distill Meaningful Insights](https://www.cloudskillsboost.google/course_templates/518/quizzes/369043)

#### Quiz 1.

> [!important]
> **Using a chlorophyll index can enable you to detect what?**
>
> - [ ] Algae levels in water
> - [ ] Element composition
> - [ ] Cloud type
> - [ ] Soil moisture

#### Quiz 2.

> [!important]
> **What code editor function lets you create a cloud-free mosaic?**
>
> - [ ] MaskClouds
> - [ ] CloudBitMask
> - [ ] CirrusBitMask
> - [ ] maskS2Clouds

#### Quiz 3.

> [!important]
> **In the Google Earth Engine code editor, what can you adjust to enhance a composite's image quality?**
>
> - [ ] The clip, to specify the correct state.
> - [ ] The region filter, to gather more information on the specific region.
> - [ ] The median, which creates an average.
> - [ ] The date filter, to gather more imagery and pixel data.

#### Quiz 4.

> [!important]
> **You must analyze soil moisture over time, not just during a single season. What can you use to accomplish this in Google Earth Engine?**
>
> - [ ] A time series
> - [ ] A time chart
> - [ ] A span
> - [ ] A geospatial map

## Features, Integrations, and Commercial Use

This module explores recently added Earth Engine Features, and describes Earth Engine Integration and common commercial use cases.

### Video - [Geometry Drawing and Dynamic World](https://www.cloudskillsboost.google/course_templates/518/video/369044)

- [YouTube: Geometry Drawing and Dynamic World](https://www.youtube.com/watch?v=6iy-oCl_GuY)

We also have drastically improved our vector. Drawing vector was always kind of meant as a additional layer that we could use for, you know, the reduction phase. But a lot of our users are like, Oh, this is cool. I want to put really big datasets into waiting for the data to become painted essentially onto the scene. And so we've upgraded that significantly using a technology that allows us to apologize to the vectors much faster. And so now we'll go the same area, turn on the new labeling, and we can do all these dynamic styling. So it's much more common modern web GIs in terms of being able to do faster vector rendering. So that's a nice improvement. The other really, really cool project, one of our scientists, Chris Brown, has been working with WRI and National Geographic on a project called Dynamic World, and we are in the minor edits phase right now of this of this project. And what this is, is, you know, in the United States we were very data rich. We have a a product called an LCD or national land cover dataset, which is a 30 meter project product that's generated by DOI and USDA that looks at the land class. You know, is this urban? Is this. Is this forestry? Is this agriculture? The rest of the world doesn't have that necessarily. So the project is to be able to create a ten meter. So even higher resolution, a dataset of land classes, which is very, very useful to look over time. Where is the city expanding, you know, how are the mangroves being impacted, etc.. And we're doing this leveraging machine learning special neural net that's been developed to be able to paint the paint this classification onto the world. So WRI helped out, they developed the taxonomy about nine classes so somebody might, you know, kind of sniff their nose and be going, oh, just nine classes because, yeah, we're not breaking down, you know, this is a parking lot versus a street, etc.. But we are looking at the general, you know, this is built up areas, crops, trees, etc.. And the important thing to keep in mind is that most of those products in in the space are just the top one. So for each area that you look at, you'll get one classification. What we're providing here is a catalog of one for one images for every sentinel to scene that gets collected. We'll show you the top one. Sure. Meaning we're most confident that it's this particular class, but we're actually providing the probabilities for all of the classes. So this is a product, but it's also kind of the foundation for you to build your own models, right? So take those probabilities and build your own models off of the values that are coming here. As if there were almost synthetic bands in an imagery. So what that allows you to do this and create these, you know, derivative mosaics and also look at the time series because the product is called dynamic world, right? When you look at some of these classes, they might change. A good example of that in the Northeast and here in up there in Boston, if you take one spot and you want to know what is that? Well, it's sometimes water and it's sometimes ice. Right. So what we're providing here, you get the full time series right? Because you can look at that region, you can say, oh, I see this is ice for two months out of the year or three months out of the year. And the rest of the time it's a normal lake. So that could be very, very useful. You can also look at things like the hill shade to understand how, you know, it might not look right at first if you just looked at this and say, why is this forest interrupted? You said, Oh, because there's a power line cut that's been put in there for for high voltage transmission lines. And because it's not just a single product, you can use that time series. Remember what I did with Ohio for, you know, the winter and then the summer. So I can create different mosaics to look at different periods of the year or look at the entire year at once to understand the probability of land class for for a particular region that could be very useful. I mentioned the change, right. So what this graphic is showing, we looked at the top eight census statistical areas where people are moving in the United States. And so this one is down near Myrtle Beach in South Carolina. And what I wanted to look at was the difference, because we're doing this for the we've gone back to 2015 with Sentinel two, and we'll continue to use for every single central to image that we get as long as it's less than 30% cloud cover. And what that allows you to do is diff write a diff on the world in terms of these classes. A better way to maybe look at this. This is taking advantage of of BigQuery where we've brought in we've sampled the data from Earth engine. We've brought it into into BigQuery GIs, which has these spatial spatial functions and we did a DB scan to cluster this to look at the areas of most change. And so if you focus in down here, this is being powered by BigQuery through a partner called Cardo to push a, a geo JSON essentially into deck AGL, which is sitting on top of Google Maps. What that allows to do is just have a nice, you know, 3D environment where I'm using Google Maps, but I'm able to zoom in on these areas that show the biggest changes between 2015 and 2017 and then 2018 to 2022. And just knowing anecdotally, I've got friends from from up here in New Jersey that have relocated down to Southport, South Carolina, and that's what you're seeing. You're seeing areas that have, you know, popped up in the last couple of years being represented here in this visualization. Okay. If you're interested in dynamic world, you can go take a look at the site. You can play around with it. It is published, although we are waiting on the actual miner publication to make the full paper paper available. But we're really, really close. And you can use this as an asset. You can be added to be able to use this as an asset in in Earth engine today.

### Video - [Earth Engine for commercial use](https://www.cloudskillsboost.google/course_templates/518/video/369045)

- [YouTube: Earth Engine for commercial use](https://www.youtube.com/watch?v=iP777U6htyg)

Final thing I want to talk about is the Earth Engine commercials. So Earth Engine has been a platform again for over a decade, and it is free for academic research purposes, and it will remain free for academic research purposes. And it will remain free for all research purposes, including in the public sector. And but we really, really are excited about this because Earth Engine is now evolving into a full part of Google Cloud platform. Google is, if you're not aware, dead serious about sustainability and our carbon footprint and Earth engine has just been such an amazing technology that we want people in the commercial space. If you're a CPG and worried about sustainable supply chain or if you're a public sector agency with a remit of forestry or water or agriculture, we want you to be able to leverage this with an enterprise agreement with an SLA behind it and support. So we will have a commercial version of it with all those terms we currently have. If you go to Earth engine dot com slash commercial or earth engine dot Google dot com slash commercial. You can say, Hey, I'm interested in learning a bit more about this and then we'll we'll follow up with you. And I mentioned the research being free and that's true even in the public sector. And we're going to you know, it's always been kind of open, but people are signing up with a Gmail account and they're using it at work. So we're trying to clean that process up, make sure everything's aboveboard. And we're looking to do institution institution grants. So come to us and say, Hey, I work at so-and-so agency and I have this research project that I want to do. Can I use our engine for it? And we'll review it and say, sure, here's institution grants for you to be able to do that. So we would separate that out from your other enterprise. Use it with a separate billing account in the project. And we really do mean research. We're finalizing what this actually should look like. But in general, if you're writing a paper, if you're doing a novel algorithm that you're trying to publish, great, go ahead and use Earth Engine for that. It's not meant to say I want to, you know, use that all this free compute generate a product that my agency is responsible for, for developing, and then I'm gonna make that available for free. Like, that's kind of taking advantage of our of our goodwill here. So it really is supposed to be for academic research purposes where we want you to continue to develop that science that we know will benefit public sector agencies and the world downstream.

### Video - [Integrations and commercial benefits](https://www.cloudskillsboost.google/course_templates/518/video/369046)

- [YouTube: Integrations and commercial benefits](https://www.youtube.com/watch?v=y3GzUwgFM1M)

GCP integration. So Earth Engine is going to be a core service, just like BigQuery. It currently is. It's in preview. We will be GA very shortly this year, which means that we take advantage of identity and access. Who can come in and use our engine in your environment, You know, who has access to run jobs and create assets or delete assets, etc.. Also give you dedicated compute so we can segment your compute from the researchers and the general pool of Earth engine users so that you can control how much you use, you can set quotas on how much is consumed, etc. We take advantage of Google cloud storage and multiple is sometimes you want to export a lot of data to put it into Azeri or to put it into some other application so you can export to Google Cloud storage. You also can use cloud storage to host what's called cloud optimized gotif files, which is an open standard for for imagery that you can put into a cloud storage bucket. And then Earth Engine can do all that cool analysis against it as if it was a native asset. And finally, we have connections to Google Cloud Platform, soon to be Vertex Connector as well, which allows you to do those types of training models using machine learning like I showed you with Dynamic World through your own classification. So think of Earth Engine from here on out as a core Google Cloud platform service and as a commercial user. If you have a time sensitive mission, you're in fighting forest fires or your public health worried about algal blooms. You don't want to be sitting behind geography one on one at a university with, you know, 20 students hammering away on the system. You want to have some predictable compute with an SLA, so we'll give you the flexibility to do that. You can reserve, just like if you're familiar with big query reservations, where you can reserve slots, the same thing can be done with with Earth Engine. So you always know that that computes available for you. And when you run a task, when new imagery becomes available, like I was showing you with Florida, it can instantly run priority for you. And then also, you know, they'll be technical support and help to actually get your projects off the ground as well.

### Quiz - [Quiz: Features, Integrations, and Commercial Use](https://www.cloudskillsboost.google/course_templates/518/quizzes/369047)

#### Quiz 1.

> [!important]
> **What is a benefit of using Google Earth Engine for research purposes in the Public Sector?**
>
> - [ ] Google Earth Engine was designed for the Public Sector.
> - [ ] Products can be generated and distributed for free.
> - [ ] Earth Engine is free for all research purposes.
> - [ ] Earth Engine is available at a discounted price.

#### Quiz 2.

> [!important]
> **How long does it take for an image to go from a satellite to Earth Engine?**
>
> - [ ] 20 hours
> - [ ] 12 hours
> - [ ] 48 hours
> - [ ] 8 hours

#### Quiz 3.

> [!important]
> **Google Earth Engine integrates with which product?**
>
> - [ ] Vertex AI
> - [ ] Document AI
> - [ ] Cloud SQL
> - [ ] Dataflow

#### Quiz 4.

> [!important]
> **At what resolution is Dynamic World available?**
>
> - [ ] 100 Meters
> - [ ] 1 Meter
> - [ ] 10 Meters
> - [ ] 30 Meters

## Course Resources

Student PDF links to all modules

### Video - [Additional resources](https://www.cloudskillsboost.google/course_templates/518/video/369048)

- [YouTube: Additional resources](https://www.youtube.com/watch?v=xI-gfq4807s)

Some resources. There's a great self-paced training that we offer allows you to go in and get your hands dirty with Earth engine, learn how to use it. We think our documentation is pretty good. Any product can always continue to get better, but it is pretty exhaustive since it's been around for so long. And then again, if you have interest in using this commercially, we have a sign up form that John's posted in here.

### Document - [Student slides](https://www.cloudskillsboost.google/course_templates/518/documents/369049)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
