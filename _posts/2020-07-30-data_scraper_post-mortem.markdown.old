---
layout: post
title:      "Data Scraper Post-Mortem or How I Learned To Be Humble and just Code"
date:       2020-07-30 18:35:34 -0400
permalink:  data_scraper_post-mortem
---


Looking back at the beginning of my journey when I first decided that I wanted to reach out and plumb the depths of data science, I didn't think it would start by being defeated by simple HTML and Table tags. It happened though! My first, and blatantly easy, task that I had assigned myself was building a webscraper that would scrape movie information, so that I could practice my *exploratory data analysis* skills on. Unfortunately, my eyes were bigger than my stomach (to borrow an old idiom), and my technical abilities at the time were not up to snuff to build this. Here I am though, and I want to break down this little scraper so that I can learn a thing or two in the process.

### The Mission

Build a simple webscraper in Python. It would take in a webpage that I had drawn the URL from using a simple python package for the BoxOfficeMojo API. The scraper would then scrape all of the relevant financial data about the movie and return it in a neat `CSV` file. This `CSV` file would be the first victim... I mean subject of my admittedly less than surgical fledgling EDA skills at the time. This data would then be openly shared to all of my classmates that wished to partake in the particular dataset that I had built. Admittedly, at the time it was a lot about pride, accomplishment, and a little bravado - having some from a slightly more technical background in Computer Science than it seemed the rest of the cohort had come from. 

### The Journey and the Destination

I had finished the READMEs and the labs early enough that I had a few days to spare on the first module before we were actually engaged to begin the project. Instead of sitting back, studying more, and taking my time to let the new ideas sink into my thick-skull I decided that I would start this data scraper in order to show off a little and to help the classmates out with some data that they might otherwise struggle to get themselves. 

The first day I mostly played around with the recommend library for the task,` BeautifulSoup`. `BeautifulSoup` for those uninitiated is an infinitely useful library that essentially turns webpages into a soup of tags, anchors, and elements that can then be searched in a clear and idiomatic way. Did I find this helpful? No! Of course not, why would I want to take the time to learn the correct way when I could do something the hacky, fast way? Isn't that the programmer's ethos? "Hack first, ask questions later. If it works, it works." Or any other of the infinitely many silly phrases that we tell ourselves when our 2AM code runs with no errors, but in the light of day we are too afraid to look. That digression aside, I found `lxml`.

`lxml` is an indispensable library. It is the fastest parser that you can use, being very close to `C time` in speed. It can break down `xml` documents with relative ease, and can allow you to pull out the information you want. A second use is parsing webpages and pulling content from them. You see, elements in a webpage have something call an `XPath` and this `XPath` is, more or less, like a file directory that allows you to reference straight to that elements on the webpage - if it exists. Now, I wouldn't have added that last part had it not been important. `XML` files are very rigid things that are structured in a purposeful way and rarely change internally. Webpages, unfortunately for me, are something that as web tech has advanced have become increasingly more dynamic. Even the most basic of websites have some dynamic element to them. Enter the downfall of my short, sweet, ever-so hacky webscraper.

I was able to successfully pull many elements from these pages that I wanted. It was wonderful and I felt very satisfied with myself as I sat back and watched as my little, brittle minion crawled these webpages and stashed the information for later consumption. What I didn't know, at the time though, was that the dynamism of webages would lead to my particularly un-Pythonic and un-Programmatic script to break. After several thousand iterations of movies stored and actual time spent my little minion hit snag. This gave me my first experiences with Python error handling. Error handling is a breeze in Python, I quickly learned. The high level nature of the language makes everything so convenient and this isn't any different. After a handful of attempts I was able to design some error handling situations that benefited my code greatly. However, I had not considered that these errors were happening for specific reasons. 

One sleep later, and now its the third day of **Operation Build This Scraper** (working title). I had left the script to run overnight and gather what information it had been directed to. Gather it did, but upon further inspection I found several inconsistencies. Certain columns in the dataset had data that didn't make sense, and this is where webpage dynamism comes in. My script had the errors handled, and that led to it picking up the wrong data if the correct data wasn't there. It made *data cleaning* and even more arduous task than it was going to be from the beginning. I spent the remainder of those 8 hours trying to reconcile this discovery. Spoiler alert, and for those who aren't familiar with post-mortems, I never worked it into a shape I was truly happy with.

I spent all of this time on a silly script that scraped twenty-something thousand movie entries of which, in the end, I only ended up using slightly over eight thousand. It was a moment of defeat. More importantly though, it was a moment of learning. 

### The Lessons Learned

* Pride is a sin, and cockiness is an insidious killer (of code).

* Brittle code is not only un-Pythonic, but its un-programmatic. Those things also kill code.

* Use the right tool for the job!

* Even moments of defeat should be celebrated. Failure is an opportunity to learn!

I haven't ventured back to revisit my silly, little scraper but I plan to one day soon. I would like to conquer my first real coding challenge as a data science inductee.
