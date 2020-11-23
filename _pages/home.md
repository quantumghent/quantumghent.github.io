---
title: "Quantum Group @ UGent - Home"
layout: homelay
excerpt: "Quantum Group at Ghent University."
sitemap: false
permalink: /
---

<div class="carousel-overlay-title">
Welcome to the QuantumGroup@UGent
</div>
<div class="carousel-overlay-subtitle">
Exploring Tensor Networks and Quantum Entanglement
</div>
<div markdown="0" id="home-carousel" class="carousel slide" data-ride="carousel" data-interval="4000" data-pause="null" data-keyboard="true" >
    <!-- Menu -->
    <!--
    <ol class="carousel-indicators">
        {% assign slide_number = 0 %}
        {% for image in site.data.home-carousel %}
        {% if slide_number == 0 %}
            <li data-target="#home-carousel" data-slide-to="{{ slide_number }}" class="active"></li>
        {% else %}
        <li data-target="#home-carousel" data-slide-to="{{ slide_number }}"></li>
        {% endif %}
        {% assign slide_number = slide_number | plus: 1 %}
        {% endfor %}
    </ol>
    -->
    <!-- Items -->
    <div class="carousel-inner" markdown="0">
    {% assign slide_number = 0 %}
    {% for image in site.data.home-carousel %}

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
  <a class="left carousel-control" href="#home-carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#home-carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>
