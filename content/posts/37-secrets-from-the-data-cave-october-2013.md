
---
wp_id: 712
wp_post_status: "draft" 
title: "Secrets from the Data Cave, October 2013"
date: 2013-10-29T10:38:56+05:00
date_modified: 2018-10-29T13:51:47+05:00
date_published: 2013-10-29T10:38:56+05:00
primary_category: "Uncategorized"
categories: ['Uncategorized'] 
seo_title: "secrets from the data cave, october 2013"
seo_meta_description: ""
summary: "" 
slug: "secrets-from-the-data-cave-october-2013"
url: "/secrets-from-the-data-cave-october-2013/"
authors: CRC
---

#Content

# _**Introducing. . . Secrets from the Data Cave**_

_by Sarah McCruden _

<div>
<i>Welcome to CRCs new monthly series of articles on all things techie: **Secrets from the Data Cave**! For those who dont know, the title references the room in our office where the data staff can geek out in an isolated setting that is fondly referred to as the bat cave. We will be offering you a sneak peek into this fascinating environment every month with the latest updates and tips on what were implementing here in the CRC data cave!</i>

**October 2013: Beware the Pumpkin Pie**

Stephen Fews <i>[Show Me the Numbers: Designing Tables and Graphs to Enlighten](http://www.amazon.com/Show-Me-Numbers-Designing-Enlighten/dp/0970601999).</i> This volume, basically a textbook, covers more info on data visualization than one could hope to fit into a blog, and is worth reading in its entirety if you get the chance. It is Fews breakdown on how the human brain processes raw sensory data from visual stimuliand why that matters when youre deciding between a pie chart or a bar graphthat has really changed the way I look at data (pun intended)! So, I wanted to share this with our readers in this first-ever **Secrets from the Data Cave**.
1</sup>) on Americans chosen Halloween costumes. Per this survey, the top Halloween costume choices for children (as represented by surveyed parents who had already decided on a costume) were:
<img alt="1_table" class="aligncenter size-medium wp-image-714" height="300" src="https://www.inciter.io/wp-content/uploads/2013/10/1_table-251x300.jpg" width="251"/>

So how would you represent these findings in chart or graph form? Often, the go-to choice for data like this is a pie chart. Heres what that might look like:

<img alt="2_piechart" class="aligncenter size-medium wp-image-715" height="300" src="https://www.inciter.io/wp-content/uploads/2013/10/2_piechart-346x300.jpg" width="346"/>

2</sup>that is, to communicate the size of the piece, relative to the whole. Yet this has a fatal flaw were not very good at estimating the comparative sizes of 2D areas like the slices of the pie above, so without labels to tell us the numeric and/or percent values for each category, the pie chart is going to fall short in communicating numbers that are close in value (i.e., the number of Pumpkins vs. Vampires vs. Ninjas).
much</i> bigger/smaller each piece is than the one before? This is tough, to say the least. Yet if we look at the same data in bar graph form, the rank and approximate values are much more easily discerned:

<img alt="3_barchart" class="aligncenter size-medium wp-image-716" height="300" src="https://www.inciter.io/wp-content/uploads/2013/10/3_barchart-470x300.jpg" width="470"/>

2</sup> Preattentive attributes will draw our attention to certain aspects of any visual stimuli: the form (length, width, orientation, shape, size and enclosure); the color (hue and intensity); and the spatial position.<sup>3</sup> We can exploit these preattentive attributes when designing charts and graphs to focus the viewers attention on the most important aspects of the data (in this case, the length of the bars in the bar graph, which represent the numeric value of each costume).
does</i> use spatial position to encode information, it uses their 2D <i>size</i>**,** as opposed to their 2D <i>position</i> (an example of data encoded with 2D position would be a scatter plot, where the location of the dots relative to one another represents the data). And when it comes to 2D size in pie charts, even though we can tell that one value is greater than another when we use width, size, or color intensity, these attributes do not indicate precisely how much a value differs., it is difficult to perceive by how much or to assign a value to the area.<sup>2</sup> And this doesnt just apply to pie charts, (which one could argue are harder to read because they dont have a labeled horizontal axis), are problematic. Any comparison of area will be more challenging than the comparisons of length one would see in a bar graph. 
should</i> we use to encode our data? According to Few, we get the maximum perceptual benefits when we rely on length and 2D position of objects for quantitative data by using:
*   Points,
*   Lines,
*   Bars, and
*   Boxes

Examples of these would be our bar graph of costume choices above, as well as the examples from Fews book below:
<img alt="data_blog_ex" class="aligncenter size-full wp-image-893" height="183" src="https://www.inciter.io/wp-content/uploads/2013/10/data_blog_ex.jpg" width="276"/>
All of the above choices would make it much easier to see the differences in how many child Pumpkins and child Ninjas we can expect to see trick-or-treating this year.
bars </i>would be a much better choice.
Happy Halloween everyone!</strong>

_**Sources:**_

<li><span style="color: #333333;">National Retail Federation. (Oct 7, 2013). <i>Traditional Costumes Favorites For Adults, Children This Halloween, According To NRF </i>[data file]. Retrieved from [http://www.nrf.com/modules.php?name=Documents&op=viewlive&sp_id=7682](http://www.nrf.com/modules.php?name=Documents&op=viewlive&sp_id=7682)</li>
<li>Few, Stephen (2012). <i>Show Me The Numbers: Designing Tables and Graphs To Enlighten, </i>Second Edition<i>. </i>Burlingame, CA: Analytics Press.</li>
<li>Ware, Colin (2004). <i>Information Visualization: Perception for Design, </i>Second Edition. San Francisco, CA: Morgan Kaufmann. </li>

