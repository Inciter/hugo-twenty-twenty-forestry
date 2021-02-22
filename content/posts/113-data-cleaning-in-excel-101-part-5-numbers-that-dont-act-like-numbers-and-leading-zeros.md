
---
wp_id: 65022
wp_post_status: "publish" 
title: "Data Cleaning in Excel 101, Part 5: Numbers That Don't Act Like Numbers and Leading Zeros"
date: 2020-05-18T10:55:33+05:00
date_modified: 2020-05-20T11:53:28+05:00
date_published: 2020-05-18T10:55:33+05:00
primary_category: "Data Management And Databases"
categories: ['Data Management And Databases'] 
tags: ['data', 'excel']
seo_title: "data cleaning in excel 101, part 5: numbers that don't act like numbers and leading zeros"
seo_meta_description: ""
summary: ""
featured_image_url: "https://www.inciter.io/wp-content/uploads/2020/05/Puzzle-Pieces-Stock-Photo.jpeg"
slug: "data-cleaning-in-excel-101-part-5-numbers-that-dont-act-like-numbers-and-leading-zeros"
url: "https://www.inciter.io/data-cleaning-in-excel-101-part-5-numbers-that-dont-act-like-numbers-and-leading-zeros/"
authors: Jacob Joseph
---

#Content



