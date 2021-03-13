
---
wp_id: 64911
wp_post_status: "draft" 
title: "Data Cleaning in Excel 101, Part 1: How to Delete Empty Rows in Excel!"
date: 2020-04-14T12:29:36+05:00
date_modified: 2020-10-18T11:42:21+05:00
date_published: 2020-04-14T12:29:36+05:00
primary_category: "Data Management And Databases"
categories: ['Data Management And Databases'] 
seo_title: "data cleaning in excel 101, part 1: how to delete empty rows in excel!"
seo_meta_description: ""
summary: "" 
featured_image_url: /wp-content/uploads/2020/04/cleaningsmall.jpg
slug: "data-cleaning-in-excel-101-part-1"
url: "/data-cleaning-in-excel-101-part-1/"
authors: Kristen Halsey
---

#Content



At Inciter, we use many tools to clean data. Google Sheets and Excel are widely available and powerful tools for basic data cleaning of small to medium data sets. In this series, we will describe different methods for cleaning data that have common problems such as blank rows, duplicates, multiple values in one column, data split into too many columns, leading zeroes, numbers that dont act like numbers, basic data recoding, and comparing two versions of a spreadsheet. 

#### Method \#1: Sort them out.

Excels column sort function wont order blank cells. If it makes sense to organize your data by a certain column, (i.e. date from newest to oldest), you can sort the entire sheet and watch the completely blank rows fall off. Just be sure all of your data is highlighted prior to sorting. **If you have a lot of blank cells, columns, or rows, Select All may miss some data.**  

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64899" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture1.png"/>
Select all cells...

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64900" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture2.png"/>
Under the data tab, select the sort function

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64901" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture3.png"/>
In the column field, select the column you want to sort by 

(use a column that has a value in every row)

Set the order (i.e. newest to oldest, A to Z, smallest to largest).

Click Ok.

#### Method \#2: Filter them out.

Use Excels filter function to filter a column for blanks to group them all together for an easy way to select and mark, hide, sort, or delete blank rows all at once.  

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64902" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture4.png"/>
Create a new column called Row Status

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64903" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture5.png"/>
Select all cells (Command + A on Mac; Ctrl + A on Windows)

Under the data tab, select the filter 

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64904" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture6.png"/>
Click one of the filter column tabs where every row has a value and select (blanks)

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64905" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture7.png"/>

<img alt="" class="wp-image-64906" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture8.png"/>

Copy this down to your first un-highlighted(un-filtered) row

<img alt="How to Delete Blank Rowsin Excel" class="wp-image-64907" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture9.png"/>
Clear your filter

Now you can sort by row status to group the blanks for deletion or filtering  
 (NOTE: you must sort by row status to group the blanks together prior to deleting them)

#### What if its not that simple? (hint: its probably not)

In methods 1 and 2, you might encounter rows that contain blanks, but are not entirely empty. You dont want to delete these. If you sorted by newest to oldest date, but had some missing dates, youve just thrown all of the rows containing blank date cells to the end of your dataset. Context clues (i.e. dates in the rows above and below your blank date cell) might have given you an idea of what the blanks should have been replaced with, but now that youve rearranged your rows, youre not sure where they belong. 

If you find that in your search for blank rows, you are uncovering rows with blank cells, youll need to investigate. You dont want to delete an entire row of data youve invested in collecting just because there are a few, or even many, fields missing.

There is a way to find and delete the blank rows in a data set with a lot of missing values...

#### Method \#3. Use a COUNTA formula. Then, sort or filter.

A COUNTA formula counts the number of cells in a range that are not empty. Its the exact opposite of a COUNTBLANK function. If your data spans 10 columns, wouldnt it be nice to clearly separate the rows that had data in 9 cells from the rows that only had data in 2?

We use COUNTA rather than COUNTBLANK because its easier to think How many cells in this row have data? rather than How many blanks shouldnt there be?

<img alt="" class="wp-image-64908" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture10.png"/>

In the cell below use the formula =COUNTA and include the first row of data in your range. For example, =COUNTA(A2:J2)

<img alt="" class="wp-image-64909" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture11.png"/>

Drag or copy to fill your formula down the column

<img alt="" class="wp-image-64910" src="https://www.inciter.io/wp-content/uploads/2020/04/Picture12.png"/>

Highlight all columns and add then sort by column row status Largest to Smallest or Z to A.

Now all of your rows are grouped by how many columns are filled in.  
Stop and take a look at your data. You might see patterns right away, like every row with 2020 Banquet has a blank date. You can figure this one out and preserve your data! Using your Not blanks column to group together rows with the same number of non-empty cells will help you put together the missing pieces of your puzzle.

If you want to delete your blank rows, you can scroll down to the first row with 0 in row status column and delete all the rows below it.

Now, you can proceed with your data cleaning. You could start by tackling those rows with low numbers in your count not blanks column. Now you know how to delete blank rows in Excel!

We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io)



