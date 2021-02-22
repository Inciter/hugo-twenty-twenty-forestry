
---
wp_id: 64936
wp_post_status: "publish" 
title: "Data Cleaning in Excel 101, Part 2: How to Split Columns in Excel."
date: 2020-04-21T09:48:59+05:00
date_modified: 2020-10-15T10:04:43+05:00
date_published: 2020-04-21T09:48:59+05:00
primary_category: "Data Management And Databases"
categories: ['Data Management And Databases'] 
tags: ['data', 'excel']
seo_title: "data cleaning in excel 101, part 2: how to split columns in excel."
seo_meta_description: ""
summary: ""
featured_image_url: "https://www.inciter.io/wp-content/uploads/2020/04/Vacuum.png"
slug: "data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns"
url: "https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/"
authors: Kristen Halsey
---

#Content



Having the right data in the right columns to meet specific requirements for your analysis plays a major role in the data cleaning process. Over the next 3 parts in our Data Cleaning in Excel series, we’ll show you how to solve common issues by utilizing both standard and Excel’s powerful “Flash Fill” shortcut. Part 2 focuses on splitting data from one cell to multiple cells. Part 3 covers the opposite: combining data from multiple columns into one column. Part 4 showcases some incredibly useful and time-saving things you can do with the mystical powers of Excel’s “Flash Fill” function.
#### __Classic Methods and an Introduction to Excel’s Magical Mind-Reading Shortcut “Flash Fill”__
While straightening up datasets, you may encounter cells containing text strings of data that need to be organized into multiple different cells or rearranged entirely. For example, your system may export your donor's full names into a single cell, but first and last names need to be separated to merge properly with another data system.&nbsp;How can you break up first and last names from one cell, and apply the change to entire columns? Try these:
#### Method \#1: "Text to Columns"

<p class="has-medium-font-size">Split one cell into multiple by telling Excel you want to separate contents by a specified delimiter, such as a comma or a blank space.</p>

<p class="has-medium-font-size"><br/>1. <strong>Select</strong> the range of cells you want to convert.</p>

<p class="has-medium-font-size">2. Under the <strong>Data</strong> tab, click <strong>Text to Columns</strong>.</p>

<p class="has-medium-font-size">3. In the “Convert Text to Columns Wizard Step 1 of 3” window that appears, select <strong>Delimited</strong>. Click <strong>Next</strong>. </p>

<p class="has-medium-font-size"><br/>4. In the Step 2 of 3 window, check “<strong>Space</strong>” as your delimiter. Click <strong>Next</strong>.</p>

<p class="has-medium-font-size">5. In the Step 3 of 3 window, make sure “<strong>general</strong>” column data format is selected. Click on the “<strong>Destination</strong>” box to change your new data’s destination to the range of cells immediately to the right of your current data range. </p>

<p class="has-medium-font-size">6. <strong>Highlight the new range</strong> with your cursor. Press <strong>Enter</strong>.</p>

<p class="has-medium-font-size">7. Click <strong>Finish</strong>. Your resulting data should look like this.</p>

#### Method \#2: Flash Fill

Let’s take a look at an example that appears to be a bit more complex. Here, not only do we have our names in one cell, but we have them in the format: (1) surname, (2) a comma and (3) first name. While it’s absolutely possible to pull off transforming these using “Text to Column”, “Flash Fill” is simple and flexible. “Flash Fill” fills a series without a formula. You type how you want your data in the adjacent cell to look, Excel notices a trend in your data entry, and then continues that pattern for you.&nbsp;
<p class="has-medium-font-size">1. In the column next to the range you’d like to change, <strong>type</strong> the donor’s first name in the first two rows. You need to type <strong>two entries</strong> so Excel can recognize that you’re creating a pattern. </p>
<p class="has-medium-font-size"><strong>2. Highlight the range</strong> in the column where you’ve typed your new values. Under the <strong>Data</strong> tab, click the <strong>fill function</strong>, and select “<strong>Flash Fill</strong>” from the dropdown menu.</p>

<p class="has-medium-font-size">3. <strong>Repeat </strong>steps 1 and 2 for your “Last Name” column.</p>

That’s it! You might already be able to think of some more functions for “Flash Fill”. This would work just the same if our donors had a middle initial, a title such as “Mrs.” before or “,Ph.D.” after their name, as long as we type enough values, and type values for special cases, to show Excel our trends.
It’s pretty intuitive, so don’t be afraid to experiment with some new patterns. Just be sure to only apply “Flash Fill” to adjacent cells, and repeat your trend to show Excel what you want. 
Stay tuned for Parts 3 and 4:  
  
Part 3: Combining data from multiple cells into one column  
Part 4: Even more time-saving applications for “Flash Fill”
We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io)


