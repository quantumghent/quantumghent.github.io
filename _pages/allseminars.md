---
title: "QuantumGroup@UGent - News"
layout: textlay
excerpt: "Quantum Seminars at Ghent University."
sitemap: false
permalink: /allseminars.html
---

# Seminars

<div class="well">
{% assign sorted_seminars = site.seminars | sort: 'talk_date' | reverse %}
{% for seminar in sorted_seminars %}
<p>
    {%- capture title -%}
        <b style="color: #5f6568;">
            {% if seminar.abstract %}
                <a href="{{seminar.url}}" style="color: #5f6568;">{{ seminar.title }}</a>
            {% else %}
                {{ seminar.title }}
            {% endif %}
        </b>
    {% endcapture %}
    {{ seminar.date | date: '%B %e, %Y, %l:%M %p (%Z)'}}
    {{ title }} {{ seminar.speaker }}, <em>{{ seminar.affiliation }}</em>
    </p>
    {% endfor %}
</div>