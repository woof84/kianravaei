---
layout: works
sidebar: right
show_meta: false
title: "Works"
subheadline: Choral
header: no
permalink: "/works-choral/"
---

{% for post in site.categories.works %}
{% if post.category_music == "Choral" %}
<div class="panel radius b20">
    <p style="text-align:left;"><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><span style="float:right;"> {{ post.year_composed }}/For {{ post.instrumentation }}</span></p>
</div>
{% endif %}
{% endfor %}