---
title: "Spatial Analysis of ridership by Census Tracts and Stations"
date: 2020-12-21
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Spatial Analysis of ridership by Census Tracts and Stations"
altair-loader:
  altair-chart-1: "charts/Top10_Ridership_pre.json"
  altair-chart-2: "charts/Top10_Ridership_post.json"
hv-loader:
  hv-chart-1: ["charts/PreCovid_CensusRidership.html", "500"] # second argument is the height
  hv-chart-2: ["charts/PostCovid_CensusRidership.html", "500"] # second argument is the height
  hv-chart-3: ["charts/PreCovid_CensusDruation.html", "500"] # second argument is the height
  hv-chart-4: ["charts/PostCovid_CensusDruation.html", "500"] # second argument is the height
toc: true
toc_sticky: true
---

In this post, we analysis the ridership with geographic locations. Census tracts and stations will be used for this analysis. 

# Ridership by Census tract 

Below are the comparsion of ridership by census tracts. As we mentioned in previous post, the total ridership decreases after Covid. Also, San Francisco sets up more bike sharing stations in 2020, with 258 stations totally. In 2019, only 237 stations in San Francisco. Here you can see more census tracts have ridership now. 

Another thing to notice is that each trip is located by ending station. In other words, these two graphic shows the ridership of census tracts as destinations. We can see that financial district and San Francisco downtown area are the most welcome destinations for bike trips. After Covid, some census tracts near San Francisco Golden Gate parks and Twin peaks area are becoming more popular for bike trips. 

<div id="hv-chart-1"></div>
<div id="hv-chart-2"></div>

# Trip Duration by census tract

Another important element is trip duration. Which census tract as a destination can have the longer trip duration? 

Below is the comparison graphics. It is interesting to see that those west area have higher trip duration. One of the main reasons is that majority of the bike stations are locted in east of the city. In this case, people may take longer trip to get to those east areas, such as Golden Gate Parks. However, after Covid, it looks like southeast areas have longer trip duration. Those previous census tracts that have long durations are witnessing a decline in trip duration. 

<div id="hv-chart-3"></div>
<div id="hv-chart-4"></div>

# Ridership by Bike Stations

Now we understand the ridership by census tract. How about each bike station? Which station has higher ridership? As we mentioned above, city has established more bike stations in 2020. Below are two maps showing the ridership by stations. 

Before Covid, most of high ridership statios are located in and near downtown San Francisco.
    station ID 30 "San Francisco Caltrain (Townsend St at 4th St)", 
    Station ID 21 "Montgomery St BART Station (Market St at 2nd St)" ,
    Station ID 15 "San Francisco Ferry Building (Harry Bridges Plaza)" 
are the top three destinations for biking.These locations are all related to public and regional transportation. Normally, people use bikes to get to those public transportation locations. 

After Covid, people are tend to bike to other places in the city instead of downtown and financial district. Some stations in the west and central city are seeing an increase ridership. 
    station ID 58 "Market St at 10th St"
    station ID 3 "Powell St BART Station (Market St at 4th St)"
    station ID 377 "Fell St at Stanyan St"
are the top three ddestinations for biking. While most of them are still related to public transportation, it is interesting to see Station 377 which is near Golden State Park. People are more willing to go to the regional parks after COVID. Also, you can see the stations in financial district have lower ridership after COVID mostly because of the working from home.   

PreCovid ridership by station
![PreCovid ridership by station]({{ site.url }}{{ site.baseurl }}/assets/images/PreCovid ridership by station.png)

PostCovid ridership by station
![PostCovid ridership by station]({{ site.url }}{{ site.baseurl }}/assets/images/PostCovid ridership by station.png)

<div id="altair-chart-1"></div>
<div id="altair-chart-2"></div>


**Important: When embedding charts, you will likely need to adjust the width/height of the charts before embedding them in the page so they fit nicely when embedded.**
