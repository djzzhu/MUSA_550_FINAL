---
title: "Compare ridership by hours, day, month(Pre and Post Covid)."
date: 2020-12-21
published: true
tags: [dataviz, matplotlib]
excerpt: "Compare ridership by hours, day, month(Pre and Post Covid)."
altair-loader:
  altair-chart-1: "charts/PreCovid_DaybyHours.json"
  altair-chart-2: "charts/PostCovid_DaybyHours.json"
  altair-chart-3: "charts/bike2019_ridership.json"
  altair-chart-4: "charts/bike2020_ridership.json"
toc: true
toc_sticky: true
read_time: false
---

# Compare ridership by day of week 

Different days of week can affect the ridership in transportation. Normally, we can say during workdays, cities may see higher ridership. Here we perform an analysis to find out the ridership changes between PreCovid and PostCovid. The March 17th is the date that San Francisco offically announced the Lockdown. And we use this date to determine the time Covid-19 happened. Although the original dataset has no day of week, we assign each starting time to specific day of week. Below are two diagrams showing this interesting comparision.

Here we find out that before Covid, workdays,especially Tuesday and Thursday, have higher bike ridership compared with weekends. After Covid, it is interesting to see that Weekends have higher ridership than weekdays. Saturday now has the highest ridership during the week. 

![PreLockdown Ridership_ dayofweek]({{ site.url }}{{ site.baseurl }}/assets/images/PreLockdown Ridership_ dayofweek.png)
![PostLockdown Ridership_ dayofweek]({{ site.url }}{{ site.baseurl }}/assets/images/PostLockdown Ridership_ dayofweek.png)

# Compare ridership by Hours

The original datasets have starting time that includes the hours. We slice this data and assign a specific category to these hours. 
     1. Daytime 10am -16pm
     2. rush hourA  6am - 10 am
     3. rush hourB  16pm - 19pm
     4. evening   19pm - 23pm
     5. others   23pm-6am

Below are the two graphics showing the comparsion. Before Covid, rush hour bike ridership has the highest number. After Covid, we can a dramatic decrease in those rushhour ridership, while daytime bike ridership increases a lot. 

<div id="altair-chart-1"></div>
<div id="altair-chart-2"></div>

# Compare ridership by Month 

Now we have seen the ridership changes by hours and days. How about each month? 2019 vs 2020? Here we have another comparison. 

Firstly, the total ridership decreases in 2020. In 2019, March, April, July and October have the highest ridership among all the months. In 2020, January, Febuary and October have the highest ridership. We can see a dramatic decline in March 2020 when Covid hit. And another decline in November when the second wave comes again in CA and entire U.S.
<div id="altair-chart-3"></div>
<div id="altair-chart-4"></div>
