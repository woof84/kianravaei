---
layout: works
sidebar: right
show_meta: false
title: "Works"
subheadline: Chamber Music
header: no
permalink: "/works-chamber-music/"
---

{% for post in site.categories.works %}
{% if post.category_music == "Chamber Music" %}
<div class="panel radius b20">
    <p style="text-align:left;"><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><span style="float:right;"> {{ post.year_composed }}/For {{ post.instrumentation }}</span></p>
</div>
{% endif %}
{% endfor %}