Ever try to do a calculation with numbers in Excel and get an error or the numbers don't seem to be adding up? Ever fight with ZIP code formatting? Below you can find some methods of dealing with numbers that just aren't acting like numbers. We’ll also review some instances in which you’ll actually _want_ Excel to store numbers as text, and how to convert them.
This is Part 5 in our Data Cleaning in Excel 101 series. [Part 1](https://www.inciter.io/data-cleaning-in-excel-101-part-1/) showed methods of removing blank rows from your data. [Part 2](https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/) focuses on splitting data from one cell to multiple cells. [Part 3](https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/) covers the opposite: combining data from multiple columns into one column. In [Part 4](https://www.inciter.io/data-cleaning-in-excel-101-part-4-more-uses-for-flash-fill/), we discussed some incredibly useful and time-saving tricks with Excel’s “Flash Fill” function.
### Numbers that don't act like numbers

Spreadsheets are all about storing numerical data and making calculations. But what do you do if numbers aren’t acting like numbers and Excel is preventing you from doing even basic calculations?
#### Method 1: Convert to Number

<ol><li>Notice the little green triangle at the top left corner of the cell. When you select the cell, it will show you a yellow triangle warning.</li></ol>
<p>2. When you click the yellow triangle warning, the specific error or warning message will be shown. In this case, “Number Stored as Text”.</p>
<p>3. If you select the “Convert to Number” option, it will change the format of the cell and allow math to work on the number.</p>
<p>4. Uh oh… 5 + 25 does not equal 5, but you don’t have to convert each cell separately. You can highlight multiple cells with the green triangle and convert them at the same time.</p>
<p>5. Okay, that looks like it’s working!</p>

There’s one additional trick with this method. You won’t see the error option to Convert to Number on cells that are already numbers. So you always have to start your highlighting from a cell that has the error, but then you can Convert to Number, and it will not alter cells that are already numbers.
#### Method 2: Convert with basic arithmetic (+, -, \*, /)
In some cases you may have a large data set but only some of the numbers are stored as text. You don’t want to hunt through each row to look for the ones that need to be converted. To convert them quickly, you can use basic arithmetic operations like addition, subtraction, multiplication, and division which automatically convert cells to numbers if they are not already numbers.
The great thing about this method is that it works faster than the Convert to Number and you don’t have to find the little green triangles which are good at hiding in large data sets.

<p>1. In this case you can use +0 or *1 to make the conversion.</p>
<p>2. If you’d like to replace the original values that were causing you issues, then you can highlight the new numbers, copy them and use paste special as values on top of the originals.</p>

#### Method 3: Remove leading or trailing characters
Sometimes numbers include spaces, letters, or symbols before or after your numbers. Unwanted characters can be removed with a few handy formulas called TRIM, LEFT, RIGHT, and LEN.
*   __TRIM__ - removes leading and trailing spaces from a cell
*   __LEFT__ - extracts a certain number of characters from a cell starting from the left
*   __RIGHT__ - extracts a certain number of characters from a cell starting from the right
*   __LEN__ - gives the length of a cell (number of characters like letters, numbers, and symbols)
In the examples below, notice that only the first row shows the green triangle that will allow you to use the Convert to Number feature.
So how do you convert the rest of them?
You can use a combination of the above formulas with the 0+ from the previous method.
<img alt="=0+TRIM(A1)
=0+LEFT(A2, LEN(A2)-1)
=0+RIGHT(A3, LEN(A3)-5)
=0+LEFT(RIGHT(A4, LEN(A4)-1),LEN(A4)-1-5)" class="wp-image-65037" src="https://www.inciter.io/wp-content/uploads/2020/05/image19-1024x268.png"/></figure>

*   __ROW 1__ - The number looks okay at first glance, but it actually has 2 spaces before and after the number like \[space\]\[space\]30\[space\]\[space\]. You can use the TRIM formula to remove unwanted leading and trailing spaces from a cell.
*   __ROW 2__ - The LEFT formula can be combined with LEN to get the whole value of the cell except the last character. Because there is only one unwanted symbol (\#), then you only need to subtract 1. If there were 2 unwanted characters (\#\#) at the end, then you could say -2 instead of -1.
*   __ROW 3__ - This works the same as the LEFT formula in ROW 2 except it starts counting from the right side of the cell.
*   __ROW 4__ - In this example both are combined to remove both a prefix and a suffix from a formula. Notice that the RIGHT formula only subtracts 1 from the LEN, but the LEFT formula subtracts both 1 and 5. (After the RIGHT formula produces a result it is already 1 shorter than the original LEN.)
### Leading Zeros
Now you know how to convert text to numbers, but in some cases, you may actually NOT want numbers to act like numbers. You may want the numbers to act like text.
A very common example of when leading zeros are necessary is with ZIP codes. Several ZIP codes in the northeastern US start with zeros. If you open a CSV file in Excel, it will usually remove leading zeros. There are 3 great ways to correct this issue so Excel will show the correct ZIP code.
#### Method 1: TEXT formula
Here's an example of how to use the TEXT formula.
The TEXT formula converts any numbers that you give it into text, so notice our little green triangles showing up again. You can no longer use formulas with math calculations, and in the case of ZIP codes, that’s not a problem.
There are plenty of other format codes available besides just “00000” which can be [found in the Excel documentation here](https://www.google.com/url?q=https://support.office.com/en-us/article/number-format-codes-5026bbd6-04bc-48cd-bf33-80f18b4eae68&amp;sa=D&amp;ust=1589561311889000).
#### Method 2: Custom format

If you want to keep the number stored as a number or want to avoid using a formula. You can use custom formatting for cells to make the numbers show up exactly how you want.

<p>1. Highlight the cells you want to reformat and right click to select “Format Cells…”<img alt="" src="images/image22.png"/></p>
<p>2. On the Number tab, select Custom<img alt="" src="images/image11.png"/>.</p>
<p>3. Then enter 00000 where it defaults to “General”<img alt="" src="images/image14.png"/>.</p>
<p>4. Now the ZIP code will show with the proper leading zeros<img alt="" src="images/image2.png"/>.</p>

#### Method 3: Open CSV into Excel and preserve leading zeros
The last option can be useful when opening a large CSV file with lots of potential leading zero issues is using the Data Import feature. It’s great because you don’t have to change formatting and copy and paste a lot of values.
1. Open a blank workbook or worksheet where you want the data to go.

<p>2. On the Excel ribbon at the top, select the Data tab and then select “From Text”.</p>
<p>3. Select the CSV file that you want to import<img alt="" src="images/image10.png"/>.</p>
<p>4. A wizard will walk you through the import steps. The first question is the Data Type (either Delimited or Fixed width). For CSV files select delimited, then click Next.</p>
<p>5. The next step asks you what characters are used as delimiters. For CSV files, you can usually select Comma and not change any other options, then click Next.</p>
<p>6. The last step asks you about formatting. This is the key step for preventing any formatting issues. Select a column in the preview pane and change the options to match how you want the numbers to be treated.</p>
<p>7. In this case, we want the quantity to be treated like a number, so we leave it as General, but we want ZIP codes to be treated like text, so we selected the first column then the Text option.</p>
<p>8. When you click Finish, Excel will ask you where you want the data to go (in a new sheet or in an existing sheet). You can usually just click OK.</p>
<p>9. Now your data is imported with the leading zeros on your ZIP codes!</p>

<p class="has-normal-font-size">We encourage you to try out these examples and let us know if you have any questions.&nbsp;We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing <a href="mailto:contact@inciter.io">contact@inciter.io</a>.</p>


