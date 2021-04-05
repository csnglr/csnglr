---
layout: category
title: Download Our Data
---

<div style="overflow-x:auto;">
<a href="/csnglr/admissions.csv" download="University Admissions Rates, Tuition Over time - ACCEPTANCE RATE.csv">Download Admissions Data 2003-2020</a>

<table>
  {% for row in site.data.admissions %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>

<a href="/csnglr/tuition.csv" download="University Admissions Rates, Tuition Over time - TUITION.csv">Download Tuition Data 2011-2020</a>
<table>
  {% for row in site.data.tuition %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
</div>

<style>

</style>
