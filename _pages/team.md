---
title: "Quantum Group - Members"
layout: gridlay
excerpt: "Quantum Group: Team members"
sitemap: false
permalink: /team/
---

# Group Members

## Senior staff
{% assign number_printed = 0 %}
{% for member in site.data.staff %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <h5><i>{{ member.info }}</i></h5>
  <a href="mailto:{{ member.email }}"><i class="fas fa-envelope-square fa-2x"></i></a>
  {% if member.scholar %}<a href="http://scholar.google.com/citations?user={{ member.scholar }}"><i class="ai ai-google-scholar-square ai-2x"></i></a>{% endif %} {% if member.github %}<a href="http://github.com/{{ member.github }}"><i class="fab fa-github-square fa-2x"></i></a>{% endif %} {% if member.twitter %}<a href="https://twitter.com/{{ member.twitter }}"><i class="fab fa-twitter-square fa-2x"></i></a>{% endif %}
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

## Postdoctoral researchers
{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <h5><i>{{ member.info }}</i></h5>
  <a href="mailto:{{ member.email }}"><i class="fas fa-envelope-square fa-2x"></i></a>
  {% if member.scholar %}<a href="http://scholar.google.com/citations?user={{ member.scholar }}"><i class="ai ai-google-scholar-square ai-2x"></i></a>{% endif %} {% if member.github %}<a href="http://github.com/{{ member.github }}"><i class="fab fa-github-square fa-2x"></i></a>{% endif %} {% if member.twitter %}<a href="https://twitter.com/{{ member.twitter }}"><i class="fab fa-twitter-square fa-2x"></i></a>{% endif %}
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

## PhD students
{% assign number_printed = 0 %}
{% for member in site.data.phds %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <h5><i>{{ member.info }}</i></h5>
  <a href="mailto:{{ member.email }}"><i class="fas fa-envelope-square fa-2x"></i></a>
  {% if member.scholar %}<a href="http://scholar.google.com/citations?user={{ member.scholar }}"><i class="ai ai-google-scholar-square ai-2x"></i></a>{% endif %} {% if member.github %}<a href="http://github.com/{{ member.github }}"><i class="fab fa-github-square fa-2x"></i></a>{% endif %} {% if member.twitter %}<a href="https://twitter.com/{{ member.twitter }}"><i class="fab fa-twitter-square fa-2x"></i></a>{% endif %}
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

<!-- ## Former members and long-term visitors -->

## Administrative Support
<a href="mailto:inge.vandervennet@ugent.be">Inge Van der Vennet</a> is helping us (and other groups) with administration.
