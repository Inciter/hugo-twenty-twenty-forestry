
---
wp_id: 65323
wp_post_status: "draft" 
title: "Understanding Data Integration"
date: 2020-10-29T08:54:41+05:00
date_modified: 2020-10-29T08:54:41+05:00
date_published: 2020-10-29T08:54:41+05:00
primary_category: "Uncategorized"
categories: ['Uncategorized'] 
seo_title: "understanding data integration"
seo_meta_description: ""
summary: "" 
featured_image_url: /wp-content/uploads/2020/04/integrationwhite.jpg
slug: "understanding-data-integration"
url: "/?p=65323"
authors: Jacob Joseph
---

#Content



We need a new data system. The stuff of dreams and nightmares. Whether you arent storing the right data in your system, or you cant get what you want out of it, you either have considered a new data system, or you were in the process of implementing one.

Decide how to spend your technology budget is always hard. And moving to a new system will inevitably involve a huge cost because migrating your existing data to a new system is very labor-intensive. Why spend a year and tens (or hundreds) of thousands of dollars on a new system, when you probably have what you need right now? A better option is a **data integration project** instead. Data integration with right-sized data infrastructure allows you to get more out of the data that you have in one or more systems without having to move it all to a new system. Beyond just repurposing the funds, you can also** reduce the risk, the time required, and the potential stress of your staff **that is so common during major migrations.  

### Modern Data Integration Concepts

#### **All my data is in one place and ready for analysis. How do I use it?**

Connect your data to **analysis, business intelligence(BI), and reporting tools**. These can be used for:  

*   Creating dashboards for stakeholders and leadership
*   Periodic reporting to answer specific questions
*   Ad-hoc reporting to answer general questions or look for trends
*   Collecting and organizing data for a future migration

You can use general tools or specialized tools depending on what type of output you want and what type of data you have. These tools often offer advanced visualizations and in-depth analysis that out of box reporting does not provide.

__If your data is:  __

*   Stored in a data lake or data warehouse, and youve got data pipelines to keep it up to date
*   Or in a system that directly integrates with your preferred tools for analysis, BI, and reporting

**Then:**

*   Setting up BI and reporting tools is relatively simple because youre using a common data source or easily integrated data sources
*   You can access, analyze and report on data from one or multiple systems in the same place
*   Your data has already been processed and cleaned with your data pipelines or your data cleaning tools and processes, so its ready to use

#### **That sounds great, but what if my data needs to be cleaned, isnt easy to connect to, or is in different places or systems?**

If your data is cleaned and structured the way that you need for reporting, then a **data warehouse** is probably a good fit for you. Use a data warehouse to provide access to your data.

#### **What is a data warehouse?**

A data warehouse is a location or service that stores data and makes standard connectors available. Data warehouses are good for frequent and consistent access to data. And you only need to add data that you plan to use. Data warehouses store your data in a common format and provide standard connectors for data analysis, visualization, and reporting tools.

#### **So how do I get my data into the data warehouse?**

Create **data pipelines** to move your data from one place to another, translate between formats, or even clean your data.  

#### **What is a data pipeline?**

A data pipeline is just a process or tool that moves data from one place to another and can make small changes to the data if needed (like decompressing a compressed file or adding a date and time to the end of a file name).

> contact@inciter.io if you have challenges getting data out of your system.

Each step in a data pipeline is like one piece of pipe that just does a simple task, and you connect the different pipe pieces together to make a pipeline. This way you can reuse the different pieces of the pipeline. For instance if you created a pipeline that retrieved data from your data system the pieces might look like this:  

*   Connect to data source or data system
*   Download specific data set
*   Create a CSV file from the data set
*   Compress the CSV file
*   Save the compressed CSV file in the right place

You might have another pipeline that watches the folder called cleaned and when it sees a new file imports it to your data warehouse.  

Whats so useful about this approach is that each of the pieces can be reused as needed. Instead of designing a single process for each combination of data source and end result, you just connect the pieces you need. Its like an erector set for data.  

#### **How do I create a data pipeline?**

There are multiple ways to make data pipelines. There are specialized tools that are low-code or no-code that just give you the pieces you need and you tell them which data or system to act on, and there are others that are based in programming which require coding. There are also many tools that offer pre-built pipelines for common data sources. Some BI tools even include some very basic data pipelines for the most common data sources.

Data pipelines can be manual or partially manual like exporting a file from your CRM and uploading the file into your business intelligence (BI) tool, but most data pipelines are automatic like fetching data from your data system periodically or as it changes and saving that data somewhere.

You can even have data pipelines that flow through tools that clean or restructure your data automatically!

#### **What if my data needs a lot of cleaning or restructuring? What if my data is difficult to get into my data warehouse or I dont want to load everything into my data warehouse?**

If your data requires a good bit of cleaning, restructuring or reformatting to get into your reporting or BI tool or into your data warehouse, then a **data lake** might be a good option. Data lakes are also great for archival storage for infrequently used data and storage of data that arrives faster than it can be prepared for use.

#### **What is a data lake?**

A data lake is just a place where you can store and organize lots of data without having to define what the data look like or what format they are in. It could be a Google Drive folder or a shared drive. Cloud data lakes are data lakes stored on redundant servers managed by someone else. They are more reliable and available than locally stored data lakes and have a significantly reduced maintenance and overhead cost.

With data stored in a data lake, its a good idea to store your data as-is prior to any modification, reformatting, etc. This makes it easy to start again with the original data if you need to use it differently later on or need a different slice of the data.

#### **How do I store data in a data lake?**

Once youve gotten your data stored in your data lake, youll probably want to access it! A data warehouse allows you to access the data thats stored in your data lake by putting it in a common format and providing connectors for data analysis, visualization, and reporting tools.

#### **How do I organize the data I put in the data lake?**

Segmentation of data is very important to create a usable data lake, but its also pretty simple! You just need to organize your data into folders or segments that correspond to things like:

*   Data processing stage or category (raw, cleaned, formatted, published, etc.)
*   Data source or destination (fromFinanceSystem, fromGoogleAnalytics, forMembershipDirector, etc.)
*   Data set (WebsiteVisits, DonorResponses, Clients, etc.)
*   Date and time (2020/04/23, 2020-04-03-18:25, etc.)

Each segment should nest within the previous segment. So you might have multiple spreadsheets saved in a folder called cleaned/fromGoogleAnalytics/WebsiteVisits/2020/04/23 that would contain all of the cleaned website visit data from Google Analytics on 4/23/2020.  

Good segmentation should allow you or a computer to easily navigate and find your data. It prevents your data lake from becoming a data swamp!  

#### **How do I use data in a data lake?**

*   You can add a data pipeline to load only the data that you will need into your data warehouse
*   Your data warehouse may connect directly to a data lake if files are in common formats (CSV for instance)
*   There are special data warehouses that allow you to asks questions about your data without having to load it
*   Some data warehouses can actually crawl through your data lake and look for data and add it automatically to your data warehouse

#### **To Sum It Up...**

Each of the above pieces of data integration make up your data infrastructure. They can build upon each other to solve complex challenges or be used alone for simpler ones. A reporting or BI tool can be used to gain and share insights from your data. A data warehouse can make your data readily available. A data lake can store and archive your data as-is so you dont have to load it all at once or if you dont need all of it frequently. Data pipelines modularly connect all the pieces so that you can reuse the processes and tasks for similar challenges.



