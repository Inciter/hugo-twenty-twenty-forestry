
---
wp_id: 64990
wp_post_status: "publish" 
title: "Data Cleaning in Excel 101, Part 3: How to Combine Columns in Excel"
date: 2020-05-04T16:24:15+05:00
date_modified: 2020-10-15T11:10:02+05:00
date_published: 2020-05-04T16:24:15+05:00
primary_category: "Data Management And Databases"
categories: ['Data Management And Databases'] 
tags: ['data', 'excel']
seo_title: "data cleaning in excel 101, part 3: how to combine columns in excel"
seo_meta_description: ""
summary: ""
featured_image_url: "https://www.inciter.io/wp-content/uploads/2020/05/Sweeping-Dandelion-scaled-e1588610847952.jpg"
slug: "data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns"
url: "https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/"
authors: Kristen Halsey
---

#Content


Having the right data in the right columns to meet specific requirements for your analysis plays a major role in the data cleaning process. In Parts 2, 3, and 4 of our Data Cleaning in Excel series, we’ll show you how to solve common issues by utilizing both standard and Excel’s powerful “Flash Fill” shortcut.

  
[Part 2](https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/) focuses on splitting data from one cell to multiple cells. Here, in Part 3, we’ll cover the opposite: combining data from multiple columns into one column. Coming up in Part 4, we’ll showcase some incredibly useful and time-saving tricks with the mystical powers of Excel’s “Flash Fill” function.
#### Combining Data from Multiple Columns
In our last blog post, we went over how to break apart data that has been exported into just one cell. What about if you have the opposite issue: data in multiple cells that you need to join together? For example, your system may export your donor's names into first and last names, but you need to put them together in one cell for your next project. How can you put together the data from both cells, and apply the change to an entire column? Try these:
#### Method \#1: CONCATENATE
The Excel formula =CONCATENATE allows you to join together text strings from multiple cells into just one. You can use the formula to combine numbers, text, and characters in addition to cell references.  

<p class="has-medium-font-size">1. <strong>Select</strong> the cell for your new value, adjacent to your cells you need to combine.&nbsp;</p>

<p class="has-medium-font-size"><br/>2. <strong>Type</strong> =CONCATENATE(</p>
<p class="has-medium-font-size">3. <strong>Select</strong> your first cell reference (first name).&nbsp;</p>

<p class="has-medium-font-size"><br/>4. Add a <strong>comma </strong>to indicate a new text string.&nbsp;<br/><br/>5. <strong>Type</strong> “ “ to indicate a space between your values.</p>

<p class="has-text-align-left has-medium-font-size">6. Add another <strong>comma</strong>.</p>
<p class="has-text-align-left has-medium-font-size">7. <strong>Select</strong> your second cell reference (last name).</p>
<p class="has-text-align-left has-medium-font-size">8. <strong>Add</strong> a “)” to close your parentheses and finish the formula.</p>

<p class="has-medium-font-size">9. Click <strong>Enter</strong>. Your new values will appear.</p>

<p class="has-medium-font-size">10.&nbsp;<strong>Drag </strong>your formula to fill your new column.</p>

#### Tip: When simply joining two cells, use an ampersand instead.   
No formula required.  
<p class="has-normal-font-size">Instead of writing the formula, you can use "&amp;" directly between the cells you want to join.</p>
<p class="has-text-align-center" style="font-size:22px"><strong>=<span style="color:blue">A1</span>&amp;<span style="color:red">B1</span></strong></p>
<p class="has-normal-font-size">It's a shorthand variation of the the =CONCATENATE formula best used when you just need to add two cells. Things get a little more complicated when you need to add a delimiter, or need to use Excel's formula builder function.</p>
#### Method \#2: CONCAT
Newer versions of Excel (after Excel 2010) have upgraded the =CONCATENATE formula to =CONCAT. The =CONCATENATE formula is still available in every version of Excel to remain compatible with older versions. The difference between the formulas is that =CONCAT can combine cell references in an entire range to fit one cell. 
The instructions for use are essentially the same as the =CONCATENATE formula above in method 1. If you want to perform the same function you can do with =CONCATENATE, just type and execute as you normally would (see below). 
<h4 class="has-text-align-left">CONCAT and Range References</h4>

<p class="has-medium-font-size">To combine range references, click a cell and expand and drag an entire range.</p>
<p class="has-medium-font-size">After you execute the formula, your new cell will look like this.</p>

#### Method 3: TEXTJOIN
If you need to combine a range of cells into text with spaces, commas or another separator, and you don’t want to waste time entering it repeatedly between cell references, use =TEXTJOIN. When you type =TEXTJOIN, Excel prompts you to provide: __(delimiter, ignore\_empty, text1, \[text2\], …)&nbsp; __
- __delimiter__ is where you specify what you want to separate the cells. In our case, we would want a “ “, to create spaces between words in our cell references.  
  
-__ ignore\_empty__ is where you choose “TRUE” or “FALSE” in regards to including empty cells. If you do want empty cells to be included, type “TRUE”. Your choice will depend on the data you have and your purposes for combining the text.  
  
- __text 1__ is the cell reference(s) you must include in your formula to execute the function (including ranges and arrays).  
  
- __\[text 2\]__ is an optional argument where you can provide additional cell references to combine if you need to.
<p class="has-text-align-center has-medium-font-size">When filled out, you formula should look like this:</p>

<p class="has-medium-font-size">Press “Enter”, and you’ll find that TEXTJOIN has combined all of your cell references easily, without having to tediously write “ “ between each cell. </p>

#### Method \#4: Flash Fill
<p class="has-medium-font-size">Check out our <a href="https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/">last data cleaning blog post</a> in this series for a review of the Excel function, “Flash Fill”.&nbsp;</p>

<p class="has-medium-font-size">To combine data into one column, we’ll type how we want our new data to look in the cell adjacent to our existing data. Remember, we have to create two entries so Excel can recognize our pattern, and fill in the rest for us. </p>

Stay tuned for Part 4 of our Data Cleaning in Excel series for an in-depth look at the versatility of Flash Fill and some example formats that are sure to inspire you to use the function in your day-to-day work in Excel.
We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io)


