---
title: "Memory Systems Lab - Projects"
layout: gridlay
excerpt: "Memory Systems Lab -- Projects"
sitemap: false
permalink: /projects
---

# Projects

{% assign number_printed = 0 %}
{% for member in site.data.projects %}
{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/projectpic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <h5> <b>Lead:</b> <a href="{{ site.url}}{{ site.baseurl }}/members">{{ member.lead }}</a></h5>
  <p> {{ member.description }} </p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
