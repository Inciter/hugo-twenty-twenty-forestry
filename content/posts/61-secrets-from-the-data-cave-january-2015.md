
---
wp_id: 1818
wp_post_status: "publish" 
title: "Secrets from the Data Cave: January 2015"
date: 2015-01-26T17:45:42+05:00
date_modified: 2020-04-30T15:25:35+05:00
date_published: 2015-01-26T17:45:42+05:00
primary_category: "Technology And Customer Service"
categories: ['Technology And Customer Service'] 
tags: ['security', '2014', 'conferences']
seo_title: "secrets from the data cave: january 2015"
seo_meta_description: ""
summary: ""
featured_image_url: "no image"
slug: "secrets-from-the-data-cave-january-2015"
url: "https://www.inciter.io/secrets-from-the-data-cave-january-2015/"
authors: CRC
---

#Content

By: [Sarah](https://www.inciter.io/who/crc-data-nerds/sarah/)
---
&nbsp;
<p style="text-align: center;">&nbsp;<em>Welcome to CRC’s monthly series of articles on all things techie: Secrets from the Data Cave! (For those who don’t know, the title references our room — fondly referred to as “the bat cave”— where data staff can geek out in an isolated setting.) Here we’ll be offering you a sneak peek into the cave, with tips and the latest updates on what we’re implementing here at CRC.</em></p>
<p style="text-align: center;"><em><span style="color: #ff9900;">(This month's SDC is an on-the-road edition!)</span></em></p>
&nbsp;
&nbsp;
Late last fall, I had the opportunity to go to <a href="http://world.phparch.com" rel="noopener noreferrer" target="_blank">phpworld 2014</a>, a conference for PHP code developers, held in Washington DC.
&nbsp;
Many different web applications use the programming language PHP, so coders have a myriad of options for deploying it (including, but not limited to, Drupal, Wordpress, Joomla, and Magneto). This&nbsp;conference is designed to bring these communities together in order for developers to learn about how others are using this language, and get ideas for enhancing existing applications.
&nbsp;
The conference sessions that fascinated me the most were those about web security. PHP is great for developers because it is a very powerful language, meaning you can do a lot with it. But, without the proper precautions, hackers can exploit that power over your applications and cause huge headaches.
&nbsp;
&nbsp;
One conference presenter gave a great example of how this might look in the real world. As context for the example, you need to know that there are certain combinations of coding language that, should a hacker type them into your application and you haven’t protected your database, the application will interpret them as legitimate SQL code and “drop” all the tables in your database. Therefore a hacker could use this technique (called “SQL injection”) with a “drop database table” command – feeding the application some code that masquerades as part of the original developer’s code— to irreversibly erase all of your data.
&nbsp;
&nbsp;
_With this in mind, consider the presenter’s example:_
A would-be hacker in Europe rigged up a fake license plate with a bit of SQL injection code on it. He was exploiting the fact that traffic cameras use picture-parsing technology to break down an image of a license plate into individual characters (to record the plate info of speeders).
&nbsp;
&nbsp;
So, this was presumably an effort to trick the traffic camera into parsing the code, feeding the data in as it would any license plate. This would have ultimately caused all the stored traffic data on the back-end to be wiped clean via the SQL injection! Now, it’s unlikely that this actually worked in practice. But, it did get me thinking about the lengths hackers will go to in order to mess with your data.
&nbsp;
&nbsp;
All in all, it__&nbsp;__was an excellent conference, and I feel I learned a lot about this powerful coding language. I’m now looking forward to connecting with more PHP developers in future!

