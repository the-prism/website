---
title: Characters
description: A list of characters relevant to the aurora story.
layout: aurora_page
categories: [library]
---

<div>
{% for page in site.pages %}
{% if page.categories contains 'character' %}
<a href="{{page.url}}" class="category">
    <div class="item">
        <h3>{{page.title}}</h3>
        <p>{{page.description}}</p>
    </div>
</a>
{% endif %}
{% endfor %}
</div>