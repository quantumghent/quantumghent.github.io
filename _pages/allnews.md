---
title: "QuantumGroup@UGent - News"
layout: textlay
excerpt: "Quantum News at Ghent University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
