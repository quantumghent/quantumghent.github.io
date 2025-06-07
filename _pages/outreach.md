---
title: "Outreach"
layout: deafault
excerpt: "Why Nobody Understands Quantum Physics"
permalink: /outreach/
---

<div style="margin-bottom: 3cm;"></div>

# Why Nobody Understands Quantum Physics

<div id="carousel" class="carousel slide" data-ride="carousel" data-interval="5000" data-pause="hover">

  <!-- Indicators -->
  <ol class="carousel-indicators">
    {% for image in site.data.outreach-carousel %}
      <li data-target="#carousel" data-slide-to="{{ forloop.index0 }}" class="{% if forloop.first %}active{% endif %}"></li>
    {% endfor %}
  </ol>

  <!-- Slides -->
  <div class="carousel-inner">
    {% for image in site.data.outreach-carousel %}
      <div class="carousel-item {% if forloop.first %}active{% endif %}">
        <img src="{{ '/assets/images/' | relative_url }}{{ image.image }}" class="d-block w-100" alt="{{ image.alt | default: 'Slide ' | append: forloop.index }}">
      </div>
    {% endfor %}
  </div>

  <!-- Controls -->
  <a class="carousel-control-prev" href="#carousel" role="button" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="carousel-control-next" href="#carousel" role="button" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>

</div>

<br><br>

**Contact the authors:** [fverstraete@gmail.com](mailto:fverstraete@gmail.com) and [celine.broeckaert@gmail.com](mailto:celine.broeckaert@gmail.com)

<div style="margin-bottom: 20cm;"></div>
