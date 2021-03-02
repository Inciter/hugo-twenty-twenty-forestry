
---
wp_id: 65083
wp_post_status: "draft" 
title: "Data Cleaning in Excel 101, Part 7: Managing Blank Cells"
date: 2020-06-02T10:05:37+05:00
date_modified: 2020-06-02T10:05:41+05:00
date_published: 2020-06-02T10:05:37+05:00
primary_category: "Data Management And Databases"
categories: ['Data Management And Databases'] 
tags: ['excel', 'data']
seo_title: "data cleaning in excel 101, part 7: managing blank cells"
seo_meta_description: ""
summary: "" 
featured_image_url: /wp-content/uploads/2020/05/Missing-Piece.jpg
slug: "data-cleaning-in-excel-101-part-7-managing-blank-cells"
url: "/data-cleaning-in-excel-101-part-7-managing-blank-cells/"
authors: Kristen Halsey
---

#Content



In this part of our data cleaning series, well be focusing on managing blank cells. There isnt a singular approach to handling blank cells in your dataset. Because there are numerous reasons why a cell might be blank, context is key when determining how to fill them. Sometimes, youll need to fill every blank cell in your data with the same constant. Other times, youll pick up clues as to what should be there from the surrounding data.

This is Part 7 in our Data Cleaning in Excel 101 series. [Part 1](https://www.inciter.io/data-cleaning-in-excel-101-part-1/) showed methods of removing blank rows from your data. [Part 2](https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/) focuses on splitting data from one cell to multiple cells. [Part 3](https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/) covers the opposite: combining data from multiple columns into one column. In [Part 4](https://www.inciter.io/data-cleaning-in-excel-101-part-4-more-uses-for-flash-fill/), we discussed some incredibly useful and time-saving tricks with Excels Flash Fill function. [Part 5](https://www.inciter.io/data-cleaning-in-excel-101-part-5-numbers-that-dont-act-like-numbers-and-leading-zeros/) covers solutions for when your numbers arent acting like numbers. [Part 6](https://www.inciter.io/data-cleaning-in-excel-101-part-6-removing-duplicates/) showed methods for removing duplicate entries.

Us data folks frequently work with incomplete datasets as we wait for data to be delivered. In our work, we typically have access to some pieces of data, but arent able to get everything we need until data collection is complete or until its all been authorized for our use. In these situations, its wise to keep a placeholder to indicate that the cell is blank for a reason.

### Method 1: Filling Blanks With a Constant

Well start with an easy example to illustrate when you would fill all blank cells the same, and how to go about doing so efficiently in Excel. Lets say were analyzing scores from a training course with three modules. In this case, we know that these blanks indicate the participant was not present during the time of an exam, but they can take the exam at a later date. We dont want to mistake these blank cells for zeroes, as this could seriously affect any short-term analysis results and our understanding of the data.

<img alt="" class="wp-image-65084" height="121" src="https://www.inciter.io/wp-content/uploads/2020/05/Training-Module-Dataset.png" width="348"/>

<img alt="" class="wp-image-65085" src="https://www.inciter.io/wp-content/uploads/2020/05/Find-and-Select.png"/>
1. Highlight all of your data and click the Find & Select function in the ribbon under the Home tab.
1. Select "Go To Special"

3. In the window that appears, select blanks, then OK.

Excel will select all of your empty cells in your dataset. The first white cell is your active cell. All of the gray cells are going to be filled with what you choose to write in the active cell. In our case, we will call these cells Absent.

4. At this stage, type "Absent".

<img alt="" class="wp-image-65086" height="187" src="https://www.inciter.io/wp-content/uploads/2020/05/Filling-Blank-Cells-1.png" width="326"/>

5. Lastly, use the keyboard shortcut Control + Enter to fill all selected cells.

<img alt="" class="wp-image-65087" height="121" src="https://www.inciter.io/wp-content/uploads/2020/05/Filling-Blank-Cells-2.png" width="337"/>

### Method 2: Filling Blanks With Values from Above

Now, lets look at an example of a scenario in which you know what should go into each blank cell because the surrounding data provides context. Here, in this training course example, we have each course date and instructor listed, with course scores for each chapter.

<img alt="" class="wp-image-65088" height="201" src="https://www.inciter.io/wp-content/uploads/2020/05/Course-Dataset-2-1024x613.png" width="336"/>

Our problem is that we know each instructor teaches and quizzes the participants on 3 chapters, but due to faulty data entry, we have blanks in our date and instructor columns. The values we do have are acting as headers. We know that the date 2/15/20 and instructor Maria Brown should be in the first 3 rows, and so on throughout the end of the course.

One way to blank cells with the value immediately above is to highlight the cells and use the keyboard shortcut Control + D. But, to execute this, we would have to still do some manual work. See here:

<img alt="" class="wp-image-65089" height="171" src="https://www.inciter.io/wp-content/uploads/2020/05/Control-D.png" width="213"/>

We would have to go through each small section, highlighting values and use Control + D repeatedly. In this case, its not a huge effort, but imagine using this method on a large dataset. It would be time consuming with a great potential for errors.

The method well use this time is similar to the previous function. Only this time, well tell Excel we want blank cells to be filled with the values from the cell above. Repeat the first three steps from the previous method:

1.   Highlight all of your data and click the Find & Select function in the ribbon under the Home tab. 
2.   Select Go To Special. 
3.   In the window that appears, select blanks, then OK.

Now, well use a formula instead of typing a value.

4. Type the = sign on your keyboard.  
5. Click the up arrow on your keyboard.

<img alt="" class="wp-image-65090" src="https://www.inciter.io/wp-content/uploads/2020/05/A2.png"/>
Now, youll see that the formula is changed to =A2. Well fill all of the selected blanks with that formula.

6. Just as we did before, press the Control key and tap Enter.

<img alt="" class="wp-image-65091" height="171" src="https://www.inciter.io/wp-content/uploads/2020/05/Last-Image-Filled-Set-1024x642.png" width="274"/>

We want to change the formulas to values so we can move things around, or make modifications to our data without having the values change. We can copy and paste our cells in the same place to modify formatting.

7. Copy and paste all of your cells.   
8. Open the clipboard icon and select paste as Values Only.

<img alt="" class="wp-image-65092" height="165" src="https://www.inciter.io/wp-content/uploads/2020/05/Paste-Values-Only.png" width="230"/>

No more blanks! We hope these methods help you as you clean your data!

We encourage you to try out these out and let us know if you have any questions. Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io).



