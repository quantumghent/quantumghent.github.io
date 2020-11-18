---
title: "Quantum Group - Publications"
layout: gridlay
excerpt: "Quantum Group -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

<script src="http://code.jquery.com/jquery-1.9.1.min.js"></script>
<script>

     $(function(){

            var iFrames = $('iframe');

            function iResize() {

                for (var i = 0, j = iFrames.length; i < j; i++) {
                  iFrames[i].style.height = iFrames[i].contentWindow.document.body.offsetHeight + 'px';}
                }

                if ($.browser.safari || $.browser.opera) { 

                   iFrames.load(function(){
                       setTimeout(iResize, 0);
                   });

                   for (var i = 0, j = iFrames.length; i < j; i++) {
                        var iSource = iFrames[i].src;
                        iFrames[i].src = '';
                        iFrames[i].src = iSource;
                   }

                } else {
                   iFrames.load(function() { 
                       this.style.height = this.contentWindow.document.body.offsetHeight + 'px';
                   });
                }

            });
</script>


<iframe
    allowtransparency="true"
    frameborder="0"
    src="https://biblio.ugent.be/publication?limit=250&amp;q=author+exact+3BD5ED34-F0EE-11E1-A9DE-61C894A0A6B4+or+author+exact+F9521A46-F0ED-11E1-A9DE-61C894A0A6B4&amp;sort=year.desc&amp;sort=datecreated.desc&amp;style=vancouver&amp;embed=1" style="width:100%; height:100%;" onLoad="calcHeight();">
</iframe>

<!--
## Group highlights

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.ch/citations?user=TqxYWZsAAAAJ), [ResearcherID](https://www.researcherid.com/rid/D-7763-2012))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %} -->
