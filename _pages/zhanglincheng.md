---
title: "Zhanglin Cheng"
layout: zhanglinTemplate
excerpt: "Zhanglin Cheng's page"
sitemap: false
permalink: /~zhanglin.html
---
{% assign year = 2049 %}
<div markdown="0">
{% for publi in site.data.czlJournal %}
    {% if year > publi.year %}
    {% assign year = publi.year %}
    <h2>{{ publi.year }}</h2>
    {% endif %}
    <ul class="style3">
    <li> <strong><a href="{{ publi.link.url }}" target="_blank">{{ publi.title }}</a></strong></li>
    </ul>
    <blockquote class="style3">
    <p>{{ publi.authors }}</p>
    <p><i>{{ publi.link.display }}</i></p>
    <p>&nbsp;</p>
    </blockquote>
{% endfor %}
</div>