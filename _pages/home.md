---
title: "QuantumGroup@UGent"
layout: homelay
excerpt: "Quantum Group at Ghent University."
sitemap: false
permalink: /
---
<div class="page-header">
<h1>
Quantum Group @ UGent<br>
<small>Exploring Tensor Networks & Quantum Entanglement</small>
</h1>
</div>

<div markdown="0" id="home-carousel" class="carousel slide" data-ride="carousel" data-interval="10000" data-pause="null" data-keyboard="true" >
    <!-- Menu -->
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
    <!-- Items -->
    <div class="carousel-inner">
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
<div align="justify">
<p class="lead"><a href="/research/">Research</a> in the QuantumGroup@Ugent is focused on unravelling entanglement patterns in interacting quantum many-body systems.  We are developing the theory of quantum tensor networks, devise novel computational methods for optimizing them, and apply those to problems in condensed matter physics, quantum field theory, atomic physics and quantum computing. Very recently we have added an experimental research line on ultra-cold atoms, with our <a href="/bec/">first Belgian lab hosting a Bose-Einstein Condensate</a>.</p>
</div>
