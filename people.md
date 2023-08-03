---
layout: gridlay
title: people
subtitle: Ramani Lab Members
---

# **lab members**
{% for person in site.data.members %}
<hr>
<!-- The paddingtop and margin-top edits allow anchors to link properly. -->
<div id = "{{person.name}}" class="row" style="padding-top: 60px; margin-top: -60px;">
    <div class="col-sm-4">
        <img class="img-responsive" src="{{person.image}}" {% if person.altimage %} onmouseover="this.src='{{person.altimage}}';" onmouseout="this.src='{{person.image}}';" {% endif %} alt="{{person.name}}"><br>
        <strong>{{person.name}}</strong> <br>
        {{person.position}} <br>
        <em>{{person.email}}</em> <br>
        {% if person.website %}
          <a href= "{{person.website}}">{{person.website}}</a> <br>
        {% endif %}
        {% if person.orcid %}
          <a href="http://orcid.org"><img class="inline-block" src="/static/img/orcid_logo.png"></a>
          <a href="http://{{person.orcid}}"> {{person.orcid}}</a> <br>
        {% endif %}
        {% if person.scholar %}
          <a href= "http://scholar.google.com/citations?user={{person.scholar}}"> Scholar Citations </a> <br>
        {% endif %}
        {% if person.twitter %}
          <a href= "http://twitter.com/{{person.twitter}}"> @{{person.twitter}} </a> <br>
        {% endif %}
    </div>
    <div class="col-sm-8">
        <p class="text-justify">{{person.description | markdownify}}</p>
    </div>
</div>
{% endfor %}
<hr>
<strong>Rotation Students</strong>: <br>
<table class="w3-table">
<tr>
  <th>Name</th>
  <th>Graduate Program / Quarter / Year</th>
  <th>Thesis Lab</th>
</tr>
<tr>
  <td>Derek Bogdanoff</td>
  <td>Tetrad / Winter / 18-19</td>
  <td>Nowakowski Lab</td>
</tr>
<tr>
  <td>Wei Gordon</td>
  <td>Tetrad / Spring / 18-19</td>
  <td>Ahituv Lab</td>
</tr>
<tr>
  <td>Tianna Grant</td>
  <td>iPQB / Summer / 19-20</td>
  <td>Ye Lab</td>
</tr>
<tr>
  <td>Jasmine Sims</td>
  <td>Tetrad / Spring / 19-20</td>
  <td>Ahituv Lab</td>
</tr>
<tr>
  <td>Zach Cogan</td>
  <td>Tetrad / Winter / 20-21</td>
  <td>Walter Lab</td>
</tr>
<tr>
  <td>Alex Hong</td>
  <td>Tetrad / Winter / 20-21</td>
  <td>Bondy-Denomy Lab</td>
</tr>
<tr>
  <td>Bryson Choy</td>
  <td>BMI / Fall / 22-23</td>
  <td>Ye Lab</td>
</tr>
</table>
<hr>
<strong>Lab Alumni</strong>: <br>
<table class="w3-table">
<tr>
  <th>Name</th>
  <th>Previous Position / Years</th>
  <th>Currently</th>
</tr>
<tr>
  <td>Aidan Keith</td>
  <td>Research Specialist / 2018 - 2020</td>
  <td>PhD Program @ UW (Genome Sciences; Shendure Lab)</td>
</tr>
<tr>
  <td>Yuan Daniel Xu</td>
  <td>Research Specialist / 2020 - 2021</td>
  <td>PhD Program @ UC Santa Cruz (BME; Haussler Lab)</td>
</tr>
<tr>
  <td>Colin McNally, PhD</td>
  <td>Postdoctoral Fellow / 2020 - 2022</td>
  <td>Computational Biologist @ Biotech Startup</td>
</tr>
<tr>
  <td>Nour Abdulhay, PhD</td>
  <td>PhD Student (BMS) / 2019 - 2022</td>
  <td>Scientist @ Biotech Startup</td>
</tr>
<tr>
  <td>Arjun Scott Nanda, PhD</td>
  <td>PhD Student (BMI) / 2020 - 2023</td>
  <td></td>
</tr>
</table>
