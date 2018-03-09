---
layout: gridlay
title: research
subtitle: Ramani Lab Research
---

# Our Research Interests
{% for project in site.data.research_aims %}
<hr>
<!-- The paddingtop and margin-top edits allow anchors to link properly. -->
<div id = "{{project.title}}" class="row" style="padding-top: 60px; margin-top: -60px;">
    <div class="col-sm-12">
        <h2 align="center"> {{project.name}} </h2> <br>
        <img align="center" class="img-responsive" src="{{project.image}}" {% if project.altimage %} onmouseover="this.src='{{project.altimage}}';" onmouseout="this.src='{{project.image}}';" {% endif %} alt="{{project.title}}"><br>
    </div>
    <div class="col-sm-12">
        <p class="text-justify">{{project.description | markdownify}}</p>
    </div>
</div>
{% endfor %}
