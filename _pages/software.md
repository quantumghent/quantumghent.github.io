---
title: "Quantum Group - Software"
layout: gridlay
excerpt: "Quantum Group -- Software."
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

* Julia code for the 2018 European Tensor Network School: [Jutho/TNSchool2018](https://github.com/Jutho/TNSchool2018)

* Python code for the 2020 European Tensor Network School: [leburgel/BadHonnefTutorial](https://github.com/leburgel/BadHonnefTutorial)

# External references

Useful links:
* [TensorNetwork.org](http://tensornetwork.org)
* [Tensors.net](https://www.tensors.net)
* [TensorTrace](https://www.tensortrace.com)

Other open-source tensor network packages
* [quimb](https://github.com/jcmgray/quimb)
* [ITensor and ITensors.jl](http://itensor.org)
* [Tensor Network by Google](https://github.com/google/TensorNetwork)
* [Tensor Network Python (TeNPy)](https://github.com/tenpy/tenpy)
* [Uni10](http://yingjerkao.github.io/uni10/)
