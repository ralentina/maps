---
layout: post
title: Atlas del Litoral Central&#58; floating population (doughnuts)

date: 2021-06-09 11:49:00
tags:
  - pie charts
  - Litoral Central
  - Chile
  - ArcMap
  - Census
  - Matplotlib
  - Python
excerpt: An alternative way to represent the floating population on the Litoral Central, in this case highlighting its size in relation to permanent residents.

---

A few weeks ago, I used a <a href="{{ '/coastal_floating_pop' | absolute_url }}">dot-density map</a> to represent the increase in population caused by tourism in the Litoral Central. This map is based on the same data, but uses doughnut charts. I'm well aware that <a href='https://www.mit.edu/~mbarker/formula1/f1help/11-ch-c6.htm' target="_blank">doughnut charts</a> are essentially pie charts, and that pie charts are the pariah of information design and data visualisation. But what can I say? I'm a rebel.


<figure class="align-center">
  <img src="{{ '/img/pobFlot_donuts.jpg' | absolute_url }}" alt="">
  <figcaption>
	 Permanent and floating population in the southern Litoral Central
	</figcaption>
</figure>

A few notes on the workflow. First, I used ArcMap to represent my data, using proportional pie charts (the pie size depends on the absolute sum of permanent urban population according to the census plus monthly floating population as estimated by SERNATUR). For some reason, when exporting my map the circles were pixelated. Since I have been playing around with <a href="https://matplotlib.org/" target='_blank'>Matplotlib</a>, I decided to use it to make new charts to add on my map. Here I was able to modify the design into doughnut charts, which, I hear, are very, very slightly cooler. I admit I was intimidated by figuring out how to scale the radius of the doughnuts to make their surface proportional to the data, so I based myself on the original ArcMap charts and used Illustrator.