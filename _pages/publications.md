---
title: "CUQuIT - Publications"
layout: gridlay
excerpt: "CUQuIT - Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

(For a full list of publications and patents see [below](#full-list-of-publications) or go to [Google Scholar](https://scholar.google.ca/citations?user=lqDWDJcAAAAJ&hl=en&oi=ao))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Preprints
E. Scott Goudreau, Connor Kupchak, Benjamin J. Sussman, Robert W. Boyd, Jeff S. Lundeen<br />
<em>Theory of Four-Wave Mixing of Cylindrical Vector Beams in Optical Fibers</em><br />
<a href="https://arxiv.org/abs/1912.10109">arXiv:1912.10109</a>

## Full List of publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
