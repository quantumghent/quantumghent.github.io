---
title: "Outreach"
layout: textwithmath
excerpt: "Why nobody understands quantum physics"
sitemap: false
permalink: /outreach/
---

<div style="margin-bottom: 3cm;"></div>

# Why Nobody Understands Quantum Physics          (And Everyone Needs to Know Something About It)



<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="2000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        {% assign slide_number = 0 %}
        {% for image in site.data.outreach-carousel %}
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
    {% for image in site.data.outreach-carousel %}

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

**Contact the authors:** [fverstraete@gmail.com](mailto:fverstraete@gmail.com) and [celine.broeckaert@gmail.com](mailto:celine.broeckaert@gmail.com)
<p> Prof. Frank Verstraete</p>
<p>Department of Mathematics and Theoretical Physics</p>
<p>Centre for Mathematical Sciences, Wilberforce Rd, Cambridge CB3 0WA</p>
<p>United Kingdom</p>





<div style="margin-bottom: 1000cm;"></div>
