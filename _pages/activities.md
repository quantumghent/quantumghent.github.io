---
title: "Activities"
layout: textlay
excerpt: "Quantum Activities at Ghent University. Needs update."
sitemap: false
permalink: /activities.html
---

# News

{% for activity in site.data.activities %}
<p>{{ activity.date }} <br>
<em>{{ activity.headline }}</em></p>
{% endfor %}
