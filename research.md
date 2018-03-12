---
layout: gridlay
title: research
subtitle: Ramani Lab Research
---

# **research interests**
{% for project in site.data.research_aims %}
<hr>
<!-- The paddingtop and margin-top edits allow anchors to link properly. -->
<div id = "{{project.title}}" class="row" style="padding-top: 60px; margin-top: -60px;">
    <div class="col-sm-7">
        <h3> {{project.title | markdownify}} </h3>
        <p class="text-justify">{{project.description | markdownify}}</p>
    </div>
    <div class="col-sm-5">
        <img class="img-responsive" src="{{project.image}}" {% if project.altimage %} onmouseover="this.src='{{project.altimage}}';" onmouseout="this.src='{{project.image}}';" {% endif %} alt="{{project.title}}"><br>
    </div>
</div>
{% endfor %}
