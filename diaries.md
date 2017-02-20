---
layout: page
title: Civil War Diaries
---

This is a list of all the Civil War Diaries: 

<ul>
{% for text in site.texts %}
{% if text.categories contains 'civilwardiaries' %}
    <li class="post-title"><a href="{{ site.baseurl }}{{ text.url }}">{{ text.title }}</a></li>
{% endif %}
{% endfor %}

</ul>

