
---
wp_id: 65060
wp_post_status: "draft" 
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
featured_image_url: /wp-content/uploads/2020/05/Stock-Photo-Bookshelf1.jpeg
slug: "data-cleaning-in-excel-101-part-6-removing-duplicates"
url: "/data-cleaning-in-excel-101-part-6-removing-duplicates/"
authors: Kristen Halsey
---

#Content



In this part of our data cleaning series, well help you find and remove duplicate entries in Excel. Repeats are a very common data entry mistake or error from a data pull. Duplicates in your data can create a variety of unfortunate consequences in administrative duties and analysis. Worst of all, they lead to a real misrepresentation of your results.

This is Part 6 in our Data Cleaning in Excel 101 series. [Part 1](https://www.inciter.io/data-cleaning-in-excel-101-part-1/) showed methods of removing blank rows from your data. [Part 2](https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/) focuses on splitting data from one cell to multiple cells. [Part 3](https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/) covers the opposite: combining data from multiple columns into one column. In [Part 4](https://www.inciter.io/data-cleaning-in-excel-101-part-4-more-uses-for-flash-fill/), we discussed some incredibly useful and time-saving tricks with Excels Flash Fill function. [Part 5](https://www.inciter.io/data-cleaning-in-excel-101-part-5-numbers-that-dont-act-like-numbers-and-leading-zeros/) covers solutions for when your numbers aren't acting like numbers. 

### Removing Duplicate Entries

There are many ways to remove duplicates in Excel. We decided that rather than list 7 ways to accomplish the same thing, lets just walk you through 2 versatile techniques to choose from to fit your needs.

#### Method 1: "Remove Duplicates" Command

Removing duplicate values is routine for us data folks. In fact, its so common that Excel has a dedicated command for it. It's located here in the ribbon, under the "Data" tab.

<img alt="How to Remove Duplicates in Excel" class="wp-image-65061" src="https://www.inciter.io/wp-content/uploads/2020/05/Remove-Duplicates-Command-in-Data-Ribbon.png"/>

1. Select any cell within your dataset. Then, select Remove Duplicates. Excel will intuitively highlight all of the data in your dataset, and youll be directed to a Remove Duplicates window

<img alt="How to Remove Duplicates in Excel" class="wp-image-65062" src="https://www.inciter.io/wp-content/uploads/2020/05/Headers-Window-1024x446.png"/>

3. Keep selected all checked if you want Excel to remove duplicates of full rows that are the same.

We typically would use Select All. However, there are other scenarios in which youd need to delete repeats that technically contain different values in some columns. For example, when working with data entered on different days, data in a time or date entry might be different because of when each was logged. In this case, here is when you would need to check the appropriate columns. For instance, you might want to just check a variable like a user or product ID.

4. Select OK. Excel will remove duplicates from your dataset, and a window will appear telling you how many duplicates were deleted and how many unique values remain.

<img alt="How to Remove Duplicates in Excel" class="wp-image-65063" height="99" src="https://www.inciter.io/wp-content/uploads/2020/05/Duplicates-Removed-Alert-1024x205.png" width="496"/>

#### **Method 2: Formulas and Conditional Formatting**

If you want to carefully examine the duplicates before deleting them, conditional formatting is a great tool. To execute this, youll first need to set up your data by creating a new column, and adding filters, as pictured below.

<img alt="" class="wp-image-65065" src="https://www.inciter.io/wp-content/uploads/2020/05/Setup-with-Headers-and-Filters.png"/>
1. Create a new column and name it combined, or another term that will help you remember the contents.

<img alt="" class="wp-image-65069" src="https://www.inciter.io/wp-content/uploads/2020/05/Filter-Button.png"/>
2. Apply filters to your headers. Select any cell within the parameters of your dataset and select the filter button under the data tab.

<img alt="" class="wp-image-65066" src="https://www.inciter.io/wp-content/uploads/2020/05/Combining-Columns-CONCAT.png"/>
3. In your new combined column, use =CONCAT to combine all of each rows data into the cells in this column.

Refer to our [blog post](https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/) on combining data from multiple cells into one column to learn more about this formula, and a few alternatives you could use instead.

<img alt="" class="wp-image-65073" src="https://www.inciter.io/wp-content/uploads/2020/05/Screen-Shot-2020-05-21-at-3.15.09-PM.png"/>
You new column should look like this.

4. Under the Home tab, select Conditional Formatting, Highlight Cell Rules and Duplicate Values.

<img alt="" class="wp-image-65068" height="200" src="https://www.inciter.io/wp-content/uploads/2020/05/Conditional-Formatting.png" width="351"/>

<img alt="" class="wp-image-65071" src="https://www.inciter.io/wp-content/uploads/2020/05/Screen-Shot-2020-05-20-at-9.09.24-PM.png"/>
5. You can leave the default format as-is, but here, we've customized the format to have a yellow "fill color". This will make it easier to filter in the next step.

<img alt="" class="wp-image-65074" src="https://www.inciter.io/wp-content/uploads/2020/05/Screen-Shot-2020-05-21-at-3.48.49-PM.png"/>
6. Select enter. Your duplicate values will be highlighted.

<img alt="" class="wp-image-65075" src="https://www.inciter.io/wp-content/uploads/2020/05/Screen-Shot-2020-05-21-at-3.57.20-PM-1024x365.png"/>
7. Present a list of just your duplicates by filtering by the color you chose to apply to conditional formatting.

Now, you can go through and examine your duplicate values and see for yourself if there are any outstanding reasons for these errors. If you like, go back and apply method one.

Now you know how to remove duplicates in excel! We encourage you to try out these examples and let us know if you have any questions. We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io).



