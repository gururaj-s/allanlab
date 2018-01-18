---
title: "MemoryLab - Publications"
layout: gridlay
excerpt: "MemoryLab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

Also available at [Google Scholar](https://scholar.google.com/citations?user=EWU0STsAAAAJ&hl=en&oi=sra), [DBLP](https://scholar.google.ch/citations?user=TqxYWZsAAAA)

{% for publi in site.data.publist %}

   <a href='{{ publi.link.url  }}'>{{ publi.title }}</a> <br />
  <em>{{ publi.authors }} </em><br />
  {{ publi.conf.preamble }} <u>{{ publi.conf.fullname }} **({{ publi.conf.abbreviation }})** </u> {% if publi.conf.location %}, {{ publi.conf.location }} {% endif %}, {{ publi.date }}.
  {% if publi.other %}<i>{{ publi.other }}</i> {% endif %}
{% endfor %}

{% comment %}
## Full List

{% for publi in site.data.publist %}

  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
{% endcomment %}

{% comment %}
## Highlights

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
{% endcomment %}
