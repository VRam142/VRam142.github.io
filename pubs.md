---
title: "Ramani Lab - Publications"
layout: gridlay
excerpt: "Ramani Lab -- Publications."
---


# **publications**
<hr>
You can also find me on [google scholar]((https://scholar.google.com/citations?user=BjwGIbcAAAAJ&hl=en)).

<!-- ## *highlights*

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?user=BjwGIbcAAAAJ&hl=en))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <p text-align="center">{{publi.title}}</p>
  <img src="{{publi.image}}" class="img-responsive" width="100%" style="float: center" />
  <p><strong><a href="{{publi.link.url}}">{{publi.link.display}}</a></strong></p>
  <p class="text-danger"><strong>{{publi.news1}}</strong></p>
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


## *full list* -->

{% include bib.html %}
