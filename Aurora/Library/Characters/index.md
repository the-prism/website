---
title: Characters
description: A list of characters relevant to the aurora story.
layout: aurora_page
categories: [library]
---

{% for page in site.pages %}
{% if page.categories contains 'character' %}
<div class="item">
    <a href="{{page.url}}"><h3>{{page.title}}</h3></a>
    <p>{{page.description}}</p>
</div>
{% endif %}
{% endfor %}
