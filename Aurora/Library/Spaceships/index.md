---
title: Spaceships
description: List of spaceships
categories: [library]
layout: aurora_page
---

*Under construction*

<div>
{% for page in site.pages %}
{% if page.categories contains 'spaceship' %}
<a href="{{page.url}}" class="category">
    <div class="item">
        <h3>{{page.title}}</h3>
        <p>{{page.description}}</p>
    </div>
</a>
{% endif %}
{% endfor %}
</div>