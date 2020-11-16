---
title: "Activities"
layout: textlay
excerpt: "Quantum Activities at Ghent University. Needs update."
sitemap: false
permalink: /activities.html
---

# News

{% for article in site.data.activities %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
