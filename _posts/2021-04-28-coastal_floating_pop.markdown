---
layout: post
title: Atlas del Litoral Central&#58; floating population (dot-density)

date: 2021-04-28 11:49:00
tags:
  - dot-density
  - Litoral Central
  - Chile
  - ArcGIS
  - Census
excerpt: A first attempt to visualise the impact of tourism on population distribution on the Litoral Central (plus some design experimentation).

---

Approximately 24,000 people live in Cartagena, the coastal town on which my research focuses. Being a major tourist destination for Santiago residents, however, its population swells during summer weekends (up to 300,000 according to municipality sources). Since vulnerability indexes typically use population data from the Census, they overlook this floating population.

I'm interested in how to represent it cartographically. A first idea is to through a color-coded dot-density map. To quantify the floating population I used a ponderated means by SERNATUR, i.e. the estimated number of travels per year divided by 12. This is not ideal, since tourists do not distribute evenly over the year. I'm now thinking of using a series of such maps representing changes over the year, based on estimates of touristic flows by month, maybe accompanied by little line graphs. 

<figure class="align-center">
  <img src="{{ '/img/population_flotante-01.jpg' | absolute_url }}" alt="">
  <figcaption>
	 Permanent and floating population in the southern Litoral Central
	</figcaption>
</figure>

For now, I took this opportunity to work on a solid design that could be used in longer map series on the Litoral Central. Below is an alternative version and some previous design tests. While I like the 1970s vibe of the sea pattern in this variation, I'm afraid it may make viewers dizzy, especially when repeated in many maps. 

<figure class="align-center">
  <img src="{{ '/img/population_flotante-alt.jpg' | absolute_url }}" alt="">
  <figcaption>
	 Permanent and floating population in the southern Litoral Central (design variation)
	</figcaption>
</figure>

<figure class="align-center">
  <img src="{{ '/img/population_flotante_design-tests.jpg' | absolute_url }}" alt="">
  <figcaption>
	 'Behind the scenes' design tests
	</figcaption>
</figure>
