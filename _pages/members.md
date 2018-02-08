---
title: "Memory Systems Lab - Members"
layout: gridlay
excerpt: "Memory Systems Lab: Members"
sitemap: false
permalink: /members/
---

# Group Members

Jump to [Current Members](#current), [Alumni](#alumni). 

## Current
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}
  
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
 
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  
  </ul>
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

## Alumni
{% assign number_printed = 0 %}
{% for member in site.data.team_members_alum %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix alum">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}
  
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
 
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  
  </ul>
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


[//]: # (## Master and Bachelor Students                            )
[//]: # ({% assign number_printed = 0 %}			    )
[//]: # ({% for member in site.data.students %}			    )
[//]: # (							    )
[//]: # ({% assign even_odd = number_printed | modulo: 2 %}	    )
[//]: # (							    )
[//]: # ({% if even_odd == 0 %}					    )
[//]: # (<div class="row">					    )
[//]: # ({% endif %}						    )
[//]: # (							    )
[//]: # (<div class="col-sm-6 clearfix">			    )
[//]: # (  <h4>{{ member.name }}</h4>				    )
[//]: # (  <i>{{ member.info }}<br>email: <{{ member.email }}></i>  )
[//]: # (  <ul style="overflow: hidden">			    )
[//]: # (  							    )
[//]: # (  {% if member.number_educ == 1 %}			    )
[//]: # (  <li> {{ member.education1 }} </li>			    )
[//]: # (  {% endif %}						    )
[//]: # (  							    )
[//]: # (  {% if member.number_educ == 2 %}			    )
[//]: # (  <li> {{ member.education1 }} </li>			    )
[//]: # (  <li> {{ member.education2 }} </li>			    )
[//]: # (  {% endif %}						    )
[//]: # (  							    )
[//]: # (  {% if member.number_educ == 3 %}			    )
[//]: # (  <li> {{ member.education1 }} </li>			    )
[//]: # (  <li> {{ member.education2 }} </li>			    )
[//]: # (  <li> {{ member.education3 }} </li>			    )
[//]: # (  {% endif %}						    )
[//]: # (  							    )
[//]: # (  {% if member.number_educ == 4 %}			    )
[//]: # (  <li> {{ member.education1 }} </li>			    )
[//]: # (  <li> {{ member.education2 }} </li>			    )
[//]: # (  <li> {{ member.education3 }} </li>			    )
[//]: # (  <li> {{ member.education4 }} </li>			    )
[//]: # (  {% endif %}						    )
[//]: # (  							    )
[//]: # (  </ul>						    )
[//]: # (</div>							    )
[//]: # (							    )
[//]: # ({% assign number_printed = number_printed | plus: 1 %}	    )
[//]: # (							    )
[//]: # ({% if even_odd == 1 %}					    )
[//]: # (</div>							    )
[//]: # ({% endif %}						    )
[//]: # (							    )
[//]: # ({% endfor %}						    )
[//]: # (							    )
[//]: # ({% assign even_odd = number_printed | modulo: 2 %}	    )
[//]: # ({% if even_odd == 1 %}					    )
[//]: # (</div>							    )
[//]: # ({% endif %}						    )
[//]: # (							    )
[//]: # (							    )
[//]: # (## Alumni						    )
[//]: # (<table align="center" style="width:100%">		    )
[//]: # (<tr><th>Visitors</th>					    )
[//]: # (    <th>Master Students</th> 				    )
[//]: # (    <th>Bachelor Students</th>				    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td>Nikolaos Iliopoulos, Spring 2016</td>		    )
[//]: # (    <td>Tjerk Benschop, Summer 2017</td>		    )
[//]: # (    <td>Vishnu Saj, Spring 2017</td>			    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td>Vitaly Fedoseev, all of 2016</td>		    )
[//]: # (    <td>Oliver Ostojic, Spring 2016</td>		    )
[//]: # (    <td>Joey Braspenning, Spring 2017</td>		    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td></td>						    )
[//]: # (    <td>Farshaad Hoeseni, Fall 2015</td>		    )
[//]: # (    <td>Margot Leemker, Spring 2017</td>		    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td></td>						    )
[//]: # (    <td></td>						    )
[//]: # (    <td>Sietske Lensen, Spring 2017</td>		    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td></td>						    )
[//]: # (    <td></td>						    )
[//]: # (    <td>Alexander Vanstone, Spring 2016</td>		    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td></td>						    )
[//]: # (    <td></td>						    )
[//]: # (    <td>Tjerk Benschop, Spring 2016</td>		    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td></td>						    )
[//]: # (    <td></td>						    )
[//]: # (    <td>Arjo Andringa, Spring 2016</td>		    )
[//]: # (  </tr>						    )
[//]: # (  <tr>							    )
[//]: # (    <td></td>						    )
[//]: # (    <td></td>						    )
[//]: # (    <td>Daniëlle van Klink, Spring 2016</td>		    )
[//]: # (  </tr>						    )
[//]: # (</table>						    )
[//]: # (							    )
[//]: # (## Administrative Support				    )
[//]: # (<a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van ng us (and other groups) with administration. )
[//]: # (                                                           )    





