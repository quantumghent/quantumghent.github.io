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
{% assign staff = site.data.staff | sort: "sname","last" %}
{% for member in staff %}

{% include teammember.html %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}

## Postdoctoral researchers

{% assign number_printed = 0 %}
{% assign postdocs = site.data.postdocs | sort: "sname","last" %}
{% for member in postdocs %}

{% include teammember.html %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}

## PhD students

{% assign number_printed = 0 %}
{% assign phds = site.data.phds | sort: "sname","last" %}
{% for member in phds %}

{% include teammember.html %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}

## Former members

{% assign number_printed = 0 %}
{% assign alumni = site.data.alumni | sort: "sname","last" %}

{% for member in alumni %}

{% include alumnimember.html %}

{% endfor %}

{% assign number_printed_mod_n = number_printed | modulo: 4 %}
{% if number_printed_mod_n == 3 %}

</div>
{% endif %}

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
