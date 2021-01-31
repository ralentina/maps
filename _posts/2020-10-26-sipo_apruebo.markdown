---
layout: post
title: Sipo, Apruebo!
date: 2020-10-26 16:00:00
tags:
  - ArcMap
  - choropleth
  - bubble-map
  - Chile
  - World
excerpt: Quick, semi-serious map showing Chilean communities abroad voted in the 2020 constitutional referendum.
---

On the 25th October 2020, Chile held a <a href="https://www.theguardian.com/world/2020/oct/26/chile-vote-scrap-pinochet-constitution">referendum</a> to change its constitution, which was imposed during Pinochet's military dictatorship. People voted overwhelmingly for change: the 'apruebo' (yes to changes) obtained a 78.28 %, the rechazo (no to changes) just 21.72%.  

On the day after the vote, I rushed to put together a map of the votes of Chileans abroad, using the partial results published by Servel. In many places, for example France, the majority of Chileans are former exiles and their relatives, so it was hardly surprising the see the 'apruebo' triumph.
Given the <a href="https://interferencia.cl/articulos/vitacura-y-versalles-la-derrota-de-la-elite">strong correlation between people income and voting choices</a>, it also makes sense that places such as the Emirates would reject the changes.

<figure class="align-center">
  <img src="{{ '/img/plebiscito.jpg' | absolute_url }}" alt="">
  <figcaption>
	 Partial results of the 2020 constitutional referendum abroad. This isn't a good map! Data source: SERVEL, 26th October 2020
	</figcaption>
</figure> 

Even as I was making it, I was aware that a choropleth was a lazy choice in this case: it's very misleading because the amount of red or blue depends on a country's size, not on the number of votes. Take Russia: it takes up a lot of space, but it counted for just 27 votes!

A few months later, when I had more time, I had a go at improving the map, this time using the complete results released by Servel. I used bubbles to display the number of valid votes in each country. It seems reasonable to assume this number works as proxy for the size of each country's Chilean population, so this adds a layer of information to the map.
I kept an (almost) identical colour scheme, but this time I used the overall referendum result (78.28% 'apruebo') as a threashold for my classes. I find the result not only clearer, but also more visually pleasing:

<figure class="align-center">
  <img src="{{ '/img/plebiscito_bubble_map.jpg' | absolute_url }}" alt="">
  <figcaption>
	 Final results of the 2020 constitutional referendum abroad. Data source: SERVEL, January 2021
	</figcaption>
</figure> 