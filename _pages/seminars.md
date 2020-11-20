---
title: "Seminars"
layout: textlay
excerpt: "Quantum Group -- Seminars"
sitemap: false
permalink: /seminars.html
---

# Seminars

We have a weekly seminar on Fridays, 1pm (Central European Time). If you are interested in giving a seminar in our group, feel free to contact any of us any time.

## List of passed and future seminars:

{% for seminar in site.data.seminars %}
<p>{{ seminar.date }}
<br><b>{{ seminar.speaker }}</b>, {{ seminar.affiliation }}
<br><em>{{ seminar.title }}</em></p>
{% endfor %}
