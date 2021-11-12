---
title: "QuantumGroup@UGent - Members"
layout: gridlay
excerpt: "QuantumGroup@UGent --- Team members."
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
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <h5><i>{{ member.info }}</i></h5>
  <a href="mailto:{{ member.email }}"><i class="fas fa-envelope-square fa-2x"></i></a>
  {% if member.site %}<a href="{{ member.site }}"><span class="fa-stack fa-1x fa-stacked"><i class="fas fa-square fa-stack-2x"></i><i class="fas fa-home fa-stack-1x fa-stack-inner fas-inverse"></i></span></a>{% endif %} {% if member.orcid %}<a href="https://orcid.org/{{ member.orcid }}"><i class="ai ai-orcid-square ai-2x"></i></a>{% endif %} {% if member.scholar %}<a href="http://scholar.google.com/citations?user={{ member.scholar }}"><i class="ai ai-google-scholar-square ai-2x"></i></a>{% endif %} {% if member.github %}<a href="http://github.com/{{ member.github }}"><i class="fab fa-github-square fa-2x"></i></a>{% endif %} {% if member.twitter %}<a href="https://twitter.com/{{ member.twitter }}"><i class="fab fa-twitter-square fa-2x"></i></a>{% endif %}
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
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
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
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <h5><i>{{ member.info }}</i></h5>
  <a href="mailto:{{ member.email }}"><i class="fas fa-envelope-square fa-2x"></i></a>
  {% if member.site %}<a href="{{ member.site }}"><span class="fa-stack fa-1x fa-stacked"><i class="fas fa-square fa-stack-2x"></i><i class="fas fa-home fa-stack-1x fa-stack-inner fas-inverse"></i></span></a>{% endif %} {% if member.orcid %}<a href="https://orcid.org/{{ member.orcid }}"><i class="ai ai-orcid-square ai-2x"></i></a>{% endif %} {% if member.scholar %}<a href="http://scholar.google.com/citations?user={{ member.scholar }}"><i class="ai ai-google-scholar-square ai-2x"></i></a>{% endif %} {% if member.github %}<a href="http://github.com/{{ member.github }}"><i class="fab fa-github-square fa-2x"></i></a>{% endif %} {% if member.twitter %}<a href="https://twitter.com/{{ member.twitter }}"><i class="fab fa-twitter-square fa-2x"></i></a>{% endif %}
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

## More pictures of the team

<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="5000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        {% assign slide_number = 0 %}
        {% for image in site.data.group-carousel %}
        {% if slide_number == 0 %}
            <li data-target="#carousel" data-slide-to="{{ slide_number }}" class="active"></li>
        {% else %}
        <li data-target="#carousel" data-slide-to="{{ slide_number }}"></li>
        {% endif %}
        {% assign slide_number = slide_number | plus: 1 %}
        {% endfor %}
    </ol>
    <!-- Items -->
    <div class="carousel-inner" markdown="0">
    {% assign slide_number = 0 %}
    {% for image in site.data.group-carousel %}

        {% if slide_number == 0 %}
            <div class="item active">
        {% else %}
            <div class="item">
        {% endif %}
            <img src="{{ site.url }}{{ site.baseurl }}/images/{{ image.image }}" alt="Slide {{ slide_number }}" />
        </div>

    {% assign slide_number = slide_number | plus: 1 %}
    {% endfor %}
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>
