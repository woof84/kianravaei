---
layout: works
sidebar: right
show_meta: false
title: "Works"
subheadline: Chamber Music
header: no
permalink: "/works-chamber-music/"
---

<ul class="side-nav">
    {% for post in site.categories.works %}
    {% if post.category_music == "Chamber Music" %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{% if post.subheadline %}{{ post.subheadline }} &middot; {% endif %}<strong>{{ post.title }}</strong><br><span style="color: #000000;">{{ post.year_composed }}/For {{ post.instrumentation }}</span></a></li>
    {% endif %}
    {% endfor %}
</ul>