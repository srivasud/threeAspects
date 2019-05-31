# How to run a data visualization project

Every data viz project begins with a need, whether that needs come from a problem, decision, or clarification, there is a certain process for each project. Firstly, each project needs data to visualize. The data that is being used and the procurement of that data is essential as it will mold the audience, argument and metric that will all need to be evaluated throughout the steps of the project. Next, an argument needs to be made that will utilize the data to explain, answer, or convey the point the viz is made to get across. Developing a good argument requires a warrant and backing followed by a rebuttal and qualifier all to support the overall argument. Following a formed argument the visualizaiton can be constructed to establish the audience and take into account the aspects of the data that will be used. In all, a data viz project has these basic steps, but the intricacies of each use case is where complexity plays a factor. Complexity can be rivaled by using subject matter experts and practices utilized by other viz projects that are explained throughout this reader.

## Introduction

While designing a data analytics project, we are often left wondering where to begin with in the first place? From data collection, cleaning, exploration, analysis and visualization, there is a lot that needs to be done in order to derive an insight that is - actionable & profitable, for the business. 

There seems to be a no set way to approach this problem. However, in order to provide a framework to organize the work needed by an organization and deliver clear insights from data, it’s useful to think of it as a cycle with different stages.[@dataviz_lifecycle1]. This article explains a data science framework, breaking it down and taking us through each step of the project lifecycle to get us familiarized with the whole process in a simpler way.[@dataviz_lifecycle2]

![](images/CRISP-DM.png)

### Step 1: Understanding the Business Issues
At the start of the project, the focus is to get a clear understanding of the overall scope of the work, business objectives, information the stakeholders are seeking, the type of analysis they want you to use, and the key deliverables. Defining these elements prior to beginning the analysis is important, as it helps in delivering better insights. Also, it is important to get a clarity at the beginning as there may not be another opportunity to ask questions before the completion of the project.

### Step 2: Understanding Your Data Set
This phase starts with an initial data collection and proceeds with activities like data quality checks, data exploration to discover first insights into the data, or to detect interesting subsets to form hypotheses for hidden information. There are a variety of tools we can use to understand the data. Depending on the size of the dataset, we can use Excel for manageable datasets, or use more rigid tools like R, Python, Alteryx, Tableau Prep or Tableau Desktop to explore and prepare the data for further analysis.

Key things to remember would be to identify key variables of interest to study the data, look for errors (omitted data, data that doesn’t logically make sense, duplicate rows, or even spelling errors) or any missing variables that need to be amended so we can properly clean the data.

It is important to note here that when working in an enterprise/ business environment, it helps to involve someone with keen knowledge of the source system such as a DBA who can assist with understanding and extraction of data. 

### Step 3: Data Preparation
Once the data has been organized and all the key variables have been identified, we can begin cleaning the dataset. Here, we will handle missing values (replace with means, drop the rows or replace with the most logical values), create new variables to help categorize the data, and remove duplicates. Data preparation tasks are likely to be performed multiple times, and not in any prescribed order. After this step, the final dataset is ready to be fed into a modeling tool for further analysis.

From a business perspective, throughout the data preparation process the need is to develop an ever-increasing understanding of the data’s structure, content, relationships, and derivation rules. It is imperative to verify that the data exists in a usable state, and its flaws can be managed, and understand what it takes to convert it into a useful dataset for reporting and visualization. In such a scenario, leveraging Data profiling can help explore the actual content and relationships in the enterprise' source systems. Data profiling can be as simple as writing some SQL statements or as sophisticated as a special purpose tool. Tableau's Data Prep for instance is a great tool for profiling data for small scale projects. With enterprises, many ETL vendors offer a variety of tools can be chosend based on the need and budget of the business.

### Step 4: Modeling
In this step, we will use various modeling techniques to test the data and seek out answers to the given objectives. Typically, there are several techniques for the same data mining problem type, with some specific requirements on the form of data. Common models include linear regressions, decision trees, and random forest modeling, among others.

### Step 5: Validation
Once we are done building the model (or models) and proceed to the final deployment, it is crucial to assess the model thoroughly and review the steps executed to construct the model, to ensure that it properly achieves the business objectives. Did the models work properly? Does the data need more cleaning? Did you find the outcome the client was looking to answer? If not, you may need to go over the previous steps again. You should expect a lot of trial and error!

At this step, it is key to identify issues, definitions, transformation rules, and data quality challenges and document them for future reference. Such a documentation is useful from a business standpoint for future users. Maintaining a list of issues and validating new issues faced during data validation can significantly enhance the quality of the project and help improve scope for future improvements and define infrastructure needs of the business.

### Step 6: Visualization
Creation of the model is generally not the end of the project. Even if the purpose of the model is to increase knowledge of the data, the derived information will need to be organized and presented in a way that is useful to the customer. Depending on the requirements, this step can be as simple as generating a report or as complex as implementing a repeatable data scoring (e.g. segment allocation) or data mining process.

In many cases, data visualization will be crucial in communicating your findings to the client. Not all clients are data savvy, and interactive visualization tools like Tableau are tremendously useful in illustrating your conclusions to clients. Being able to tell a story with your data is essential. Telling a story will help explain to the client the value of your findings.

As with any other project, it is important to identify the business objectives clearly. Breaking the process into steps will ensure we get the best deliverables for our clients.

