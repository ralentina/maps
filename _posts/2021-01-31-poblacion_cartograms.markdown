---
layout: post
title: Where does the population of Chile lives?
date: 2021-01-30 11:49:00
tags:
  - QGIS
  - cartogram
  - Chile
  - Census
  - infographic
excerpt: Four graphics answering this burning question (cartograms).
---

Famously, Chile is a very long, <a href="https://www.penguinrandomhouse.com/books/189554/travels-in-a-thin-country-by-sara-wheeler/">thin country</a>, with all regions lined up one after the other from North to South. It occured to me that such a shape would lend itself to cartograms! Regions are numbered progressively from top to bottom (with a few 'jumps' for regions that have been created later on), hence the numbers on the maps.  

As attribute data, I have used the population by region according to the 2017 census. There were just under 19 million people living in Chile, of which over 7 in the Región Metropolitana de Santiago, as the fat 'bellies' in the middle of these maps suggest.

<figure class="align-center">
  <img src="{{ '/img/poblacion_cartograms_withK.jpg' | absolute_url }}" alt="">
  <figcaption>
	 Population of Chile by region. Data source: Census, 2017
	</figcaption>
</figure>

I like the first option on the left, but it makes it hard to compare the relative size of regions, and clearly downplays just as populated is the Metropolitan Región. The Dorling cartogram is perhaps my favourite option here: it looks fine and strikes a good balance between preserving the rough shape of Chile and communicating the data. 