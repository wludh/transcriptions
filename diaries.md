---
layout: page
title: Civil War Diaries
---

This is a list of all the Civil War Diaries: 

<ul>

{% for page in site.categories[civilwardiaries] %}
           <li class="post-title"><a href="{{ page.permalink }}">{{ page.title }}</a></li>
{% endfor %}

</ul>

