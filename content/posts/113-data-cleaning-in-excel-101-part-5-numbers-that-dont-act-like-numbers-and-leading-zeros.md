
---
wp_id: 65022
wp_post_status: "draft" 
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
featured_image_url: /wp-content/uploads/2020/05/Puzzle-Pieces-Stock-Photo.jpeg
slug: "data-cleaning-in-excel-101-part-5-numbers-that-dont-act-like-numbers-and-leading-zeros"
url: "/data-cleaning-in-excel-101-part-5-numbers-that-dont-act-like-numbers-and-leading-zeros/"
authors: Jacob Joseph
---

#Content



Ever try to do a calculation with numbers in Excel and get an error or the numbers don't seem to be adding up? Ever fight with ZIP code formatting? Below you can find some methods of dealing with numbers that just aren't acting like numbers. Well also review some instances in which youll actually _want_ Excel to store numbers as text, and how to convert them.

This is Part 5 in our Data Cleaning in Excel 101 series. [Part 1](https://www.inciter.io/data-cleaning-in-excel-101-part-1/) showed methods of removing blank rows from your data. [Part 2](https://www.inciter.io/data-cleaning-in-excel-101-part-2-splitting-up-cell-contents-into-multiple-columns/) focuses on splitting data from one cell to multiple cells. [Part 3](https://www.inciter.io/data-cleaning-in-excel-101-part-3-combining-data-from-multiple-columns/) covers the opposite: combining data from multiple columns into one column. In [Part 4](https://www.inciter.io/data-cleaning-in-excel-101-part-4-more-uses-for-flash-fill/), we discussed some incredibly useful and time-saving tricks with Excels Flash Fill function.

### Numbers that don't act like numbers

Spreadsheets are all about storing numerical data and making calculations. But what do you do if numbers arent acting like numbers and Excel is preventing you from doing even basic calculations?

<img alt="example of SUM formula not working for two numbers" class="wp-image-65024" src="https://www.inciter.io/wp-content/uploads/2020/05/image13.png"/><figcaption>This happens when numbers are stored as text. A good way to tell that Excel is storing numbers as text is checking how the numbers are aligned. Excel left-aligns text and right-aligns numbers. Often, the error is a result of an export from another system that doesnt encode the numbers correctly. There are a few ways to fix this issue.</figcaption>

#### Method 1: Convert to Number

<img alt="yellow triangle error message" class="wp-image-65026" src="https://www.inciter.io/wp-content/uploads/2020/05/image16.png"/>
1. Notice the little green triangle at the top left corner of the cell. When you select the cell, it will show you a yellow triangle warning.

<img alt="Error options after click" class="wp-image-65027" src="https://www.inciter.io/wp-content/uploads/2020/05/image6.png"/>
2. When you click the yellow triangle warning, the specific error or warning message will be shown. In this case, Number Stored as Text.

<img alt="results of convert to number" class="wp-image-65029" src="https://www.inciter.io/wp-content/uploads/2020/05/image9.png"/>
3. If you select the Convert to Number option, it will change the format of the cell and allow math to work on the number.

<img alt="highlight to convert multiple" class="wp-image-65032" src="https://www.inciter.io/wp-content/uploads/2020/05/image18.png"/>
4. Uh oh 5 + 25 does not equal 5, but you dont have to convert each cell separately. You can highlight multiple cells with the green triangle and convert them at the same time.

<img alt="all numbers converted correctly" class="wp-image-65033" src="https://www.inciter.io/wp-content/uploads/2020/05/image7.png"/>
5. Okay, that looks like its working!

Theres one additional trick with this method. You wont see the error option to Convert to Number on cells that are already numbers. So you always have to start your highlighting from a cell that has the error, but then you can Convert to Number, and it will not alter cells that are already numbers.

#### Method 2: Convert with basic arithmetic (+, -, \*, /)

In some cases you may have a large data set but only some of the numbers are stored as text. You dont want to hunt through each row to look for the ones that need to be converted. To convert them quickly, you can use basic arithmetic operations like addition, subtraction, multiplication, and division which automatically convert cells to numbers if they are not already numbers.

The great thing about this method is that it works faster than the Convert to Number and you dont have to find the little green triangles which are good at hiding in large data sets.

<img alt="using +0 and *1 to convert text to number" class="wp-image-65034" src="https://www.inciter.io/wp-content/uploads/2020/05/image4.png"/>
1. In this case you can use +0 or *1 to make the conversion.

<img alt="copy and paste as values menu" class="wp-image-65036" src="https://www.inciter.io/wp-content/uploads/2020/05/image17-1-1024x841.png"/>
2. If youd like to replace the original values that were causing you issues, then you can highlight the new numbers, copy them and use paste special as values on top of the originals.

#### Method 3: Remove leading or trailing characters

Sometimes numbers include spaces, letters, or symbols before or after your numbers. Unwanted characters can be removed with a few handy formulas called TRIM, LEFT, RIGHT, and LEN.

*   **TRIM** - removes leading and trailing spaces from a cell
*   **LEFT** - extracts a certain number of characters from a cell starting from the left
*   **RIGHT** - extracts a certain number of characters from a cell starting from the right
*   **LEN** - gives the length of a cell (number of characters like letters, numbers, and symbols)

In the examples below, notice that only the first row shows the green triangle that will allow you to use the Convert to Number feature.

So how do you convert the rest of them?

You can use a combination of the above formulas with the 0+ from the previous method.

<img alt="=0+TRIM(A1)
=0+LEFT(A2, LEN(A2)-1)
=0+RIGHT(A3, LEN(A3)-5)
=0+LEFT(RIGHT(A4, LEN(A4)-1),LEN(A4)-1-5)" class="wp-image-65037" src="https://www.inciter.io/wp-content/uploads/2020/05/image19-1024x268.png"/>

*   **ROW 1** - The number looks okay at first glance, but it actually has 2 spaces before and after the number like \[space\]\[space\]30\[space\]\[space\]. You can use the TRIM formula to remove unwanted leading and trailing spaces from a cell.
*   **ROW 2** - The LEFT formula can be combined with LEN to get the whole value of the cell except the last character. Because there is only one unwanted symbol (\#), then you only need to subtract 1. If there were 2 unwanted characters (\#\#) at the end, then you could say -2 instead of -1.
*   **ROW 3** - This works the same as the LEFT formula in ROW 2 except it starts counting from the right side of the cell.
*   **ROW 4** - In this example both are combined to remove both a prefix and a suffix from a formula. Notice that the RIGHT formula only subtracts 1 from the LEN, but the LEFT formula subtracts both 1 and 5. (After the RIGHT formula produces a result it is already 1 shorter than the original LEN.)

### Leading Zeros

Now you know how to convert text to numbers, but in some cases, you may actually NOT want numbers to act like numbers. You may want the numbers to act like text.

A very common example of when leading zeros are necessary is with ZIP codes. Several ZIP codes in the northeastern US start with zeros. If you open a CSV file in Excel, it will usually remove leading zeros. There are 3 great ways to correct this issue so Excel will show the correct ZIP code.

#### Method 1: TEXT formula

Here's an example of how to use the TEXT formula.

<img alt='=TEXT(a2, "00000")' class="wp-image-65038" src="https://www.inciter.io/wp-content/uploads/2020/05/image20-1024x176.png"/><figcaption>The 00000 tells the TEXT formula to format as text that is 5 digits long and adds leading zeros if they arent present. So the 2383 turns into 02383 and the 21201 appears unaffected.</figcaption>

The TEXT formula converts any numbers that you give it into text, so notice our little green triangles showing up again. You can no longer use formulas with math calculations, and in the case of ZIP codes, thats not a problem.

There are plenty of other format codes available besides just 00000 which can be [found in the Excel documentation here](https://www.google.com/url?q=https://support.office.com/en-us/article/number-format-codes-5026bbd6-04bc-48cd-bf33-80f18b4eae68&sa=D&ust=1589561311889000).

#### Method 2: Custom format

If you want to keep the number stored as a number or want to avoid using a formula. You can use custom formatting for cells to make the numbers show up exactly how you want.

<img alt="right click &gt; format cells" class="wp-image-65039" src="https://www.inciter.io/wp-content/uploads/2020/05/image22.png"/>

<img alt="custom format options" class="wp-image-65041" src="https://www.inciter.io/wp-content/uploads/2020/05/image11-1024x965.png"/>
.

<img alt='enter "00000" as custom format' class="wp-image-65042" src="https://www.inciter.io/wp-content/uploads/2020/05/image14-1024x975.png"/>
.

<img alt="corrected zip codes" class="wp-image-65043" src="https://www.inciter.io/wp-content/uploads/2020/05/image2.png"/>
.

#### Method 3: Open CSV into Excel and preserve leading zeros

The last option can be useful when opening a large CSV file with lots of potential leading zero issues is using the Data Import feature. Its great because you dont have to change formatting and copy and paste a lot of values.

1. Open a blank workbook or worksheet where you want the data to go.

<img alt='Data tab then "From Text"' class="wp-image-65044" src="https://www.inciter.io/wp-content/uploads/2020/05/image8.png"/>
2. On the Excel ribbon at the top, select the Data tab and then select From Text.

<img alt="open file dialog" class="wp-image-65045" src="https://www.inciter.io/wp-content/uploads/2020/05/image10-1024x673.png"/>
.

<img alt="text import wizard &gt; Step 1: data type" class="wp-image-65046" src="https://www.inciter.io/wp-content/uploads/2020/05/image21-1024x776.png"/>
4. A wizard will walk you through the import steps. The first question is the Data Type (either Delimited or Fixed width). For CSV files select delimited, then click Next.

<img alt="text import wizard &gt; Step 2: delimiter" class="wp-image-65047" src="https://www.inciter.io/wp-content/uploads/2020/05/image5-1024x785.png"/>
5. The next step asks you what characters are used as delimiters. For CSV files, you can usually select Comma and not change any other options, then click Next.

<img alt="text import wizard &gt; Step 3: column data format preview" class="wp-image-65048" src="https://www.inciter.io/wp-content/uploads/2020/05/image3-1024x776.png"/>
6. The last step asks you about formatting. This is the key step for preventing any formatting issues. Select a column in the preview pane and change the options to match how you want the numbers to be treated.

<img alt="text import wizard &gt; Step 3: column data format preview with type changed to text" class="wp-image-65049" src="https://www.inciter.io/wp-content/uploads/2020/05/image12-1024x773.png"/>
7. In this case, we want the quantity to be treated like a number, so we leave it as General, but we want ZIP codes to be treated like text, so we selected the first column then the Text option.

<img alt="Where do you want to put the data dialog" class="wp-image-65050" src="https://www.inciter.io/wp-content/uploads/2020/05/image1-1.png"/>
8. When you click Finish, Excel will ask you where you want the data to go (in a new sheet or in an existing sheet). You can usually just click OK.

<img alt="imported data in cells formatted correctly" class="wp-image-65052" src="https://www.inciter.io/wp-content/uploads/2020/05/image15-1.png"/>
9. Now your data is imported with the leading zeros on your ZIP codes!

We encourage you to try out these examples and let us know if you have any questions. We hope these methods help you as you clean your data! Please let us know if there are other topics or data cleaning problems you would like us to tackle by emailing [contact@inciter.io](mailto:contact@inciter.io).



