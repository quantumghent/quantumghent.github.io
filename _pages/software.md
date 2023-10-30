---
title: "QuantumGroup@UGent - Software"
layout: gridlaywithmath
excerpt: "QuantumGroup@UGent -- Software."
sitemap: false
permalink: /software/
---
# Open-source software and notebooks

Our group has developed several publicly available (and thus open source) software packages using the scientific programming language [Julia](https://www.julialang.org). We also have an extensive amount of actively developed tensor network code using [MATLAB](https://nl.mathworks.com/products/matlab.html); contact Laurens Vanderstraeten or Bram Vanhecke for more information.

## Physics and tensor network packages

{% assign number_printed = 0 %}
{% for package in site.data.software %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if package.language == "julia" %}
{% if package.topic == "physics" %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ package.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/software/{{ package.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ package.description }}</p>
  <p><i class="fab fa-github"></i>/<strong><a href="{{ package.link.url }}">{{ package.link.display }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## General purpose packages

{% assign number_printed = 0 %}

{% for package in site.data.software %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if package.language == "julia" %}
{% if package.topic == "general" %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ package.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/software/{{ package.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ package.description }}</p>
  <p><i class="fab fa-github"></i>/<strong><a href="{{ package.link.url }}">{{ package.link.display }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Notebooks and other software links

* Julia notebooks for Tensor Network Methods: [quantumghent/TensorTutorials](https://quantumghent.github.io/TensorTutorials/intro.html)

* Python code for the 2020 European Tensor Network School: [leburgel/uniformMpsTutorial](https://github.com/leburgel/uniformMpsTutorial)

* Julia code for the 2018 European Tensor Network School: [Jutho/TNSchool2018](https://github.com/Jutho/TNSchool2018)

{% capture pubsUsingPkg %}{%  bibliography_count -f usingPkg -q @Article[key!=ExampleArticle]* @Preprint[key!=ExamplePreprint]* @Thesis* @PhdThesis[key!=ExamplePhD]* @MastersThesis[key!=ExampleMasters]* @HonoursThesis* %}{% endcapture %}
{% assign pubsUsingPkg = pubsUsingPkg | plus: 0 %}

{% capture pkgUsingPkg %}{%  bibliography_count -f usingPkg -q @Package[key!=ExamplePackage]* --group_by none %}{% endcapture %}
{% assign pkgUsingPkg = pkgUsingPkg | plus: 0 %}

{% if pubsUsingPkg > 0 %}
## Publications using QuantumGroup@UGent software packages

A partial list of publications and software pacakges that make use of QuantumGroup@UGent packages. If you want to add your publication or package to this list, please contact us.

{% bibliography -f usingPkg -q @Article[key!=ExampleArticle]* @Preprint[key!=ExamplePreprint]* @Thesis* @PhdThesis[key!=ExamplePhD]* @MastersThesis[key!=ExampleMasters]* @HonoursThesis* %}

{% if pkgUsingPkg > 0%}
### Packages extending ours

{% bibliography -f usingPkg -q @Package[key!=ExamplePackage]* --group_by none %}
{% endif %}{% endif %}
