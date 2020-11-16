---
title: "Activities"
layout: textlay
excerpt: "Quantum Activities at Ghent University."
sitemap: false
permalink: /activities.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
