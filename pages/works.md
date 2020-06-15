---
layout: works
sidebar: right
show_meta: false
title: "Works"
subheadline: All
header:
    image_fullwidth: Kian_Header_idea_5.png
permalink: "/works/"
---

<ul class="side-nav">
    {% for post in site.works reversed %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{% if post.subheadline %}{{ post.subheadline }} &middot; {% endif %}<strong>{{ post.title }}</strong><br><span style="color: #000000;">{{ post.year_composed }}/For {{ post.instrumentation }}</span></a></li>
{% endfor %}
</ul>