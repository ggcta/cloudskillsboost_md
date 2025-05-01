---
id: 568
name: 'Google Security Operations - SOAR Developer'
type: Course
url: https://www.cloudskillsboost.google/course_templates/568
date_published: 2024-05-07
topics:
  - SOAR
  - Orchestration
  - Chronicle SOAR
---

# [Google Security Operations - SOAR Developer](https://www.cloudskillsboost.google/course_templates/568)

**Description:**

This course helps developers customize Chronicle and augment its abilities with third party integrations.

**Objectives:**

* Develop new interfaces using the SDK
* Create actions, jobs, and connectors

## Introduction

This module will provide a short introduction to Chronicle SOAR Developer

### Video - [Introduction and Framework](https://www.cloudskillsboost.google/course_templates/568/video/472949)

* [YouTube: Introduction and Framework](https://www.youtube.com/watch?v=Z4sIrqA13tU)

hi and welcome to the chronicle soar developer course in this course we will learn how to develop new Integrations in chronicle soar by using its built-in IDE and utilizing the SDK this course consists of the following topics development environments Chronicle soar IDE and SDK the integration framework and the background on a technical level of these components after we've covered these topics we should be ready to start diving into the creation of actions jobs and connectors in chronicle soar let's get started first we need to understand what an integration is in chronicle soar to do that we can go to the integration settings this is located in the marketplace let's take a look at one of our Integrations such as active directory if you click the details button we can see more information about this particular integration here we can see the integration details we were looking for for an integration like active directory we can see that it has multiple actions and managers we'll review the difference between actions and managers later in this video but for now let's take a look at another integration I've selected qradar which is a Sim product we can see the actions jobs managers as well as the connectors this integration includes these are the four types of integration components that we can manage in chronicle soar an integration can be viewed as a self-sustained bundle of objects including any number of actions jobs connectors and managers Additionally you can provide configuration details and credentials as well as other properties of the integration like we see here when you create or install an integration in chronicle soar a python virtual environment is created for that integration if you're referencing any third-party Library within the code it will be included with the integration as part of the integration bundle now this is something that's not presented here in the integration details but will be detailed later in the series as we dive further into the development of Integrations as an example let's take a look at the tools integration and the files that are exported out of Chronicle soar here's a brief look at what the directory structure looks like and the files it contains returning to the integration let's look at what actions we have available now if we export this integration we can see that we have a folder for Action definitions which is the metadata for the actions what properties they have parameters what integration it is related to and so on we then have action scripts which are the actual python code for each action we have our dependencies which are all of the third-party python dependencies which are usually WHL files that we see here or really anything that could be installed using a pip command or any python file that you can use as a reference directly we then have managers these are the python files that are managed through the chronicle soar platform we will detail these later in the UI in addition to these we have the integration definition file which is the metadata about the integration itself including what version of python we are going to use what properties are defined on the integration level and could be shared between actions and jobs and what descriptions we have for that integration Etc in this example we don't see connectors and jobs as there aren't any for this particular integration the structure will look similar to the action structure job definitions job scripts connector definitions and connector scripts for the same purposes at the server level we have the following structure if we first go to the SDK folder which is located here you will see the python files that our SDK is comprised of these are the actions between all Integrations these SDK modules can be referenced when writing actions jobs connectors as well as managers and we will detail these later in the course for example we have our simplify dot Pi file here this is the most basic Chronicles or SDK function which is the wrapper for our API and we inherit the chronicle soar actions and jobs from it based on the type of action manager or job that you are writing you are going to use the appropriate SDK object seen in this list of files additionally we have the integration virtual environment folder here which consists of all of the installed Integrations we have in chronicle soar right now in this case we have many Integrations installed you can see from the folder names that each integration also has a version associated with it if you have multiple connectors that are already running in your environment you may retain older versions of the virtual environment to sustain these connectors until you decide to upgrade them each of these virtual environments holds dependencies that were installed with that specific integration if we look at the Active Directory integration we can open this folder and see the WHL files that were installed with this integration if you recall from earlier in the video These are part of the dependencies that we had originally installed it's very important to remember that different virtual environments are isolated and have no access to the resources of other virtual environments so if you import something or if you have a dependency available in one of the virtual environments you cannot access it from a different environment you have to duplicate it and recreate it in the same environment this concludes our intro and general framework topic thank you and we'll see you in the next video

## Chronicle SOAR Developer

This module helps developers customize Chronicle and augment its abilities with third party integrations.

### Video - [MyNewIntegration and Dummy Action](https://www.cloudskillsboost.google/course_templates/568/video/472950)

* [YouTube: MyNewIntegration and Dummy Action](https://www.youtube.com/watch?v=QuOS8kIHIHg)

hi and welcome back in this session we're going to take a look at the chronicle soar IDE we can access the IDE with this button here on the left side we see a list of all of the installed Integrations we have in chronicle soar for each one of these we will have a virtual environment on the server itself now we see both the official integration and custom Integrations available custom Integrations are identified by the gear icon this gear will also be used to configure the integration and manage some properties that we can use later down the road here's an example of the configuration we can manage here we can select the python version We would like to use either 3.7 or 2.7 we then have a short description that will be presented in the marketplace followed by the SVG icon and image uploads one for playbooks and one for the marketplace integration Banner we can also provide a list of categories which are essentially tags used for filtering Integrations available in the marketplace next we can see and import the python dependencies that we require in the integration code these are pip installable dependencies finally we have a list of the parameters we can use in the integration itself typically to configure connectivity and authentication for the integration these are all shared across our integration code such as actions jobs connectors and managers to begin our journey we will start by creating a new integration let's go over to the plus sign and choose integration we'll give it a name such as my new integration and click the blue create button now our integration is added to the list we'll scroll down and configure it giving it a description and noting the python version we can also upload an image give it a category and then add our dependencies we have two ways to add dependencies we can either click the plus sign to the right of the script dependencies and add a WHL file or python file or we can choose a library from the public internet if access is available as an example we can add the requests library and Chronicle soar will pull the library using pip and add these to the integration it's the same as downloading all dependencies yourself and adding them one by one the next thing we have here are parameters these are the main parameters to make the integration operate for example URLs logins passwords Etc let's click the plus sign and create a new parameter we'll give it a name and a description for type we'll choose string save the parameter and click on the save button for the integration once you click save a new virtual environment will be created and updated with the latest information we have on the back end of the server which we'll take a look now through an SSH terminal after listing the folders we'll now see our integration is here now that we have an integration let's create some objects inside this integration to do that we will do the same thing as we did for creating an integration we'll click the plus sign on the top left this will display all other items we can create in chronicle soar we can create a connector an action a job and a manager if you recall these are the same integration components we saw in the qradar integration as optional integration components that could be installed with an integration these are Python scripts that are managed in the IDE alongside all of the dependencies that could be added to the level of the integration itself we'll Begin by creating an action we'll give it a name and choose the integration you want to add it to we will select my new integration and click create by default Chronicle soar provides an actionscript template for us this template will not run on its own but it does include the necessary components of the action that you may want to consider incorporating into your code to keep it simple we will review these components and then we will remove what we don't need for our first action here we have our SDK objects an action requires us to import the chronicle soar action Library this inherits the chronicle sore objects we need to communicate back and forth with the chronicle Source server we use these objects to obtain the alerts information action parameters to return Json results and any action results back to Chronicle soar next we have the chronicle soar utils this is essentially a common Library we use in chronicle soar it has multiple functions that may be useful when writing your code in addition we have script result which is an object Chronicle sore returns to the server it usually contains Json results or tables that you might want to present to the end user action results attachments and other similar complex objects you do not have to import it specifically but it does provide in this example flags that you can return in your action to indicate the state of the action our code could be completed successfully it could be a failure or a timeout later on in this course we will see that we can also return a flag that says that the action is in progress next we have our constants to help keep your code organized Chronicle soar provides commented sections in this template we have the integration name which we will match with the integration name we are developing for in other words my new integration this is useful to help Define the location of the integration logs and to retrieve configurations previously we created a new parameter here called parameter one and we would now like to retrieve it we can use the integration name to do that also we have a script name which is mainly for logging purposes if you want to have logs for this action then you need to let the SDK know the name of the action so that it can put the logs in the correct folder moving on the output Handler wrapper below is to help with our debugging process while this is not a required component this will help to put all the logs that you create throughout the action in the debug output window which we'll see later in chronicle soar we create a main function and input our code into it you don't have to do it this way but this is our best practice and the template that we would recommend every action requires a Chronicle sore action object to execute correctly this object provides access to the Chronicles or SDK and will be used for everything you do within your integration it will be used to retrieve parameters send back results and interact with the chronicle soar platform if we take a look at line 12 of our template we can see the script name again this is used for logging everything to a specific folder if you do not provide this information then the logger will most likely fail letting you know that there is no logging folder to work with now that we have that in place the next line is used to write your first line to the log we have a logger object assigned to Chronicle soar you can use this object to invoke the inform worn error or the exception methods each of these will be useful as you're building your Integrations on the simplified platform and for debugging your Python scripts the next section beginning on line 15 we find the configuration extraction one option is to use the extract configuration param method we provide the integration name and the param name that we are looking for in this case it would be my new integration and the parameter name of parameter 1. this is case sensitive so make sure you write it correctly the output of this function would be the parameter value itself in this case the value is empty but if we put something here like test Val for example and save it the output would be test file the default value we just set and param a would contain the value of this parameter if you don't put any other properties in the method like default value and input type then the default value will be a string but if you let it know that it's a Boolean for example it will attempt to cast it for you in this case it's obviously a string and we'll leave it that way for our integration but in other types of parameters you may want to specify the data type optionally you can also do it yourself and don't have to use this function in addition you don't have to use the extract configuration param method if you don't want to use a wrapper to the process of extracting a property you can directly access the objects using the get configuration method this is a wrapper to our API that accepts an integration name and returns a dictionary of all of the properties that we have in our integration in this case we only have one property so the result would be a dictionary with one key value pair param a could be the result of this method where we access a specific key parameter one please note that if you choose to do it this way it's your responsibility to make sure that this case sensitive key exists already you'll also need to make sure that it's in the correct format in order for this to work it's up to you to set up the input checks in this scenario the next section would be the same as above but instead of a configuration of the whole integration it's going to be a configuration for the action itself in this case the action has no parameters yet what we will do is add the first parameter here to do this we'll go to the right side of the screen and click the plus sign we'll call it action parameter 1 and input a description we'll set the data type for this parameter to be a string and give it a default value we now have a new parameter here that we can access and be mindful that this one is case sensitive as well we'll copy this here and put the value here as well the extract action param method is pretty much the same as the extract configuration param method however while this method accesses the action parameters and not the integration configuration it essentially has the same properties therefore you simply Define the parameter name whether or not you want to print it to the logs if it is mandatory or not and while the example doesn't show it you can also input the data type the next line here is a logging message we'll use this to separate the parameter initialization from the actual logic this is a best practice to help keep our code organized below that we have a start to our logic we first initialize all the properties we're expecting to return to Chronicle soar we have our status with a predefined state of completed before we continue with the logic I'd like to discuss the result of the action we ran python code in this try accept then we logged all of the results that we found and a few additional items before we exit the action finally we reach the chronicle soar end function this is like a return function in Python this method takes the results we gathered this is an output message result value and status and sends it back to the chronicle Source server this method lets Chronicle soar know whether or not this action was completed successfully failed if it is in a Timeout state or what we will see later if it's in progress and should be run again the output message would be a result that is presented on the action result for the analyst the result value would be a value that is returned to the playbook for Automation and this is essentially the return value of the entire action our job in the action itself would be to perform our action logic and then make sure that these properties in the end method are properly set now let's see what we have in the main Logic for the action by looking at line 21 of our code it's recommended to encapsulate your logic with the try and accept statements and deal with your errors in this case if we have an error We'll add the error to the logs for further analysis and we'll set the state to failure to let Chronicle soar know the action has indeed failed optionally you can also simply raise an error and it will fail the action for you even if you didn't call the chronicle soar end method however it is recommended to use the flag to fail the chronicle soar action because it will allow you to gracefully control the response within your action the output message is then yours to modify and you can specify what you want to be returned as well as the result value now for the logic Chronicle soar has two different types of actions actions that run once and actions that will Loop over a list of entities within the scope of the action in this second scenario the action script will iterate over entities and perform the logic we have defined in this example the difference is here here is whatever part of code you want to run once and then over here you will have a for Loop that iterates over Chronicle sore entities and then you can do whatever you want multiple times we will get into the target entities later down the road but for now we will remove it from the script as we don't need this functionality what we do now is write our code and make sure to fill in these three properties because these are the properties that we're going to return to Chronicle soar for example what we can do is very simple we can say that the return would be hello world and the result value would be Yes we made it the status would say that we finished completely and correctly so there are no issues with the action and that we're ready to return these two properties let's go ahead and save our code if we run this action we should be able to see the output message and result value to run this action we will first need to create an integration instance and then we will be able to run it however before we do that let's test our code to do this we'll go to the testing tab we'll choose a scope and the case to run it on then we will need to choose an integration instance since this is a new integration we created and we don't have an instance to find this list will be empty let's go ahead and quickly create a new integration instance and come back to the screen to test our code a quick note on the test case that you'll run the action script on you'll actually need to create a simulated case so that you can select this within the testing tab in the IDE ate to the marketplace from the top menu it may take a moment to load now type in the name of our integration my new integration and if you're unable to locate it simply click Integrations under settings navigate to the default environment and add your instance here after we've created the integration instance we can select it for our testing let's run it and see what we get we see that we do get the script result which is Yes we made it this is the result value in addition we also have an output message which is hello world and everything looks correct what we can do now is go to the debug output and see if there are any issues prints or errors what we see here is our logs only there are no issues or errors here thanks for watching and we'll see you in the next video

### Video - [Installing Dependencies](https://www.cloudskillsboost.google/course_templates/568/video/472951)

* [YouTube: Installing Dependencies](https://www.youtube.com/watch?v=n2lg_JpHs_s)

hi and welcome back in this video we're going to talk about integration dependencies so for this video we're going to use the air table integration to demonstrate the process of installing dependencies now we already have an airtable integration as uncertified Community integration meaning we can modify its configuration as well as its dependencies let's take a look and see how it is created and defined we'll begin with a demonstration of the search function for this integration We Begin by importing the simplify action here we do have a third-party dependency for airtable that we will have to fetch and we see here the parameters that we are going to use we need an API key a base ID which is a namespace and the table that we're going to retrieve we will use a different function so we don't need the rest of these these lines are how we are going to use airtable and retrieve the results please keep this in mind when we create our own integration let's now return to the action in our integration to begin we know that we have a new dependency we need to include to do that we will go to the integration definition and we are going to add a new integration dependency we write the name of the dependency in the same way you would when you try to download it through pip this would be a pip install air table pip downloads this library in the back end of Chronicle soar when we click the add button we have now downloaded the dependencies we need and if you look closely you will see that we have it here now when we click save it will install these dependencies in the virtual environment of our my new integration integration in addition we need to add a couple of new parameters so let's go ahead and do that this is going to be the API key and it's going to be an obfuscated password parameter so we don't see it when we open the integration page it should be the only parameter here we'll click save and let the chronicle Source server install our new dependencies this will take a moment to complete when we're done installing we can continue working on our new integration in The Next Step we're going to retrieve the actual property we created the API key from the integration credentials page first we need to provide the integration name when we go here to one of these options we have the integration name to let Chronicle soar know where to retrieve this information for now we will only use one and we'll give it a proper name remember this is case sensitive this property should be the API key for this action to work we also know that we need to supply the base ID of the namespace of the table and the table itself therefore We'll add two parameters quickly the base ID with the description and a default value and the table name with the same now let's add these new parameters to our code remember these values are case sensitive so make sure that you type them correctly or your parameters won't work let's now provide a default value for our output message and our result value let's continue with coding the rest of our new action we'll Begin by instantiating the object for the air table with its credentials so that we can use it later to retrieve information and get the data that we need for this we'll Supply the base ID table name and the API key parameters we'll then make an API call using the air table library to grab the data that we're looking for we'll see the data that's returned here shortly before moving on let's save our updated code we'll now need to input an API key for the service let's click on the Integrations Tab and open the settings for our original air table integration to inspect the settings search for the my new integration we're building and open the settings now we'll paste in our unique API key from airtable and click save we now have our API key available to our action the next thing would be to fill in our test parameters and then obtain the base ID and the table name for our test in the next video we'll continue working on our first action and testing the features that we've built thanks for watching and we'll see you in the next video

### Video - [Finishing First Action](https://www.cloudskillsboost.google/course_templates/568/video/472952)

* [YouTube: Finishing First Action](https://www.youtube.com/watch?v=PqHlrS0Jkco)

hi and welcome back now that we have everything set up let's run a test for the action we will first need to choose the scope of the entities we run it on in this action we don't use entities yet so this field doesn't really matter so in this case we can choose the all entities option then we choose a test case on which data we want to run it the easiest way to generate a test case is to simulate an existing alert from the case view in this example it doesn't matter which test case we choose from because we're not using the data from the alert itself how the integration instance is defined matters because we need to choose one that's properly configured which is something that we did in a previous video when everything is ready we'll click the Run button and we should see results the results are from the default and that's expected in the debug options section we have Json data that came in from the logger here we do get the information we expected and we will see that it's from the data table we had previously configured that means we can continue to our next step now we would like to make this log data appear in a more elegant way with that in mind we have the script result object in chronicle soar which is accessed through simplify action object and through that the results property here you have built-in actions that are used to demonstrate outputs we will start with the data table in this case we will use the add data table method to accomplish what we're trying to do we are going to use this method which retrieves a string as the title and a list as another parameter let's add it to our code and see what we can do with it we'll adjust the sample parameters before we continue giving it a custom title and a list of test objects we're simulating a CSV file here each string represents a line in the list and is separated with a comma to represent different columns as you'd find in a CSV if you click run and return to the testing tab you will see that we have another output titled this is my title if you open it you will see our new table here we have three rows one of them is the column with headers and the rest are their values we'll use the same thing to demonstrate a table output from airtable now to save time we'll use pre-built code for this particular demonstration these two functions are used to obtain a list of Json objects or a list of dictionaries and create them in the CSV formats to be used with the data table function essentially we're going to take the Json and format it into the same format that we expect in the data table function which represents a list of convertible strings let's comment out our previous test and add another line here we're going to supply a title again and this is going to be table contents the rest is going to be the end result of the construct CSV function this function accepts a Json list and converts it into something that's usable with the data table function let's run our code and see what we get we can see from our debug output that we're missing a required Library let's add that in and rerun our code we now see the table we were looking for however you'll notice that we have something that's not really readable the result of the table is actually in fields therefore we need one more step to fix that issue let's adjust our code to print the list out properly this looks much better if you want to retain metadata like when this field was created and information about its ID then we can do something else here and not just extract the fields however this is the easiest way to only show the contents of the table in addition to the data table we have other objects we can use the next thing we would like to do here is to get the whole Json as an output as a result of the action we're running the data table is a UI widget that is only available in the case wall if you want this information to be available for use within a Playbook as you're developing your own automation then you'll need to call the add result Json method from our simplify result SDK to make it available this method accepts just Json data and assigns it to the Playbook as we expected so we can put results as a parameter and we'll see what we get as an output if you look at the results you will see that we have another object here this is the Json result which contains all of the elements from our table it's also a part of our response object in chronicle soar for the action results you will see the technical details the final step is to construct an appropriate output message before we finish the action and assign a real result value in this case the result value will be the number of rows that were found this is also an object that can be used in our Playbook let's quickly write the code for this we'll write a result value and then our output message and now let's run our code excellent we found various results in a table named my first table and our action is complete this concludes our video on actions thanks for watching and we'll see you in the next video

### Video - [Iterating Entities and Enrichment](https://www.cloudskillsboost.google/course_templates/568/video/472953)

* [YouTube: Iterating Entities and Enrichment](https://www.youtube.com/watch?v=WS9oo1rCsKU)

hi and welcome back in this video we'll talk about iterating over entities and enriching entities to begin we've already prepared a duplicate of our previous action and made some adjustments we'll go over those changes here in a second here is our newly modified action the first thing that you may notice is a new property called column name for identifier first let's cover what we're doing here we're going to iterate over all entities in the action scope and try to determine if a given entity identifier exists in our air table in a column that we specify if we find it we're going to retrieve the same row and enrich it as data on the entity now in order to do that we've added a couple of entries to the air table and a column called identifier we've also put some entity identifiers in for later use the first two identifiers exist in the case we'll be using and the rest are here as an example the identifiers will correspond to our new parameter field here in addition python code has been added to our action that will be going over in more detail the initialization is the same we've added another parameter here and we'll be using it later in this video here's the important part when you want to iterate over entities you will need to use the simplified.target entities property this is a list of objects of the type domain entity in chronicle soar where each of them represents an entity in the action scope if you look at the testing tab you will notice that we have a scope field that allows us to choose from a variety of different types of entities within a given case to run this action on if you choose only external users for example Target entities would represent a list of all of the objects that represent external users and so on returning to our code we'll want to extract information from from that entity object and use it to run on our search we have a couple of the most used properties for this object first we have the entity.identifier then we have the entity.type commented out which could be a file hash file name address URL username as well as whether or not it's suspicious or not these are the most common three properties of the entity object we will use we also have an additional property in the entity which represents a dictionary that has the rest of the data about the entity this is what we call the enrichment we'll be using this line to extract The Entity identifier and then use it to search the air table for that specific identifier if we do find the identifier we're searching for in the table under that specific column we specified here we'll go ahead and perform the actual enrichment process we will access the additional properties object a dictionary of the entity properties and add more fields to it this is a flat dictionary which means it has no hierarchy just key values the word values represents simple objects in Python including strings integers and other similar data types we access it by extracting the first result from the search if we have more than one row this python code would need to be adjusted to work properly we could also look at ordering them by creation time modification time and take only the latest one depending on what we're trying to do within our action once we call the additional properties dot update method we enrich The Entity object on the local level of the Python script now we will need to push it back to Chronicle soar this is where we utilize the simplify dot update entities method this method receives a list of entity objects and transmits them back to Chronicle soar through our API optionally you can also send an entire list of entities even if you have not changed each individual entity object the API will update each accordingly ideally it's best to make sure that you have a defined list of only the entities you've modified this is a list of those entities in which we'll be sending over via the API the last thing we have to do here is the Json results the action has multiple outputs divided into two sections we have the output message tables files and so on this is something that's only accessible in the web UI we also have a second portion of it called the technical details and here we return the Json result value of the script result of the action that was executed these are primarily used in Playbook automation you need to make sure that they are properly formatted which is why we take some time to make sure that it's going to be in the format that's most compatible with our Expression Builder in chronicle soar therefore the first thing we will do is instantiate a new dictionary and make sure that each result we get from each entity is stored in this dictionary the key would be the entity identifier and the value would be whatever value we found this is the form format of our Json that's not easy to use with the Expression Builder and because of that we ran through a little bit of transformation here we can convert a dictionary to a Json result dictionary this is in our utils library here this function will transform the dictionary into a list of predefined keys which is a lot easier to access with the Expression Builder we'll soon see an example of this particular output next we need to make sure we set up the output message and the result value so that they're useful to us when we're running our code best practice is to put a very simple response here so it's very easily searchable with a condition in the playbook in this case we put the amount of entities that were found in the air table as a result in doing so we can quickly have a condition that says if this amount is zero then we perform a specific action otherwise if it's more than zero we may want to create an Insight or something to that effect ultimately it's up to you what you want to return here although keep in mind that it should be something that's fairly simple and straightforward the last thing you need to make sure that you do is to supply a Json example because it's a lot more difficult to work within the Expression Builder without any Json example available we'll go to the details Tab and turn on the include Json result toggle to let Chronicle soar know that it should expect the Json if you don't turn it on then you simply won't have it available in the Playbook as a placeholder we'll now import the Json file that represents the result our action should return okay let's quickly run our action and we'll see what it returns then we can continue with the data we'll need for the import as you can see we found entities that were defined previously in our air table navigating to the cases tab we will retrieve the Json that we're going to import to do so we will select the test case that has been referenced in our previous tests we will then perform a manual action on the case wall by first selecting the example action from my new integration once we fill out the required fields and execute this action we can export the Json file here heading back to the IDE we can now import our Json sample with the properties we enriched and save our code with a Json response connected to the example thanks for watching and we'll see you in the next video

### Video - [Async Actions](https://www.cloudskillsboost.google/course_templates/568/video/472954)

* [YouTube: Async Actions](https://www.youtube.com/watch?v=PWCVyuv25xI)

hi and welcome back in this video we're going to talk about asynchronous actions we've already learned the flags that an action returns to the chronicle Source server in order to let it know the status we've already reviewed the completed status which is the default we've also touched on a failed status which is when we raise an issue and we've also discussed the timeout status in this video we would like to introduce an in-progress status essentially the previous status methods told Chronicle soar that the action finished either successfully or with an error these statuses are used to either continue an execution stop the Playbook or Implement further remediation efforts when things don't go as planned now the last state flag lets Chronicle soar know that the action has finished an iteration but still has work to do essentially Chronicle sore will call this action again x amount of times every 30 seconds which is the default Trigger Time the action itself looks exactly the same we invoke the simplified dot end here because this is the end of the line and we let it know whether or not we are finished obviously we can have multiple options for the flag like the in progress flag that we have here or the ones we discussed earlier in this course it's up to you the developer of the action to make sure you don't inadvertently add an infinite Loop and that you have properly added an ending condition in your code regardless of what you do Chronicle soar has a timeout set in the configuration section of Your Action if you don't reach your end criteria after this amount of time the action will simply fail with a timeout we won't have to worry about that very much but it's still very important to have the stopping criteria because we don't want it to run our action for that long please also note that you will need to make sure that you have the flag constants available the flag is imported from the script result Library which provides access to the execution state in progress afterward you need to decide on your logic in this simple example we increase our count so that after every iteration we're going to have a different message presented via our debug output when it's finished it's going to say finished iterating after Etc when you do finish an iteration there is a way to send the information over to the next iteration this allows us to retain access to anything that we need if you have parameters a configuration entities scope and so on you can still access the data contained in these in addition to that we have a new implicit parameter defined on line 19. let's call it additional data now it's different from the action parameters we have defined here and it will be called differently the previous iteration data variable is the result value of the previous step in this case it's empty in the first iteration this is how we check whether or not we run the first time or not we must make sure that this object is not empty if it is empty we'll put this message here and output 1 which is the current duration and number to the result value of the script this is what you're sending to the Automation in the this case it's in the in progress State and this is what's going to be returned to us in the additional data so in this case we sent the current number of the iteration if it's not the first iteration then we increase this number by 1 and evaluate our stopping criteria if it's not over 10 our code will continue to do the same thing and output what iteration we're on we send the current iteration and continue if it's already met our limit then we have a different message that signals that we're done then the action finishes let's see how our code runs via the case view by running it as a manual action in chronicle soar with no Action Properties let's view the case wall to see the results of our first iteration remember Chronicle soar will call this action again in 30 seconds by default for the next iteration therefore we need to wait for roughly 30 seconds before we can refresh it and see the next iteration with the output that we specified in our output debugger when we refresh the case we can see a different message in Orange in another 30 seconds we should see the number three and so on until we reach 10. for our tutorial we already have it prepared so let's see how it looks at the end of the completed execution cycle in the end it looks something like this it finished iterating after X amount of iterations it's no longer orange but gray and it continues on with its execution if it's in a Playbook it will simply continue to The Next Step these are async actions now just a few remaining notes about asynchronous actions first it is impossible to check or test the actions in the IDE it is only the first iteration that would run in that case even if you set the status as in progress it will simply run once and will not run again in addition it is very strongly recommended to use the logs here because it's difficult to monitor what's going on with the execution of the action you won't know what the given inputs and outputs are for every iteration and it may change depending on the code you're writing if you are relying on enrichment from the entities for example it might change during execution and the logs would be the only way to determine the value shift thanks for watching and we'll see you in the next video

### Video - [Accessing Alert Information](https://www.cloudskillsboost.google/course_templates/568/video/472955)

* [YouTube: Accessing Alert Information](https://www.youtube.com/watch?v=vFWf2k6MWEk)

hi and welcome back in this short video we'll see how to access alert fields from an action in Python if you have an entity object you can access these properties much like the accessing of entity properties you can also do the same thing accessing the alerts information the simplify object has an object called current alert which is an object that represents the alert itself in chronicle soar it has its own properties as an identifier a list of events called security events and other additional properties what we'll do in this example is retrieve the first event we will then extract the information from the event into an entity we'll go to current alert and to index 0 in the events list then we extract the first event as a dictionary we lower case the keys of everything so it's a little bit easier to find the keys we want to enrich then we iterate over the entities to see whether or not the field exists if we find one of the fields that we want to enrich then we add it to the entity on line 33 we are running the update entities method and that's it please remember that we also have the representation for the alert itself including all entities if you go far enough you can also access the simplify case and see if it has a list of alerts available so the rest of our alerts are accessible as well it's recommended to explore these objects and if you would like to take a deeper look you can reference the simplified data model python file in the python SDK to see how this object is built thanks for watching and we'll see you in the next video

### Video - [Connectors](https://www.cloudskillsboost.google/course_templates/568/video/472956)

* [YouTube: Connectors](https://www.youtube.com/watch?v=aRQTOAboE_E)

hi and welcome back in this video we're going to talk about connectors if you recall we have three types of scripts in chronicle soar actions jobs and connectors actions can be triggered manually or within a Playbook connectors and jobs both run periodically you'll choose the amount of time you want to add between each iteration the underlying python code in your connector will get executed at this interval it's important to remember that you'll want to give your connector sufficient time to run through each iteration to ensure it doesn't fail to execute or trigger any rest API limits if you're integrating with one we'll Begin by creating a new connector to create a connector click the plus icon and choose the connector option here we'll give it a name and select the integration we want it to be located within we'll put this in our new integration as expected we see the default template here providing the structure we'll need to begin writing our connector in this template you have random alerts being created most of its logic creates the actual random alert but the core python code we need is here we will go through it quickly to see what Chronicle soar expects from the connector later on we'll see the actual connector and how it runs first we have the chronicle soar SDK objects in this case we'll call it simplify connector execution in the previous examples we saw it was simplify action so it's a slightly different model in this case this Library supports connectors and the ingestion of new alerts in addition we have a data model for connectors that we import from the Alert info objects it represents an alert in chronicle soar this object is what we utilize in this connector to create alerts in Chronicles or the rest are Handler functions we don't have to use them this is just part of the template example we have a section of constant properties from line 14 down that we will use later on specifically for this template exam sample then we dive straight into the main function however before we do that we see that the main has a parameter let's see where we obtain it in chronicle soar there are two modes of running the connector we have the test run and we have a real run the difference is that one is for developing and configuration testing and runs with a flag the other is an operational run and runs every x amount of time based on the interval you set however we don't have to use that we can call the same function without any flag but if we want to distinguish between a test connection or for debugging we can use the is test run flag as we want to do this our main function is called with that flag we instantiate the chronicle soar SDK objects here as usual in the first real line of our function the last line of coding in our script would be the return package which is essentially the same thing as the end method you would see in an action this method is like a return for any function and here we return the results for this iteration back to Chronicle soar in this case the return value would be a list of what we'll create a list of alert objects each item in the list is an alert info object that will be returned via the return package method the connector's purpose is to ensure that these objects are built correctly we'll ignore the login commands in the main function for now and move on to parameter extraction connector parameter extraction is handled in a similar way as extracting a parameter meter from an action it uses the same method here you can use the chronicle soar parameters instead it is the same as doing this again values here are case sensitive the difference is this one also does validation and tries to cast it for you if you don't want to use the function or don't understand it completely you can do it yourself simply grab the property make sure it exists cut it to whatever you need and go from there the main logic part here is to create the list of alerts if we see the result here we want to obtain a list of alerts with actual data and send them back to Chronicle soar we do it based on some logic in this case we iterate over random data and create alerts in some way if you apply this to your own code you may want to retrieve information from somewhere it could be an API call or something similar then we iterate all that over the results we found and apply that logic to it you may only be looking to ingest a portion of data instead of the entire result or you may want to parse it first and so on part of parsing is creating the Alert info objects which are separated into a different function here this is the most important function of the connector it builds the Alert info objects therefore we instantiate new objects and we fill them with the necessary properties what you see here is mandatory we have the display ID a unique identifier for this Alert in chronicle soar the same display ID cannot be used more than once if alerts have the same display ID the ingestion process will simply drop that second alert a ticket ID is an identifier for the alert that is also searchable on the search page in chronicle soar it does not have to be unique you can use it as a common identifier for multiple alerts it is best practice to ensure that you put a value in the ticket ID as it's how you will find alerts via the search feature in chronicle soar then we have the alert name which displays the value presented on the overview screen you have the rule generator which is called the alert type in chronicle soar and we also use it to assign automatic tags or assign playbooks for alerts we then have the start and end time which are the Unix timestamps in milliseconds of the alerts we're building make sure that this variable contains a value usually we will take the first event of the alerts as the start time and the last event as the end time If the product you're integrating with already has an alert or predetermined time step values you can always use those values instead it's up to you the priority of the alerts represents exactly that priority when adjusting an alert to an existing case this number will be added to the existing priority otherwise it would be created with that priority now we have priority values here on line 77 and need to put an INT for the value in chronicle soar we can see the name of each informative is negative one medium is 60 critical is 100. notice we have some other values commented out here next device vendor and device product are two other properties of the alert the device product is also used for triggering playbooks therefore it's more important than the vendor these are just a few properties that we expect the alert to have and will be displayed the next thing we have on alerts are events alerts have their own metadata but usually contain a list of at least one event as well events are applied to the Alert info object here and the events property this is a list of dictionaries without a hierarchy each event should have a flat dictionary key value pair where the value is simple and valuable in Python that's either a string integer or similar so no other dictionaries or lists are contained therein we'll need to ensure that our events are flat and don't contain a hierarchy if we have a hierarchy we'll need to either choose what to bring or make it flat somehow events don't support complex objects however Chronicle sword does support more than one event so you can have many events attached to a single Alert in our example we don't see that but we also have the alert extension property essentially a key value property attached to the alert itself it will look like this it's equal to a flat key value dictionary in a later example we'll see how this is built as a recap of what we've learned so far the connector is responsible for ingesting alerts into Chronicle soar the process would be to retrieve information from somewhere and then run through processing logic where we build alerts each alert contains some mandatory fields as we can see here in front of us each alert has one or more events in a list the events within our alerts are just flat dictionaries alright now let's move to an example prior to this video we set up an air table connector before we dive into the code we'll look at this air table and the information in it so we have context for when we're looking at our python script this is the table that I've created it has the following fields alert name alert type product name file hash username hostname address reporter and is read obviously it could be anything else you want so this is just an example we will create an alert for each row in this table consider a row to be an individual alert the data we'll be presenting is a key or the column name and the value would be whatever we have in the column on that row we're trying to ingest let's Dive In first we import the SDK and data model of the Alert info second we import whatever object we need from the air table from the third party dependency we use then we can move into our code we have the main function where we instantiate our new connector we instantiate an empty list for alerts which we will fill later as you can see it's already here on lines 83 to 86 we add alerts in our for Loop and then send them back to Chronicle soar on lines 58 to 66 we retrieve properties from the connector definition we have the API key base ID table name and other fields added for the logic of this connector we have an alert name field to populate the Alert info which we will see here in a second it's the same thing for the rule generator and product columns these will let the connector know where to put the values from the air table then we instantiate the air table object on line 72 so we can query the table and retrieve results it is important that we don't attempt to ingest the same row twice if you have a duplicate with the same display ID the first one will be ingested and the second one will not however this puts additional stress on the server which is against our best practices now we have a list of results on line 77 much like what we saw in the actions in a previous video we iterate through each one of them and for each row we create an alert once we finish iterating through all these records we return the package back to Chronicle soar that means we send those alerts to the chronicle Source server which then Begins the ingestion process the important part is that we're creating alerts based on these airtable results let's now review the generate alert from record function a ticket ID is assigned for this case so you can use the Chronicle Source search feature for the row to correlate events together for the start and end times we'll take that from the creation time of the record once the record is created we assume this is the creation time of the alerts if you have a field for that in your data you can also attempt to read and process it but make sure it uses the Unix time format there is no priority column in the air table we built so we'll manually assign it using a default value of 40. 40 is a low priority for every new alert processed in this function on line 43 it Returns the Alert info object we use that to directly populate another element in the list of alerts that we're going to send to Chronicle soar once we're finished with all the results we send it back let's save our code and see how it runs for this example we've already created the connector and pre-configured it however we have yet to run it let's run a test to see what we get we have three alerts in here populating correctly we have alert name product start time and end time time these were processed from our input properties alert name alert type and product name if we refer back to our air table we'll see that these are the columns alert name alert type and product name we can now open the results and see our data populated we have an event list and then alert information we also have our ticket ID which is the same as the record ID and display ID we have the alert name device product taken from the table and the start and end time calculated from the record also we have the extension property which is a flat dictionary in this case it's represented as a list of the dictionaries with a key value pair but on the alert itself they will look like simple key value pairs we then have the product name and file hash Fields everything we saw on the air table is here in the event itself we also have the raw data the extensions in the event are the same right now but it doesn't have to be that way we have the same values we saw in the air table so everything is here we can now click on the alert and load it to the chronicle Source system this will create it as a test case in chronicle soar now you can open the case and work with your data thanks for watching we'll see you in the next video

### Video - [Integrations - Jobs and Managers](https://www.cloudskillsboost.google/course_templates/568/video/472957)

* [YouTube: Integrations - Jobs and Managers](https://www.youtube.com/watch?v=l2sJpFGDtPY)

hi and welcome back the next Chronicle soar object we're going to talk about is jobs we can use jobs to synchronize data between Chronicle soar and an external system for example if you create a ticket in servicenow from a Chronicle soar Playbook you may want to keep some things synchronized between the servicenow ticket and the chronicle sore case to do that we would run a job that synchronizes all of the open cases that we have in chronicle soar with their respective service now tickets and vice versa when an analyst takes a look at the chronicle sore case they can see what happened in the servicenow ticket another use case for jobs is to run monitoring Chronicle soar comes with a handful of monitoring jobs already that can monitor the various aspects of the system starting from connectors and ingestion processes and ending with the playbook's actions we have an example of a job that we can review here jobs are handled like any other object in chronicle soar we first need to create an SDK object in this case that object is called simplified job we first instantiate it as we're doing with every other script at the bottom of our code on line 36 we will call the end script method this method behaves much like the end method in an action and the return package in connectors this method lets Chronicle soar know the job is completed in this case we don't have any parameters because the job doesn't have any outputs the job does something simple and writes logs the next import that we have here in our example is for airtable we're going to reset the is red flag from the table that we've created for the connectors before we begin we'll detail that later as we're testing our code we then instantiate the chronicle soar SDK object on line 11. set a script name for the logs start the log and get information from the parameters we need in the same manner as in the chronicle soar actions and connectors videos on lines 15 to 18 we retrieve the parameters properties remember remember the parameters are case sensitive so we'll need to make sure it makes the parameters we have here on the right it's not detailed in this video but a job can also access the configuration information from the marketplace like we've seen in previous videos via the get configuration method moving on we create an object for the table with the appropriate credentials then search for everything that's true and that the connector has already retrieved afterward one by one we change the column to false and reset whatever the connector did to those records this is mainly for testing in this example for a job the next object we're going to discuss is managers let's use Alien Vault as an example a manager is a python file that resides in the same folder as the scripts you are running if you run an action under a selected integration and if this integration has managers as well these managers are going to be present in the running folder and thus a accessible to the action itself in this example we're going to run the enrich entities action for Alien Vault if you look closely on line 7 you will see we have an import for a specific file this file is called Alien Vault TI manager and it has the exact same name we see on the manager entry here in chronicle soar this is how you're going to access your manager dependencies in chronicle soar the idea is that we can write some common code for our integration in the manager and then only reference it from actions jobs or connectors this is most common when we deal with authentication for third-party products obviously it's going to be the same thing among all actions connectors and jobs from that integration this is helpful as we're able to code a function once in the manager and reference it throughout our integration scripts let's look at the alien vault manager it's a very simple python file that has its own Imports if it's relevant and constants then we usually create a class but this is not required it can also just be separate functions that you can simply utilize throughout your code thanks for watching

## Assessment

This quiz focuses on the topics covered throughout the course

### Quiz - [Developer Quiz](https://www.cloudskillsboost.google/course_templates/568/quizzes/472958)

#### Quiz 1.

> [!important]
> **Virtual environments have access to the resources of other virtual environments.**
>
> * [ ] False
> * [ ] True

#### Quiz 2.

> [!important]
> **Events have ___________ dictionaries.**
>
> * [ ] Flat
> * [ ] Both Nested & Flat
> * [ ] Nested

#### Quiz 3.

> [!important]
> **Which field(s) in an alert object would be useful for correlating an alert to an external ticketing system?**
>
> * [ ] ticket_id
> * [ ] third_party_id
> * [ ] external_id
> * [ ] system_id

#### Quiz 4.

> [!important]
> **The following are parameters when using the method that's responsible for getting action parameter values:
Example: function(a, b, c) where a,b,c are parameters.
(select all that apply)**
>
> * [ ] input_type
> * [ ] data_type
> * [ ] All of the options
> * [ ] param_name
> * [ ] default_value

#### Quiz 5.

> [!important]
> **How would you add a table to a ScriptResult?**
>
> * [ ] Siemplify.result.data_table()
> * [ ] All of the options
> * [ ] Siemplify.result.table()
> * [ ] Siemplify.result.add_data_table()

#### Quiz 6.

> [!important]
> **Which is the correct way to write an output message to the log?**
>
> * [ ] SIEMPLIFY.LOGGER.output("Value")
> * [ ] SIEMPLIFY.ACTION.log("Value")
> * [ ] SIEMPLIFY.LOGGER.info("Value")
> * [ ] SIEMPLIFY.INSTANCE.output("Value")

#### Quiz 7.

> [!important]
> **The start and end_time are NOT required parameters in an alert object.**
>
> * [ ] False
> * [ ] True

#### Quiz 8.

> [!important]
> **Which folder in the Integration export contains the metadata for actions?**
>
> * [ ] ActionScripts
> * [ ] Dependencies
> * [ ] ActionData
> * [ ] IntegrationDefinitions
> * [ ] ActionDefinitions

#### Quiz 9.

> [!important]
> **A connector can NOT be put in "test mode".**
>
> * [ ] False
> * [ ] True

#### Quiz 10.

> [!important]
> **Each Integration runs in its own virtual environment.**
>
> * [ ] True
> * [ ] False

#### Quiz 11.

> [!important]
> **You can update multiple entities at once.**
>
> * [ ] False
> * [ ] True

#### Quiz 12.

> [!important]
> **What method is used to get action parameters?**
>
> * [ ] get_param
> * [ ] All of the options
> * [ ] extract_action_param
> * [ ] get_action_param

#### Quiz 13.

> [!important]
> **Where would you store common methods, like the authentication to a third party product, for use in an integration?**
>
> * [ ] Action
> * [ ] Manager
> * [ ] Connector

#### Quiz 14.

> [!important]
> **You can manually run actions in cases.**
>
> * [ ] False
> * [ ] True

#### Quiz 15.

> [!important]
> **What icon is used to denote a "Custom Integration"?**
>
> * [ ] Paper Clip
> * [ ] Gear
> * [ ] Pencil
> * [ ] None of these

#### Quiz 16.

> [!important]
> **Select the basic components available as part of a Chronicle SOAR integration (select all that apply).**
>
> * [ ] Actions
> * [ ] Connectors
> * [ ] Plugins
> * [ ] Managers
> * [ ] Jobs
> * [ ] All of the options

#### Quiz 17.

> [!important]
> **The ___________ flag would be used to indicate a failure in your script.**
>
> * [ ] SIEMPLIFY_FAIL
> * [ ] EXECUTION_STATE_FAILED
> * [ ] SCRIPT_FAILURE
> * [ ] SCRIPT_FAILED

#### Quiz 18.

> [!important]
> **Scripts will populate logs with or without a SCRIPT_NAME**
>
> * [ ] False
> * [ ] True

#### Quiz 19.

> [!important]
> **What happens if you don't end an asynchronous action?**
>
> * [ ] The action will not run.
> * [ ] The action will disable itself and alert you.
> * [ ] An infinite loop occurs but the action will timeout.
> * [ ] An infinite loop occurs that can crash your server.

#### Quiz 20.

> [!important]
> **The ___________ flag would be used to indicate that your script completed successfully.**
>
> * [ ] EXECUTION_STATE_COMPLETED
> * [ ] SIEMPLIFY_SCRIPT_SUCCESS
> * [ ] SSCRIPT_COMPLETED
> * [ ] SCRIPT_SUCCESS

#### Quiz 21.

> [!important]
> **It's best practice to wrap your code in a try/except to handle errors.**
>
> * [ ] False
> * [ ] True

#### Quiz 22.

> [!important]
> **Which field is used to hold the raw data in an event?**
>
> * [ ] data
> * [ ] _data
> * [ ] _rawData
> * [ ] raw_data

#### Quiz 23.

> [!important]
> **In the context of the Chronicle SOAR testing platform.The scope specifies ____________.**
>
> * [ ] The connection information.
> * [ ] The action that we'll be running.
> * [ ] The instance we're using.
> * [ ] The entities that we're running our script against.wer

#### Quiz 24.

> [!important]
> **Which flag is used for asynchronous actions to let the Chronicle SOAR API know that the code is to continue running?**
>
> * [ ] EXECUTION_STATE_INPROGRESS
> * [ ] AYNCH_EXCECUTION
> * [ ] SCRIPT_RUNNING

#### Quiz 25.

> [!important]
> **Python dependencies for integrations can be installed in the following ways: (select all that apply)**
>
> * [ ] Manually uploaded through the Siemplify WebUI.
> * [ ] By import statements in your Python code.
> * [ ] Via the CLI using pip.
> * [ ] Have Siemplify download the library from the WebUI.
> * [ ] All of the options

#### Quiz 26.

> [!important]
> **Which of these fields are mandatory when creating an alert object?**
>
> * [ ] display_id
> * [ ] All of the options
> * [ ] alert_id
> * [ ] instance_id

#### Quiz 27.

> [!important]
> **When getting a parameter value, the parameter name is case sensitive.**
>
> * [ ] False
> * [ ] True

#### Quiz 28.

> [!important]
> **Select which objects can be used to iterate over entities:**
>
> * [ ] All of the options
> * [ ] Siemplify.target_entities
> * [ ] Siemplify.entities
> * [ ] Siemplifyaction.entities

#### Quiz 29.

> [!important]
> **What method is used to end a Job?**
>
> * [ ] end_script()
> * [ ] end()
> * [ ] end_job()

#### Quiz 30.

> [!important]
> **You can only have one action in an integration.**
>
> * [ ] True
> * [ ] False

#### Quiz 31.

> [!important]
> **An iteration in an asynchronous action can share information with the next iteration.**
>
> * [ ] False
> * [ ] True

#### Quiz 32.

> [!important]
> **The _______ method is used to update the data in entities.**
>
> * [ ] modify_entities()
> * [ ] update_entity()
> * [ ] update_entities()

#### Quiz 33.

> [!important]
> **Which method(s) would be used to add JSON information that can later be used in a playbook?**
>
> * [ ] Siemplify.result.json()
> * [ ] All of the options
> * [ ] Siemplify.result.result_json()
> * [ ] Siemplify.result.add_result_json()

#### Quiz 34.

> [!important]
> **What method is used to get configuration parameters?**
>
> * [ ] get_param
> * [ ] get_configuration_param
> * [ ] extract_integration_param
> * [ ] extract_configuration_param
> * [ ] All of the options

#### Quiz 35.

> [!important]
> **Siemplify populates a new action with the following libraries: (select all that apply)**
>
> * [ ] ScriptResult
> * [ ] SiemplifyObject
> * [ ] SiemplifyUtils
> * [ ] SiemplifyTools
> * [ ] SiemplifyAction
> * [ ] All the options

#### Quiz 36.

> [!important]
> **Which method is used to let the Siemplify server know that script execution has completed?**
>
> * [ ] script.end()
> * [ ] siemplify.end()
> * [ ] action.completed()
> * [ ] siemplify.completed()

#### Quiz 37.

> [!important]
> **Where do we download integrations for Chronicle SOAR?**
>
> * [ ] Through the Chronicle SOAR WebUI.
> * [ ] Through the Manula portal.
> * [ ] On the Chronicle SOAR website.

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
