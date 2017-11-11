---
layout: post
title:  "Examination 1"
date:   2017-11-06 03:53:09 -0500
categories: jekyll update
---
# Examination Questions:

1. What do you think of pre-compiling your CSS?  
*Compare to regular CSS  
*Which techniques did you use?  
*Pros and cons?  

2. What do you think of static site generators?  
*What type of projects are they suitable for?

3. What is robots.txt and how have you configure it for your site?

4. What is humans.txt and how have you configure it for your site?

5. How did you implements comments to blog posts?

6. What is Open Graph and how do you make use of it?


# Examination Answers:

1. I haven't worked much with CSS, but from the little experience I have, I'd say that
pre-compiling CSS code makes a lot of sense.  
By doing so I can create variables to hold various values. I can reuse these in different ways. I can create what could be considered CSS functions, which saves time, probably enhances performance, and compresses the code.  
In regular CSS I will have to write the same thing several times. By pre-compiling, I still
have to write the same thing several times, but I can for example use a preordained variable.
This allows me to, in the end, write less code.

>For this webpage I created some variables, I made two mixins, I created a variable for a background-image etc. I have been trying to understand how it works, and I feel now that I grasp the basic concept, surrounding preprocessors(or atleast SASS), quite adequately (even if I still hardly know nothing). 

2. SSG's are new to me, as is basically the whole environment of creating websites. Even so, from what I've understood, an SSG will be more stable than many other kinds of websites.  
The need for bandwidth is for example not as great as that of other kinds of site generators. It is also more safe, as it doesn't have as many functions which could be exploited by malware and hackers.

    SSG's seem like a valid option for sites which need to prioritize stability, and which are primarily information based. With this I mean, that if a site I build doesn't have the need for complex apps etc. but rather just seeks to inform about for example a program, and the budget of the project is small, then an SSG might be the way to go.  
    For a larger project, which also wants to portray a certain image, then something a bit more "fancy" might seem more attractive.

3. Robots are a kind of script which searches webpages on the internet for various information.  
A robots.txt provides information for these robots. It tells them which parts of the site they can scan for information etc.  
A robot doesn't have to adhere to what the robots.txt says though, which is common with "Bad robots". So the robots.txt mainly serves a purpose in telling law-abiding robots what they are allowed and not allowed to do on the webpage in question.

4. Humans.txt is a document in which various information about the webpage project, and mainly the people behind it, is presented. One can give credit to the various people who have been involved, also specifying _how_ they have been involved.  
It is a good tool for example in the regard that if someone like the webpage, and would like to come into contact with the creators, they can do so by help from the humans.txt.

5. I used Disqus to implement a way to comment on blogposts. It was pretty straightforward.  First I registered(on the Disqus webpage) a name for the site(utvecklingavmjukvara).  After this I implemented a JS-script which the Disqus webpage provided me with a link to. I pasted this into the minima/_include folder's disqus_comments.html, and included the following command at the end of each blog post:  
include disqus_comments.html  
It worked as intended.

6. Open Graph is a protocol which gives the developer the possibility to share links in a way that is, to the developer, considered appropriate.  
It allows the developer to design the output of the link, so that the image and text presented represents what the link itself is about. For example:  
A link, that if you click on it, leads to a webpage about trekking in himalaya, might show up in the feed of a social media program as a picture of Himalayan mountains, and with a short text that says something like: "Trekking in Himalaya".  
This could give the person recieving the link more of an incitament to actually decide whether the link might be of interest or not. Thus making it easier to decide whether to click on it or not.  
It is put to use trough an HTML implementation.


{% include disqus_comments.html %}
