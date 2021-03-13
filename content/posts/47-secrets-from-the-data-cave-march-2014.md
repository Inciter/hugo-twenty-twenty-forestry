
---
wp_id: 1267
wp_post_status: "draft" 
title: "Secrets from the Data Cave: March 2014"
date: 2014-03-27T12:46:58+05:00
date_modified: 2014-03-27T13:03:53+05:00
date_published: 2014-03-27T12:46:58+05:00
primary_category: "Dataviz"
categories: ['Dataviz'] 
tags: ['communciation', 'data visualization']
seo_title: "secrets from the data cave: march 2014"
seo_meta_description: ""
summary: "" 
slug: "secrets-from-the-data-cave-march-2014"
url: "/secrets-from-the-data-cave-march-2014/"
authors: CRC
---

#Content

_by Sarah McCruden_

<i>Welcome to CRCs monthly series of articles on all things techie: **Secrets from the Data Cave**! (For those who dont know, the title references our room  fondly referred to as the bat cave where data staff can geek out in an isolated setting.) Here well be offering you a fascinating sneak peek into the cave, with the latest updates & tips on what were implementing here at CRC!</i>

**March 2014: I Am Going to S P A C E**

<img alt="1280px-Galaxy_history_revealed_by_the_Hubble_Space_Telescope_(GOODS-ERS2)" class="aligncenter wp-image-1268" height="271" src="https://www.inciter.io/wp-content/uploads/2014/03/1280px-Galaxy_history_revealed_by_the_Hubble_Space_Telescope_GOODS-ERS2-1024x452.jpg" width="614"/>

Earlier this month, while looking for some new and interesting data visualizations, I came across this nifty [website that gives a spatial representation of the distance between planets in our solar system](http://joshworth.com/dev/pixelspace/pixelspace_solarsystem.html)<sup>1</sup>. After thoroughly enjoying the learning experience (along with the witty interjections, as I patiently scrolled though the empty space signifying millions of miles), I visited the creators blog page, where he explained his motivation to undertake this project:

I kept trying to describe the distance using metaphors like if the earth was the size of a golf ball, then Mars would be across the soccer field etc., but I realized I didnt really know much about these distances, besides the fact that they were really large and hard to understand. Pictures in books, planetarium models, even telescopes are pretty misleading when it comes to judging just how big the universe can be. _**Are we doing ourselves a disservice by ignoring all the emptiness? **_<sup>2, (emphasis mine)</sup>

It got me thinking: we put a premium on space use in data visualization when it comes to things like BI dashboards, infographics, or even paper reports. We typically want our data spread across as few pages as possible, so that we can process related information simply by shifting our gaze, as opposed to shuffling/scrolling through multiple pages. We might also want to see the same data represented as numbers in a table _and_ as a chart or graph, so it makes sense to try and squeeze multiple representations of the same data onto one page.

But the question remains: as convenient as it is to see _everything at once_ without scrolling across a screen, what do we lose in impact when we choose to condense large datasets into small visual representations? Even when we keep those representations relatively true to scale, how much is lost?

Take, as another example, epidemiological data on different countries AIDS-related deaths in 2001 and 2011 (UNAIDS<sup>3</sup>). This dataset has been condensed to include a few example countries:

<img alt="aids_datatable" class="aligncenter size-full wp-image-1272" height="175" src="https://www.inciter.io/wp-content/uploads/2014/03/aids_datatable.jpg" width="528"/>

<img alt="aids_datachart" class="aligncenter size-full wp-image-1274" height="215" src="https://www.inciter.io/wp-content/uploads/2014/03/aids_datachart.jpg" width="444"/> 

The graph generally conveys the message that AIDS-related deaths in Kenya have dropped substantially in the last 10 years, while the number of such deaths remained about the same in the USA and United Kingdom, and that Kenya has many more deaths, overall, than the other two countries. But its still very difficult to wrap ones mind around the magnitude of so many deaths just from the chart above.

For that reason, I created an alternative visualization of Kenyas 130,000 estimated AIDS deaths in 2001 that, like the outer space example, involves a lot of scrolling. You can find it as a PDF <span style="color: #ff6600;">[here](https://www.dropbox.com/s/jm1v9bja5m8w5ry/Kenya_AIDSDeaths2001.pdf).

Now, I live in the real world. I get that we all need to consider limitations on space when creating data visualizations, especially when they will be printed. (Save some trees!) I also recognize that comparing sizes using the scrolling model is difficult because we can only hold so much precise measurement in our memory once it is out of our line of sight. This is why I only included data for one country and one year, rather than comparing all three in one visualization. But, my point remains that condensing as a visualization strategy does not always make comprehending data easier, especially when very large numbers are involved. There is something to be said for a visual representation of data that takes up a lot of space, when the data it represents is larger than life. And for that reason, going forward I plan to space my data visualizations out as much as I can, whenever possible and applicable.

Do any of our readers have any input on this topic? Leave a comment and let us know!

_Sources:_

1.   [http://joshworth.com/dev/pixelspace/pixelspace\_solarsystem.html](http://joshworth.com/dev/pixelspace/pixelspace_solarsystem.html)
2.   <http://www.joshworth.com/a-tediously-accurate-map-of-the-solar-system/>
3.   [http://www.unaids.org/en/media/unaids/contentassets/documents/epidemiology/2012/gr2012/20121120\_UNAIDS\_Global\_Report\_2012\_with\_annexes\_en.pdf](http://www.unaids.org/en/media/unaids/contentassets/documents/epidemiology/2012/gr2012/20121120_UNAIDS_Global_Report_2012_with_annexes_en.pdf)

 

