
---
wp_id: 65060
wp_post_status: "publish" 
title: "Data Cleaning in Excel 101, Part 6: How to Remove Duplicates"
date: 2020-05-27T10:26:09+05:00
date_modified: 2020-10-18T11:35:53+05:00
date_published: 2020-05-27T10:26:09+05:00
primary_category: "Data Management And Databases"
categories: ['Data Management And Databases'] 
tags: ['excel', 'data']
seo_title: "data cleaning in excel 101, part 6: how to remove duplicates"
seo_meta_description: ""
summary: ""
featured_image_url: "https://www.inciter.io/wp-content/uploads/2020/05/Stock-Photo-Bookshelf1.jpeg"
slug: "data-cleaning-in-excel-101-part-6-removing-duplicates"
url: "https://www.inciter.io/data-cleaning-in-excel-101-part-6-removing-duplicates/"
authors: Kristen Halsey
---

#Content



In this part of our data cleaning series, we’ll help you find and remove duplicate entries in Excel. Repeats are a very common data entry mistake or error from a data pull. Duplicates in your data can create a variety of unfortunate consequences in administrative duties and analysis. Worst of all, they lead to a real misrepresentation of your results.
This is Part 6 in our Data Cleaning in Excel 101 series. [Part 1](https://www.inciter.io/data-cleaning-in-excel-101-part-1/) showed methods of removing blank rows from your data. [Part 2](https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/) focuses on splitting data from one cell to multiple cells. [Part 3](https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/) covers the opposite: combining data from multiple columns into one column. In [Part 4](https://www.inciter.io/data-cleaning-in-excel-101-part-4-more-uses-for-flash-fill/), we discussed some incredibly useful and time-saving tricks with Excel’s “Flash Fill” function. [Part 5](https://www.inciter.io/data-cleaning-in-excel-101-part-5-numbers-that-dont-act-like-numbers-and-leading-zeros/) covers solutions for when your numbers aren't acting like numbers. 
### Removing Duplicate Entries

There are many ways to remove duplicates in Excel. We decided that rather than list 7 ways to accomplish the same thing, let’s just walk you through 2 versatile techniques to choose from to fit your needs.
#### Method 1: "Remove Duplicates" Command
Removing duplicate values is routine for us data folks. In fact, it’s so common that Excel has a dedicated command for it. It's located here in the ribbon, under the "Data" tab.
1. Select any cell within your dataset. Then, select “Remove Duplicates”. Excel will intuitively highlight all of the data in your dataset, and you’ll be directed to a “Remove Duplicates” window

<p>2. If your data is appropriately in tabular format with a header row, check “my data has headers”.<br/></p>

<p><br/>3. Keep “selected all” checked if you want Excel to remove duplicates of full rows that are the same.</p>

We typically would use “Select All”. However, there are other scenarios in which you’d need to delete repeats that technically contain different values in some columns. For example, when working with data entered on different days, data in a “time” or “date” entry might be different because of when each was logged. In this case, here is when you would need to check the appropriate columns. For instance, you might want to just check a variable like a user or product ID.
4. Select OK. Excel will remove duplicates from your dataset, and a window will appear telling you how many duplicates were deleted and how many unique values remain.
#### __Method 2: Formulas and Conditional Formatting__
If you want to carefully examine the duplicates before deleting them, conditional formatting is a great tool. To execute this, you’ll first need to set up your data by creating a new column, and adding filters, as pictured below.

<p class="has-normal-font-size">1. Create a new column and name it “combined”, or another term that will help you remember the contents.<br/></p>
<p class="has-normal-font-size">2. Apply filters to your headers. Select any cell within the parameters of your dataset and select the “filter” button under the data tab.</p>
<p class="has-normal-font-size">3. In your new “combined” column, use =CONCAT to combine all of each row’s data into the cells in this column.</p>

Refer to our [blog post](https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/) on combining data from multiple cells into one column to learn more about this formula, and a few alternatives you could use instead.

<p class="has-normal-font-size">You new column should look like this.</p>

4. Under the Home tab, select “Conditional Formatting”, “Highlight Cell Rules” and “Duplicate Values”.

<p class="has-normal-font-size">5. You can leave the default format as-is, but here, we've customized the format to have a yellow "fill color". This will make it easier to filter in the next step.</p>
<p class="has-normal-font-size">6. Select enter. Your duplicate values will be highlighted.</p>
<p class="has-normal-font-size">7. Present a list of just your duplicates by filtering by the color you chose to apply to conditional formatting.</p>

Now, you can go through and examine your duplicate values and see for yourself if there are any outstanding reasons for these errors. If you like, go back and apply method one.
<p class="has-normal-font-size">Now you know how to remove duplicates in excel! We encourage you to try out these examples and let us know if you have any questions.&nbsp;We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing <a href="mailto:contact@inciter.io">contact@inciter.io</a>.</p>


