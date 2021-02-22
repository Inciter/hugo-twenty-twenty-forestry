
---
wp_id: 64911
wp_post_status: "publish" 
title: "Data Cleaning in Excel 101, Part 1: How to Delete Empty Rows in Excel!"
date: 2020-04-14T12:29:36+05:00
date_modified: 2020-10-18T11:42:21+05:00
date_published: 2020-04-14T12:29:36+05:00
primary_category: "Data Management And Databases"
categories: ['Data Management And Databases'] 
tags: ['']
seo_title: "data cleaning in excel 101, part 1: how to delete empty rows in excel!"
seo_meta_description: ""
summary: ""
featured_image_url: "https://www.inciter.io/wp-content/uploads/2020/04/cleaningsmall.jpg"
slug: "data-cleaning-in-excel-101-part-1"
url: "https://www.inciter.io/data-cleaning-in-excel-101-part-1/"
authors: Kristen Halsey
---

#Content



At Inciter, we use many tools to clean data. Google Sheets and Excel are widely available and powerful tools for basic data cleaning of small to medium data sets. In this series, we will describe different methods for cleaning data that have common problems such as blank rows, duplicates, multiple values in one column, data split into too many columns, leading zeroes, numbers that don’t act like numbers, basic data recoding, and comparing two versions of a spreadsheet. 
#### Method \#1: Sort them out.

Excel’s column sort function won’t order blank cells. If it makes sense to organize your data by a certain column, (i.e. date from newest to oldest), you can sort the entire sheet and watch the completely blank rows fall off. Just be sure all of your data is highlighted prior to sorting. __If you have a lot of blank cells, columns, or rows, Select All may miss some data.__  

<p class="has-medium-font-size">Select all cells...</p>
<p class="has-medium-font-size">Under the data tab, select the “sort” function</p>
<p class="has-text-align-left has-medium-font-size">In the column field, select the column you want to sort by </p>

<p>(use a column that has a value in every row)</p>

<p>Set the order (i.e. newest to oldest, A to Z, smallest to largest).</p>

<p>Click Ok.</p>

#### Method \#2: Filter them out.

Use Excel’s filter function to filter a column for blanks to group them all together for an easy way to select and mark, hide, sort, or delete blank rows all at once.  

<p class="has-medium-font-size">Create a new column called “Row Status”</p>
<p class="has-medium-font-size">Select all cells (Command + A on Mac; Ctrl + A on Windows)</p>

<p>Under the data tab, select the “filter” </p>
<p class="has-medium-font-size">Click one of the filter column tabs where every row has a value and select “(blanks)”</p>
<p>Enter “blank row” in your “row status” column<br/></p>

<p class="has-large-font-size"></p>

<p>Copy this down to your first un-highlighted(un-filtered) row</p>
<p class="has-medium-font-size">Clear your filter</p>

Now you can sort by “row status” to group the blanks for deletion or filtering  
 (NOTE: you must sort by row status to group the blanks together prior to deleting them)
#### What if it’s not that simple? (hint: it’s probably not)
In methods 1 and 2, you might encounter rows that contain blanks, but are not entirely empty. You don’t want to delete these. If you sorted by newest to oldest date, but had some missing dates, you’ve just thrown all of the rows containing blank date cells to the end of your dataset. Context clues (i.e. dates in the rows above and below your blank date cell) might have given you an idea of what the blanks should have been replaced with, but now that you’ve rearranged your rows, you’re not sure where they belong. 
If you find that in your search for blank rows, you are uncovering rows with blank cells, you’ll need to investigate. You don’t want to delete an entire row of data you’ve invested in collecting just because there are a few, or even many, fields missing.
There is a way to find and delete the blank rows in a data set with a lot of missing values...
#### Method \#3. Use a COUNTA formula. Then, sort or filter.
A COUNTA formula counts the number of cells in a range that are not empty. It’s the exact opposite of a COUNTBLANK function. If your data spans 10 columns, wouldn’t it be nice to clearly separate the rows that had data in 9 cells from the rows that only had data in 2?
We use COUNTA rather than COUNTBLANK because it’s easier to think “How many cells in this row have data?” rather than “How many blanks shouldn’t there be?”

<p>Name the first free column next to your data “row status”<br/> </p>

<p class="has-large-font-size"></p>

<p>In the cell below use the formula =COUNTA and include the first row of data in your range. For example, =COUNTA(A2:J2)</p>
<p class="has-large-font-size"></p>

<p>Drag or copy to fill your formula down the column</p>
<p class="has-large-font-size"></p>

<p>Highlight all columns and add then sort by column “row status” Largest to Smallest or Z to A.</p>

Now all of your rows are grouped by how many columns are filled in.  
Stop and take a look at your data. You might see patterns right away, like “every row with ‘2020 Banquet’ has a blank date”. You can figure this one out and preserve your data! Using your “Not blanks” column to group together rows with the same number of non-empty cells will help you put together the missing pieces of your puzzle.
If you want to delete your blank rows, you can scroll down to the first row with 0 in “row status” column and delete all the rows below it.
Now, you can proceed with your data cleaning. You could start by tackling those rows with low numbers in your count “not blanks” column. Now you know how to delete blank rows in Excel!
We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io)


