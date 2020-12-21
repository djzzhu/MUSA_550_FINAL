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

This post will show examples of embedding interactive charts produced using [Altair](https://altair-viz.github.io) and [Hvplot](https://hvplot.pyviz.org/).

## Altair Example

Below is a chart of the incidence of measles since 1928 for the 50 US states.

This was produced using Altair and embedded in this static web page. Note that you can also display Python code on this page:


## HvPlot Example

Lastly, the measles incidence produced using the HvPlot package:

<div id="hv-chart-1"></div>
<div id="hv-chart-2"></div>
<div id="hv-chart-3"></div>
<div id="hv-chart-4"></div>

PreCovid ridership by station
![PreCovid ridership by station]({{ site.url }}{{ site.baseurl }}/assets/images/PreCovid ridership by station.png)

PostCovid ridership by station
![PostCovid ridership by station]({{ site.url }}{{ site.baseurl }}/assets/images/PostCovid ridership by station.png)

<div id="altair-chart-1"></div>
<div id="altair-chart-2"></div>


**Important: When embedding charts, you will likely need to adjust the width/height of the charts before embedding them in the page so they fit nicely when embedded.**
