---
title:  Pharmacies in Santiago
date:   2020-03-02 16:40:16
tags:
  - ArcMap
  - interactive
  - Python
  - Chile
  - choropleth
  - SVG
excerpt: Two maps and a graph exploring the relation between pharmacy accessibility and economic inequalities in Santiago de Chile.
--- 

Forty percent of Chilean pharmacies belong to three major chains: Ahumada, Salcobrand and CruzVerde, which collectively control between [80%](https://www.fne.gob.cl/wp-content/uploads/2019/11/Informe_preliminar.pdf) and [95%](href="https://www.economia.gob.cl/wp-content/uploads/2013/04/Boletin-Mercado-de-Medicamentos.pdf) of the market, depending on the source.
These sellers have been involved in [collusion](http://economia.uc.cl/wp-content/uploads/2015/07/tesis_vserey.pdf) and have been repeatedly accused of [inflating the prices of drugs](https://www.publimetro.cl/cl/noticias/2019/10/10/medicamentos-precios.html).
According to a 2019 [government report](https://www.fne.gob.cl/wp-content/uploads/2019/11/Informe_preliminar.pdf), these chains only cover 44% of the country’s municipalities, and appear to concentrate in highly-populated areas with relatively high income.

In this analysis, I used population data from the 2017 census, data about [average income levels](http://www.sil.mintrab.gob.cl/) from the Ministry of Work and about [poverty levels](http://observatorio.ministeriodesarrollosocial.gob.cl/casen-multidimensional/casen/casen_2017.php) from the Encuesta Casen to explore how this uneven distribution plays out in Santiago de Chile.
For the [pharmacies location](https://rentry.co/bs-scrape)) I scraped some commercial directories using [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)).


<figure class="align-center">
  <img src="{{ '/img/ph-choropleth-2.svg' | absolute_url }}" alt="">
  <figcaption>
	The maps shows the distribution of pharmacies in relation to the population, by municipality. The lighter shade of grey marks areas where my research did not return any pharmacy. Sources: Census 2017, scraped pharmacy dataset 
	</figcaption>
</figure> 


<figure class="align-center">
  <img src="{{ site.baseurl }}/img/ph-scatter-plot-2.svg">
  <figcaption>
	In the scatterplot, each square represents a municipality, using the same colour coding as the map above. The dotted lines mark the boundaries between quantiles.  
	</figcaption>
</figure> 


Together, the scatterplot and map give a good general overview, showing how wealthier areas are much better served by these pharmacy chains.
On the downside, it is hard to see how a particular municipality is doing, especially for those who are not familiar with the city. Rather than crowding the map with labels, I experimented with making an interactive version of the map.
First, I exported the map with <a href="https://mapshaper.org/">Mapshaper</a>, adding a [unique ID field](https://simplemaps.com/resources/guide-to-mapshaper).
I then exported the attribute data from ArcGIS into a CSV, and used [Python](https://rentry.co/csv2svgmap) to match it to my polygons.

<figure class="align-center">
	<object class="col three" data="{{ site.baseurl }}/img/ph-interactive-map-2.svg" type="image/svg+xml">
    </object>
  <figcaption>
	Hover on a polygon to discover its name, people-to-pharmacies ratio and average income levels. As of early 2020, 1000 CLP is approximately 1 GPB, or just over 1 EURO. 
	</figcaption>
</figure> 