### Step 7: Documentation
An important addition to the steps in a data visualization project is documentation. Similar to the projects done in class, this documentation should provide a brief description of the project, data sources, data profile and quality, limitations of the data or arising during the use of data, key transformations and models introduced and their impact or usefulness in enhancing the quality of visualization. 
Lastly, this documentation should also note the issues encountered when working with the data or creating a certain visualization that can be addressed in the future.

## Important Prerequisites of data visualization project

The below are the important prerequisites of a successful data visualization project.
[@prerequisites_vizhitachi]

+ **Defining the project** Behind every project there is an organizational need. The need could be as simple as a weekly sales performance dashboard or a sophisticated predictive recommendation engine. Addressing these needs with a concrete measurable objectives provide the right framework to deliver the right information in  right fashion. The communication of Key Performance Indicators (KPIs) from the end product is very important for the consumers. To do this, you need to collect requirements, set design processes, schedule regular discussions with users and continue these meetings until the final project rollout.

Sample questions that can help one understand the project better:
  + what is the organization need you are trying to address?
  + What are the main data sources you need to access? 
  + Is the data upto date or will it provide updated data in regular intervals?
  + which type of data visual works best?
  + Is there a measurable goal you want to achieve?
  + What are the core KPIs to convey to users if any?
  + Which type of KPI visualization is suitable for this goal?
  


+ **Understanding the audience** How will they process this visualization is another important prerequisite. Designing a visualization for scientists is entirely different from a visualization designed for law-makers or for general public. Most user want to see 'Key performance indicators' which are the main drivers for visualizations. The following are different kinds of visualizations that can be used to display KPIs:
  + Quantities: counts or measures. Example - Count of likes or comments
  + Trends and changes over time:  time series. Example - Change in sales quantity over time
  + Relatives Share and proportions:  display relationship between the parts and the whole. Example - breakdown of a stock portfolio by asset.
  + Ranked list: although not a real data visualization, it could achieve the goal needed.
  + Geographical Location: Gives user spatial and physical relationships.

+ **Understanding the audience** How will the consumers process this visualization, is another important prerequisite. Designing a visualization for scientists is entirely different from a visualization designed for law-makers or for general public. Most users want to see 'Key performance indicators' which are the main drivers for the visualizations. The following are different kinds of visualizations that can be used to display KPIs:
  + Quantities: counts or measures. Example - Count of likes or comments.  
  + Trends and changes over time:  time series. For example, Change in sales quantity over time.  
  + Relatives Share and proportions:  display relationship between the parts and the whole. Example - breakdown of a stock portfolio by asset.  
  + Ranked list: although not a real data visualization, it could achieve the goal needed.  
  + Geographical Location: Gives user spatial and physical relationships.  


[@prerequisites_tools]
  Choosing a tool, depends on the person conducting or designing the visualization, and the platform he wants to integrate his work into.It also depends on the ability of the user and their needs. eg:-Tableau has a no code approach whereas D3.js ,Altair etc has coding approaches. These approaches help users to adopt and customize further. For example: With Tableau, users can add customization such as a new formula addition, sorting behaviors to the charts initially developed, whereas D3.js and other coding tools may not give that flexibility and the users are dependent on the designer to make further changes.

These approaches are discussed in detail below:

**No coding:**
One can start with MS Excel and probably use pivot tables feature, in excel you come up with decent charts. If you already have some data and need a powerful tool to explore the data visually, Tableau is the tool. There is a free public version and a paid version , which students can get for free. One can publish the charts to web .To start Tableau Public website has a good number of examples to take inspiration from.

**Some coding:**
If somebody wants to venture in the coding world to build charts, R is a good start. It is easy to learn, free as it is opensource.One can us the ggplot library in R to come up with visual data exploration. You can publish these charts with the help Shiny package and add a bit of interaction as well.

**More coding:**
This section is derived because of recent innovation in interactive visualization, especially on the web. One might ask where to start to come up with interactive visualizations as good as New York Times. The answer is D3.js, many of the data visualizations running in the browser today is D3.js, created by Mike Bostock. This does mean you&#39;ll need to learn some Javascript in general and then D3.js specifically. One area to call out as a particular strength of D3 is geospatial visualizations. D3 is great at creating maps of many flavors.

Finally, if you really want to learn a do-it-all programming language that just happens to be great at data visualization, go with Python. Python is a general purpose and powerful tool, and it&#39;s quite popular in the data science community. Finally, much like D3.js for Javascript or ggplot for R, there are many Python libraries dedicated to data visualization. Seaborn (which builds on an older popular library, matplotlib) and Bokeh are probably the best-in-class right now, but this is a quickly evolving and improving landscape. Both the [Seaborn](http://stanford.edu/~mwaskom/software/seaborn/examples/index.html) and [Bokeh](http://bokeh.pydata.org/en/latest/docs/gallery.html) websites include galleries showing off the kinds of visualizations you can create with those tools.

+ **Understanding the data you are trying to visualize** such as shape, dimension of the data, is data a time-series, relationship in data between entities,categorical attributes is also an important prerequisite. Is this data from a single source or multiple sources?. If the data is from multiple sources, they need to be blended together without loosing the meta data constraints and business rules. When the data is collected, the end goal should be kept in mind.

+ **Deciding which visual is best.**
One of the biggest challenges for business users is deciding which visual should be used to best represent the information. Tables, Linechart, Areachart, Barchart, Scatterplots, Piechart, Treemaps, Heatmaps, Natual Language Generation, Etc.
