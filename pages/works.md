---
layout: page
show_meta: false
title: "List of works"
subheadline: "yup, this is it"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/works/"
---

{% for post in site.categories.works %}
<div class="panel radius b20">
    <p><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> ({{ post.year_composed }}) for {{ post.instrumentation }}</p>
</div>
{% endfor %}
