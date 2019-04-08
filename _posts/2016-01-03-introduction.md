---
layout: post
title: NYC MTA Turnstile Entry Volume Analysis
---



### PREMISE

This analysis project was a team project to determine where a company should place its street teams to best find potential donors to their cause. WomenTechWomenYes(WTWY), a tech company with an initiative to gain support for more female representation in the tech industry, wished to utilize data analytics to answer this question, and it was left up to our team to think up a solution.


-----

### DATA


We used the [NYC MTA turnstile data](http://web.mta.info/developers/turnstile.html) to conduct our analysis. Since WTWY were deploying their teams during the beginning of Summer, we focused specifically on data taken from May during the years of 2016, 2017, and 2018. By isolating each turnstile and grouping by stations, we were able to isolate the stations with the highest foot traffic across this time period.


Once we had pulled all of the data that we needed from MTA, we explored and noticed certain key aspects that were important to keep note of for future analyses. We also encountered issues with the data that we had to further identify and clean…


* Turnstiles count entries in a cumulative fashion, usually counting up
* Turnstiles were also able to count down, leading to negative # of entries
* Entries were taken at regular 4 hour intervals, although there were certainly some that were recorded at random time intervals
* After taking the daily entries for each turnstile, there were some clear outliers present, which were removed in our analysis

To get to our final entry tally, we removed our “problem” data mentioned above, and grouped our data first by station, and then by day of the week and time of the day. Our goal for this was to identify the best likely place, day, and time for WTWY to send their teams out.


-----


### RESULTS


The following graph shows the top 5 busiest stations according to the results of our aggregate analysis:


![Top 5](https://github.com/Baddy2shoes/Baddy2Shoes.github.io/blob/master/images/top5.png?raw=true)


Since we wanted to focus in on weekday and time as well, the following graph shows the cumulative entries for our top 5 stations, further split up by weekdays:


![Weekdays](https://github.com/Baddy2shoes/Baddy2Shoes.github.io/blob/master/images/weekdays.png)

It seems that the bulk of traffic going into the stations happens in the middle of the week, concentrated on Tuesday, Wednesday, and Thursday, with Monday occasionally showing up with high traffic as well.

Now to further concentrate our efforts, we looked at time series data for entries for our top stations as well:

![Time of Day](https://github.com/Baddy2shoes/Baddy2Shoes.github.io/blob/master/images/timeofday.png?raw=true)

The bulk of traffic, as expected of a busy city like New York, is centered around the lunch rush, and the end of the day, when all the commuters are heading home. The most entry by volume happens from 12pm to 9pm.

To conclude, our team recommended WTWY to place their teams at Penn Station, Grand Central, Union Square, 34ST Herald, and 23ST, focusing on Tuesday through Thursday (and Monday and Friday as well if funding permits) during 12pm to 9pm.



-----

