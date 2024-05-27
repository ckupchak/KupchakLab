---
title: "cuQIT - Publications"
layout: gridlay
excerpt: "cuQIT - Publications."
sitemap: false
permalink: /publications/
---


# Publications

You can also find our research contributions on [Google Scholar](https://scholar.google.ca/citations?user=lqDWDJcAAAAJ&hl=en&oi=ao)


### *cuQIT Lab*

A. Tareki, C. Kupchak, K. Mnaymneh<br />
<em> The Influence of Deposition Temperature and Material Stress on Low-Loss Silicon Nitride Films for Integrated Quantum Optics</em><br /> 
<a href="https://ieeexplore.ieee.org/document/10146373/similar#similar">IEEE Photonics Journal, vol. 15, no. 4, pp. 1-7 (2023) </a>
 


E. Scott Goudreau, Connor Kupchak, Benjamin J. Sussman, Robert W. Boyd, Jeff S. Lundeen<br />
<em>Theory of Four-Wave Mixing of Cylindrical Vector Beams in Optical Fibers</em><br />
<a href="https://www.osapublishing.org/josab/fulltext.cfm?uri=josab-37-6-1670&id=431634">JOSAB Vol. 37, Issue 6, pp. 1670-1682 (2020)</a>

### *Prior to Carleton*

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
