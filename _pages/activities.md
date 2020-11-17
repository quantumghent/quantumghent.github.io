---
title: "Activities"
layout: activitieslay
excerpt: "Quantum Activities at Ghent University. Needs update."
sitemap: false
permalink: /activities.html
---

# Activities. Needs update!!

{% for activity in site.data.activities %}
<p>{{ activity.date }} <br>
<em>{{ activity.headline }}</em></p>
{% endfor %}

{% include carousel.html height="50" unit="%" duration="7" %}

