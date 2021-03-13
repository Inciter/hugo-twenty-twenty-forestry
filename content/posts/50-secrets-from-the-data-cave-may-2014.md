
---
wp_id: 1295
wp_post_status: "draft" 
title: "Secrets from the Data Cave, May 2014"
date: 2014-06-09T11:48:52+05:00
date_modified: 2014-06-09T11:51:06+05:00
date_published: 2014-06-09T11:48:52+05:00
primary_category: "Uncategorized"
categories: ['Uncategorized'] 
tags: ['process', 'tools', 'organization', 'stakeholder use', 'data']
seo_title: "secrets from the data cave, may 2014"
seo_meta_description: ""
summary: "" 
slug: "secrets-from-the-data-cave-may-2014"
url: "/secrets-from-the-data-cave-may-2014/"
authors: CRC
---

#Content

_by Sarah McCruden_

<i>Welcome to CRCs monthly series of articles on all things techie: **Secrets from the Data Cave**! (For those who dont know, the title references our room  fondly referred to as the bat cave where data staff can geek out in an isolated setting.) Here well be offering you a fascinating sneak peek into the cave, with the latest updates & tips on what were implementing here at CRC!</i>

**May 2014:  The Difficult Database, Part 1: _The Data Monster_**
        In my experience working with relational databases, Ive seen it all: the good, the bad, and the _very_ ugly in data-keeping practices.  Ive learned a lot about wrangling data in an unruly database. While plenty of problems I see are caused by a complicated combination of elements and require time-consuming fixes, sometimes the issues are simple and could be addressed relatively quickly and painlessly by program directors or database managers. Over the next few months I will review a few of these common problems, what might be causing them, and how I would address them in a mini-series of posts regarding The Difficult Database.

This month, Ill talk about a very serious problem plaguing organizations everywhere . . . THE DATA MONSTER!

[caption id="attachment_1296" align="alignleft" width="226"]

<img alt="The Data Monster, as portrayed for Ashley Faherty circa 2009. Ms. Faherty kept the sketch as a reminder of the trouble the Monster can cause. Note: Not drawn to scale." class="size-full wp-image-1296" height="286" src="https://www.inciter.io/wp-content/uploads/2014/06/datamonster.jpg" width="226"/>

 The Data Monster, as portrayed for Ashley Faherty circa 2009. Ms. Faherty kept the sketch as a reminder of the trouble the Monster can cause. _Not drawn to scale._[/caption]

<span style="line-height: 1.5em;">The Data Monster is a seldom-seen creature that sneaks into your database/case notes/paper records under cover of night and eats all the data. Youll know you have a Data Monster if, when it comes time to pull a report out of your database, many of the records for your clients/patients/students are mysteriously missing. You <i style="line-height: 1.5em;">know </i>the work was done, and the efforts of your team should be reflected in your reportso where did the data go? The Data Monster ate it. That is to say, you have no idea where it went and why its not on the report. So you suffer from:

**<span style="text-decoration: underline;">The Common Problem**: **No data/incomplete data in your database and on your reports, or inexplicably low participant counts for some measures.**

**<span style="text-decoration: underline;">Possible Cause(s) and Ways to Address Them****:**

 <span style="text-decoration: underline;"> 1. Records are not being entered by program staff at all

If you suspect that entire records are not being entered AT ALL (so, for example, someone filled out an intake questionnaire on paper for Suzie Q., who is enrolling in your Workforce Development program, but now months down the line Suzy Q. doesnt have an intake in the database at all), here are some things to consider:

*   _Are you setting your database fields to required for too many answers on a very long form_? While this may seem like a good way to _prevent_ incomplete data, this can actually backfire if used excessively. It requires program and data entry staff to enter every single field all in one sitting before they can submit the form (and Ive seen forms with hundreds of fields to be completed, which could take hours to enter). When a form like this meets program staff who already have a full day of tasks to complete, its easy to see why data entry for something that will eat up such a large chunk of time might get put off until later, which unfortunately can translate into _much_ later, or never, because there is a continuous stream of new records coming in that will also require entry. Even if staff have the option to save part-way through the entry process and return later to enter the rest, youre likely to get a lot of saved partially-completed forms that will never make it to submission/completion, which is only slightly better than not having them entered at all.
*   _I would suggest_: Think about what should REALLY be required on that form, and adjust your field settings accordingly. First and last name? Most likely need that information completed. Mothers maiden name? Probably not something you should require. Yes, in a perfect world, every field would be completed every time, and there are likely certain things that funders ask you to collect, but you need to think about the bare minimum of necessary information, and make those the required fields. That way, at the very least you will have _some_ data to show on those participants, as opposed to none when their data is never entered, or their form is never completed and submitted.

  2. Records for a participant are in the database, but the fields you need for data aggregation are blank/incorrect

Sometimes participants will have a record, but wont show up where they are supposed to/dont have the correct values filled in for certain fields are not being entered (so Suzie Q., who is enrolling in your Workforce Development program, has an intake form, but things that should be filled in are blank or wrong), here are some things to consider:

*   _Are the data entry staff the same as the data collectors themselves? If not, is there an understanding between the two of how certain values should be entered? _While some programs are set up such that the same person who would collect the data on paper would enter it into the database, many rely on designated data entry staff to do the electronic entry component. As someone who started out as a Data Entry Specialist, I have seen many cases where the person who filled out the paper form would leave a field blank, either because they were doing some type of task that involved them being quick in their observation/note taking (for example, observing motor skills in young children, who will not perform on command), or because it was not applicable and/or the correct value was assumed to be common sense or obvious. As a data entry professional, I entered things exactly as they appeared on the paper, especially since I did entry for a lot of standardized tests on which I wasnt qualified to assume anything. Ideally one would ask for clarification if something is blank, but that is not always an option, especially if the person who completed the form is very busy. Thus, you might end up with blank fields in your database because, for example, the person completing the form left a field blank and assumed it would be filled in during entry, but it wasnt.
*   _I would suggest_: The best way to deal with this is to have a meeting between those who complete the fields on paper and those who do the entry, and agree upon what is to be entered when a field is left blank. If there are exceptions to the rule, they need to be explicitly stated because ultimately, though you might want people to just use common sense in their entry, you also wouldnt want them to assume something in error and cause the wrong value to be entered into your database. Communication is key to resolving this issue.

*   _Does your form and/or database contain items with forced-choice values that are too close in meaning?_ If you have a drop-down menu in your database, or multiple choice item on a form, where two or more values are too close in meaning, you may end up with some program staff choosing one option, while others choose a different one, in cases where the value should be the same. For example, if your questionnaire asks what type of government assistance a participant receives, and you have one option for Utility Assistance and one for Water Bill Assistance, some program staff might assume that water is a utility and thus belongs under utility assistance. Then, when it comes time to get your total number of participants receiving assistance on their water bill, your count for Water Bill Assistance will be lower than it should be because some are counted in the Utility Assistance total instead. This is more often a problem when there are many options to choose from (Ive seen databases with over 100 choices for a single item).
*   _I would suggest_: Either generate a list for program staff that spells out which values should be used for which responses, or remove some of the options/change things so that they cannot be confused anymore (for example, you could change Utility Assistance to Gas/Electric Assistance, so that program staff know that it doesnt refer to the water bill). Do keep in mind, though, that no matter what you do to fix this issue going forward, you old data may still have errors caused by the initial confusion, and you would need to be mindful of that when crafting your report.

**Hopefully, armed with the above suggestions, you can tackle some of the issues you might be experiencing with your database, and that pesky DATA MONSTER will leave you alone once and for all!**

 

