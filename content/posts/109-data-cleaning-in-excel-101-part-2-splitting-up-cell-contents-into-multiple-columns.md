
---
wp_id: 64936
wp_post_status: "draft" 
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
featured_image_url: /wp-content/uploads/2020/04/Vacuum.png
slug: "data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns"
url: "/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/"
authors: Kristen Halsey
---

#Content



Having the right data in the right columns to meet specific requirements for your analysis plays a major role in the data cleaning process. Over the next 3 parts in our Data Cleaning in Excel series, well show you how to solve common issues by utilizing both standard and Excels powerful Flash Fill shortcut. Part 2 focuses on splitting data from one cell to multiple cells. Part 3 covers the opposite: combining data from multiple columns into one column. Part 4 showcases some incredibly useful and time-saving things you can do with the mystical powers of Excels Flash Fill function.

#### **Classic Methods and an Introduction to Excels Magical Mind-Reading Shortcut Flash Fill**

While straightening up datasets, you may encounter cells containing text strings of data that need to be organized into multiple different cells or rearranged entirely. For example, your system may export your donor's full names into a single cell, but first and last names need to be separated to merge properly with another data system. How can you break up first and last names from one cell, and apply the change to entire columns? Try these:

#### Method \#1: "Text to Columns"

<img alt="" class="wp-image-64955" src="https://www.inciter.io/wp-content/uploads/2020/04/Step-1-Select-Range.png"/>
Split one cell into multiple by telling Excel you want to separate contents by a specified delimiter, such as a comma or a blank space.

1. **Select** the range of cells you want to convert.

2. Under the **Data** tab, click **Text to Columns**.

<img alt="" class="wp-image-64956" height="81" src="https://www.inciter.io/wp-content/uploads/2020/04/2.-Under-the-Data-tab-click-Text-to-Columns.-1024x155.png" width="540"/>

<img alt="" class="wp-image-64957" src="https://www.inciter.io/wp-content/uploads/2020/04/Step-3-Check-delimited-1024x776.png"/>
3. In the Convert Text to Columns Wizard Step 1 of 3 window that appears, select **Delimited**. Click **Next**. 

4. In the Step 2 of 3 window, check **Space** as your delimiter. Click **Next**.

<img alt="" class="wp-image-64959" src="https://www.inciter.io/wp-content/uploads/2020/04/Screen-Shot-2020-04-20-at-7.23.31-PM-1024x776.png"/>
5. In the Step 3 of 3 window, make sure **general** column data format is selected. Click on the **Destination** box to change your new datas destination to the range of cells immediately to the right of your current data range. 

<img alt="" class="wp-image-64960" src="https://www.inciter.io/wp-content/uploads/2020/04/Step-5-1024x358.png"/>
6. **Highlight the new range** with your cursor. Press **Enter**.

<img alt="" class="wp-image-64961" src="https://www.inciter.io/wp-content/uploads/2020/04/Method-1-End-Result.png"/>
7. Click **Finish**. Your resulting data should look like this.

#### Method \#2: Flash Fill

Lets take a look at an example that appears to be a bit more complex. Here, not only do we have our names in one cell, but we have them in the format: (1) surname, (2) a comma and (3) first name. While its absolutely possible to pull off transforming these using Text to Column, Flash Fill is simple and flexible. Flash Fill fills a series without a formula. You type how you want your data in the adjacent cell to look, Excel notices a trend in your data entry, and then continues that pattern for you. 

<img alt="" class="wp-image-64963" src="https://www.inciter.io/wp-content/uploads/2020/04/Method-2-Image-1.1.png"/>
1. In the column next to the range youd like to change, **type** the donors first name in the first two rows. You need to type **two entries** so Excel can recognize that youre creating a pattern. 

**2. Highlight the range** in the column where youve typed your new values. Under the **Data** tab, click the **fill function**, and select **Flash Fill** from the dropdown menu.

<img alt="" class="wp-image-64964" height="344" src="https://www.inciter.io/wp-content/uploads/2020/04/Method-2-Image-2-1024x641.png" width="550"/>

<img alt="" class="wp-image-64965" src="https://www.inciter.io/wp-content/uploads/2020/04/Method-2-Image-3.png"/>
3. **Repeat **steps 1 and 2 for your Last Name column.

Thats it! You might already be able to think of some more functions for Flash Fill. This would work just the same if our donors had a middle initial, a title such as Mrs. before or ,Ph.D. after their name, as long as we type enough values, and type values for special cases, to show Excel our trends.

Its pretty intuitive, so dont be afraid to experiment with some new patterns. Just be sure to only apply Flash Fill to adjacent cells, and repeat your trend to show Excel what you want. 

Stay tuned for Parts 3 and 4:  

Part 3: Combining data from multiple cells into one column  
Part 4: Even more time-saving applications for Flash Fill

We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io)



