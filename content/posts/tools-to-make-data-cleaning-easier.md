---
title: "Tools to make data cleaning easier"
date: 2020-10-21T14:22:15-07:00
year: 2020
month: "10"
aliases: [
    "/my-other-new-blog-post"
]
categories: ["Databases"]
author: "Jacob Joseph"
featured_image_url: "flat-lay-photography-of-hand-tools-1029243.jpg"
---

Cleaning, wrangling, munging, preparation, validation, ETL, transformation, ELT… these are all different names for “making data more useful.” Whether you’re doing one-off analysis, scheduled reports analytics, or integrating two different data systems or applications, when you work with data, data cleaning is an important part of almost all data processes. Data cleaning is taking data as-is and changing the content, structure or format to be more useful. Removing blank rows and deleting invalid addresses are examples of data cleaning. Data cleaning can be the most laborious part of a data analysis project. At Inciter, we use tools to streamline the process and save us hours of tedious work.

There are a seemingly endless number of tools to assist in the process of data cleaning. Some of them can only be used for specific data cleaning tasks (like address verification), and others are multifunctional and are used for a variety of data cleaning tasks. We use three kinds of tools for data cleaning: manual, programmatic, and automated. Below, we describe the difference between those tools, strengths and weaknesses, and offer a few recommendations of tools worth checking out.

MANUAL DATA CLEANING TOOLS
Data set size: Small to Medium (up to ~2 million values)
Transformation complexity: Simple to Moderate
Cost: Low
Start-up effort: Low
Ongoing effort: High
Manual tools are great for exploring a data set. However, they cannot handle large datasets. These tools typically reach their limit around 1 million values – e. g., 100 columns with 10k rows.  Their capacity is also limited by the number of formulas in use. For large data sets, these manual tools can be used for prototyping a data cleaning process and doing one-off data cleaning on a smaller set of sample data. There is some automation possible through scripting languages (Macros, VBA, and Google Apps Scripts) but it is often fragile and difficult to maintain.

Repeating periodic processes like a monthly or weekly report or dashboard will usually involve an employee doing each individual step manually which is error-prone and time consuming. At Inciter, we use both Excel and Google Sheets on a daily basis for small data projects and one-off analyses.

Tools recommended for simple, manual data cleaning
Excel is best used for data sets with fewer formulas and for sharing with people who don’t have access to a Google Account.
Google Sheets is best used for data sets with more formulas and for collaborating with others in real time.
AUTOMATED DATA CLEANING TOOLS
Data set size: Any
Transformation complexity: Any
Cost: High for paid tools, Low for open-source tools
Start-up effort: Low for paid tools, High for open-source tools
Ongoing effort: High
Automated tools provide a more user-friendly way to set up repeated data cleaning processes, but they aren’t 100% automated. They often include drag-and-drop interfaces as features to estimate data quality–for example, checking that all dates are valid dates. Paid tools are often more intuitive, and offer professional services, support, documentation and/or training with their licensing. Open-source or community tools are “free”, but they often have a steep learning curve and may be difficult to maintain and support.

While applying these tools is more practical than learning a programming language, their limitations should be strongly considered prior to implementation. Their price rises with their data capacity. These tools are worth investing in if you have a team without programming expertise or if you need to move very quickly. At Inciter, we use these services when they provide good fits for our client needs based on the speed of delivery needed and affordability within the clients’ project budget.

Tools recommended for automate data cleaning (paid)
Trifacta is a powerful tool for AI-assisted data cleaning that can simplify complex data cleaning processes without programming. 
Google Dataprep by Trifacta is a version of Trifacta offered through Google.
Google Cloud Data Fusion is a tool focused on connecting and transforming data. It can be used with Google Dataprep and has a  drag-and-drop interface.
Honorable mentions (paid)
Parabola is an easy to use and learn and is relatively inexpensive. However, it is not suitable for use with sensitive data or large datasets.
Hevo and Panoply are both suitable for light transformations and include many pre-built connectors to commonly used enterprise tools; they focus on moving and centralizing data.
Stitch is suitable for light transformations and includes many pre-built tools. It features open-source versions of its connectors.
Cloudingo  is a Salesforce data tool that features pre-built cleaning processes and tasks.
Honorable mentions (has open-source or community version available)
DataCleaner handles data profiling, quality, and analysis, in addition to cleaning.
KNIME is a data-science focused tool. Paid versions of this tool scale up to handle larger data sets.
Orange is a visual interface for building data workflows with special features for machine learning and advanced data visualization.
RapidMiner is a data-science focused tool built around modeling and performing complex data analysis.
OpenRefine is an application most useful for cleaning large datasets, but is not practical for automating repeated processes.
PROGRAMMATIC DATA CLEANING TOOLS
Data set size: Any
Transformation complexity: Any
Cost: Low
Start-up effort: High
Ongoing effort: Medium
If you are a developer or have them on staff, you might consider employing a programming language to simplify repeated processes. Although these usually don’t require an upfront software cost, their usability is contingent upon skills and expertise. These programming tools have the capacity to handle large volumes of data. If you already have an expert on staff, applying this method may be the most time and cost-effective solution. It can be difficult to maintain though as it requires continued updates to stay usable in the long-term.

Developers use notebook-style sharing tools like Google Colaboratory, JupyterLab, and Jupyter Notebook to create processes that others without working knowledge of programming can use. At Inciter, we use Python and notebook-style sharing tools to automate some complex data cleaning processes.

Tools recommended for programmatic data cleaning
Python is easier to learn than other programming languages. Many high quality free and paid online resources are available for learning Python, so you can find approachable methods to help you master Python.
Pandas is a commonly used library for operating on tabular data.
Spyder IDE is a tool with features for easy interactive data viewing and manipulation with Python.
Google Colaboratory is a notebook-style tool that makes sharing easy through Google Drive. In addition to data cleaning, you can use it for analysis and visualization.
At Inciter, we work with nonprofits to help them have more impact by using data they already have. If you are on the struggle bus with your reporting, or you spend hours and hours wrestling with Excel sheets, there is a good chance we can take that off your plate and give you the insights you need with a lot less effort.

Contact us at contact@inciter.io and we can tell you about our Impact Road Map. This process will uncover ALL the uses for your data, where it all is stored, what’s possible with what you’ve got, and will reveal your next steps.