---
layout: works
sidebar: right
show_meta: false
title: "Works"
subheadline: Solo
header: no
permalink: "/works-solo/"
---

<ul class="side-nav">
    {% for post in site.categories.works %}
    {% if post.category_music == "Solo" %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{% if post.subheadline %}{{ post.subheadline }} &middot; {% endif %}<strong>{{ post.title }}</strong><br><span style="color: #000000;">{{ post.year_composed }}/For {{ post.instrumentation }}</span></a></li>
    {% endif %}
    {% endfor %}
</ul>