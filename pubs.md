---
title: "Ramani Lab - Publications"
layout: gridlay
excerpt: "Ramani Lab -- Publications."
---


# **publications**
<hr>
Here is a sampling of some of the papers that guide our lab's research. You can also find me on [google scholar](https://scholar.google.com/citations?user=BjwGIbcAAAAJ&hl=en) and [pubmed](https://www.ncbi.nlm.nih.gov/pubmed?term=\(Vijay%20Ramani%5BAuthor%20-%20Full%5D\)%20AND%20Jay%20Shendure%5BAuthor%20-%20Full%5D#rss_menu). #: senior author; \*: equal contribution. In cases where a first author is from the lab, all first authors are highlighted in <b>bold</b>.

<div class="wrapper row3">
  <div id="container">
    <div class="full_width clear">
      <ol>
        {% for publication in site.data.publist %}
          <li>
            {{publication.authors}}. "{{publication.title}}." <i>{{publication.journal}}</i>; {{publication.date}}; PMID: {{publication.pmid}}; <a href="{{publication.pdf}}">[pdf]</a>
          </li>
          <br>
        {% endfor %}
      </ol>
    </div>
  </div>
</div>
