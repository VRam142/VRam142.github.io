---
title: "Ramani Lab - Publications"
layout: gridlay
excerpt: "Ramani Lab -- Publications."
---


# **publications**
<hr>
Here is a sampling of some of the papers that guide our lab's research. You can also find me on [google scholar](https://scholar.google.com/citations?user=BjwGIbcAAAAJ&hl=en) and [pubmed](https://www.ncbi.nlm.nih.gov/pubmed?term=\(Vijay%20Ramani%5BAuthor%20-%20Full%5D\)%20AND%20Jay%20Shendure%5BAuthor%20-%20Full%5D#rss_menu). #: co-senior author; \*: equal contribution.

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
