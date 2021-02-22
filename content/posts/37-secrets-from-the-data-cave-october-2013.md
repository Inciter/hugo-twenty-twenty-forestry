
---
wp_id: 712
wp_post_status: "publish" 
title: "Secrets from the Data Cave, October 2013"
date: 2013-10-29T10:38:56+05:00
date_modified: 2018-10-29T13:51:47+05:00
date_published: 2013-10-29T10:38:56+05:00
primary_category: "Uncategorized"
categories: ['Uncategorized'] 
tags: ['']
seo_title: "secrets from the data cave, october 2013"
seo_meta_description: ""
summary: ""
featured_image_url: "no image"
slug: "secrets-from-the-data-cave-october-2013"
url: "https://www.inciter.io/secrets-from-the-data-cave-october-2013/"
authors: CRC
---

#Content

<h1 align="center"><em><strong>Introducing. . . Secrets from the Data Cave</strong></em></h1>
<span style="color: #888888;">_by Sarah McCruden&nbsp;_</span>
<div>
<p><span style="color: #888888;"><i>Welcome to CRC’s new monthly series of articles on all things techie: <b>Secrets from the Data Cave</b>! For those who don’t know, the title references the room in our office where the data staff can geek out in an isolated setting that is fondly referred to as “the bat cave.” We will be offering you a sneak peek into this fascinating environment every month with the latest updates and tips on what we’re implementing here in the CRC data cave!</i></span></p>
</div>
<div style="text-align: center;"><span style="color: #ff6600; font-size: large;"><b>October 2013: Beware the Pumpkin Pie</b></span></div>
<div style="text-align: left;">
<p>This month’s topic— how to effectively represent data based on basic principles of visual perception, as discussed in <a href="http://www.amazon.com/Show-Me-Numbers-Designing-Enlighten/dp/0970601999" target="_blank">Stephen Few’s </a><i><a href="http://www.amazon.com/Show-Me-Numbers-Designing-Enlighten/dp/0970601999" target="_blank">Show Me the Numbers: Designing Tables and Graphs to Enlighten</a>.</i>&nbsp;This volume, basically a textbook, covers more info on data visualization than one could hope to fit into a blog, and is worth reading in its entirety if you get the chance. It is Few’s breakdown on how the human brain processes raw sensory data from visual stimuli—and why that matters when you’re deciding between a pie chart or a bar graph—that has really changed the way I look at data (pun intended)! So, I wanted to share this with our readers in this first-ever <b>Secrets from the Data Cave</b>.</p>
<p>In the “spirit” of the season, I’ll be using data from a 2013 consumer survey (National Retail Federation<sup>1</sup>) on Americans’ chosen Halloween costumes. Per this survey, the top Halloween costume choices for children (as represented by surveyed parents who had already decided on a costume) were:</p>
<p>&nbsp;</p>
<p>So how would you represent these findings in chart or graph form? Often, the go-to choice for data like this is a pie chart. Here’s what that might look like:</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>The pie chart, a familiar graphic for anyone in research, is used to “encode values in an assortment of 2D shapes that represent values in proportion to their area”<sup>2</sup>—that is, to communicate the size of the piece, relative to the whole. Yet this has a fatal flaw— we’re not very good at estimating the comparative sizes of 2D areas like the slices of the “pie” above, so without labels to tell us the numeric and/or percent values for each category, the pie chart is going to fall short in communicating numbers that are close in value (i.e., the number of Pumpkins vs. Vampires vs. Ninjas).</p>
<p>See for yourself: Can you rank the pieces from largest to smallest, without cheating and looking at the table above? And even if you can get the rank correct, can you tell how <i>much</i> bigger/smaller each piece is than the one before? This is tough, to say the least. Yet if we look at the same data in bar graph form, the rank and approximate values are much more easily discerned:</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>This difference in perception lies in preattentive processing, which “occurs below the level of consciousness at an extremely high speed and is tuned to detect a specific set of visual attributes.”<sup>2</sup> Preattentive attributes will draw our attention to certain aspects of any visual stimuli: the form (length, width, orientation, shape, size and enclosure); the color (hue and intensity); and the spatial position.<sup>3</sup> We can exploit these preattentive attributes when designing charts and graphs to focus the viewers’ attention on the most important aspects of the data (in this case, the length of the bars in the bar graph, which represent the numeric value of each costume).</p>
<p>While the pie graph <i>does</i> use spatial position to encode information, it uses their 2D <i>size</i><b>,</b> as opposed to their 2D <i>position</i> (an example of data encoded with 2D position would be a scatter plot, where the location of the dots relative to one another represents the data). And when it comes to 2D size in pie charts, “even though we can tell that one value is greater than another when we use width, size, or color intensity, these attributes do not indicate precisely how much a value differs…., it is difficult to perceive by how much or to assign a value to the area.”<sup>2</sup> And this doesn’t just apply to pie charts, (which one could argue are harder to read because they don’t have a labeled horizontal axis), are problematic. Any comparison of area will be more challenging than the comparisons of length one would see in a bar graph.&nbsp;</p>
<p>So what <i>should</i> we use to encode our data? According to Few, we get the maximum perceptual benefits when we rely on length and 2D position of objects for quantitative data by using:</p>
<ul>
<li>Points,</li>
<li>Lines,</li>
<li>Bars, and</li>
<li>Boxes</li>
</ul>
<p>Examples of these would be our bar graph of costume choices above, as well as the examples from Few’s book below:</p>
<p>All of the above choices would make it much easier to see the differences in how many child Pumpkins and child Ninjas we can expect to see trick-or-treating this year.</p>
<p>So the moral of the story is: Beware the Pumpkin pie! Pumpkin <i>bars </i>would be a much better choice.</p>
<p><strong><span style="color: #ff6600;">Happy Halloween everyone!</span></strong></p>
<p>&nbsp;</p>
<p><span style="color: #333333;"><em><b>Sources:</b></em></span></p>
<ol>
<li><span style="color: #888888;"><span style="color: #333333;">National Retail Federation. (Oct 7, 2013). <i>Traditional Costumes Favorites For Adults, Children This Halloween, According To NRF </i>[data file]. Retrieved from</span>&nbsp;</span><a href="http://www.nrf.com/modules.php?name=Documents&amp;op=viewlive&amp;sp_id=7682" target="_blank">http://www.nrf.com/modules.php?name=Documents&amp;op=viewlive&amp;sp_id=7682</a></li>
<li>Few, Stephen (2012). <i>Show Me The Numbers: Designing Tables and Graphs To Enlighten, </i>Second Edition<i>. </i>Burlingame, CA: Analytics Press.</li>
<li>Ware, Colin (2004). <i>Information Visualization: Perception for Design, </i>Second Edition. San Francisco, CA: Morgan Kaufmann.&nbsp;</li>
</ol></div>

