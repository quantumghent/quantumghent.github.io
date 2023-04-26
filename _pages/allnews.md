---
title: "QuantumGroup@UGent - News"
layout: textlay
excerpt: "Quantum News at Ghent University."
sitemap: false
permalink: /allnews.html
---

# News

{% assign articles = site.data.news | sort: 'date' | reverse %}
{% for article in articles %}
<p>{{ article.date | date: '%B %e, %Y'}}<br>
<em>{{ article.headline }}</em></p>
{% endfor %}
