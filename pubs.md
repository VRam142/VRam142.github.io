---
title: "Ramani Lab - Publications"
layout: gridlay
excerpt: "Ramani Lab -- Publications."
---


# **publications**
<hr>
Here is a sampling of some of the papers that guide our lab's research. You can also find me on [google scholar](https://scholar.google.com/citations?user=BjwGIbcAAAAJ&hl=en) and [pubmed](https://www.ncbi.nlm.nih.gov/pubmed?term=\(Vijay%20Ramani%5BAuthor%20-%20Full%5D\)%20AND%20Jay%20Shendure%5BAuthor%20-%20Full%5D#rss_menu). #: co-senior author; \*: equal contribution.

{% for publication in site.data.publist %}

<div class="wrapper row3">
  <div id="container">
    <div class="full_width clear">
      <ol>
        <li>
          publication.
            <i>Mol. Cell.</i> 2019; pii: S1097-2765(19) 30618-5. PMID: 31495564.
            <a href="files/2019_MolCell_sci-L3.pdf" target="_blank">[pdf]</a>
            </br>
            Featured in Chinese by BioArt <a href="https://mp.weixin.qq.com/s?__biz=MzA3MzQyNjY1MQ==&mid=2652474921&idx=4&sn=6e60487c14dc5ea8cbda9ead6071789c&chksm=84e21d9db395948bc61a9e882d854647cc03706f340d3833f49aac97ed7fc8bb6127d3a5f273#rd" target="_blank">[link]</a>
            </br>
            Jay Shendure hosted on Nature Biotech webcasts <a href="https://www.workcast.com/register?cpak=4117659951158076&referrer=WEBCASTHOMEPAGE_MISSIONBIO_0619" target="_blank">[link]</a>
        </li>
      </ol>
    </div>
  </div>
</div>

			<!--PDBS - optional-->
			{% if publication.pdbs %}
			<li>Deposited Structure{% if publication.pdbs.size > 1 %}s{% endif %}:
				{% for code in publication.pdbs %}
				<a href="http://www.rcsb.org/pdb/explore/explore.do?structureId={{code}}">{{code}}</a>{% unless forloop.last %}, {% endunless %}
				{% endfor %}
			</li>
			{% endif %}

</div> <br>
{% endfor %}
</div>
