---
title: "cuQIT - Publications"
layout: gridlay
excerpt: "cuQIT - Publications."
sitemap: false
permalink: /publications/
---


# Publications

You can also find my research contributions on [Google Scholar](https://scholar.google.ca/citations?user=lqDWDJcAAAAJ&hl=en&oi=ao)


## Preprints
E. Scott Goudreau, Connor Kupchak, Benjamin J. Sussman, Robert W. Boyd, Jeff S. Lundeen<br />
<em>Theory of Four-Wave Mixing of Cylindrical Vector Beams in Optical Fibers</em><br />
<a href="https://arxiv.org/abs/1912.10109">arXiv:1912.10109</a>

## Full List of publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
