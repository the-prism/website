---
title: Factions
description: List of factions in the aurora universe.
categories: [library]
layout: aurora_library
---

*Under construction*

<div>
{% for page in site.pages %}
{% if page.categories contains 'faction' %}
<a href="{{page.url}}" class="category">
    <div class="item">
        <h3>{{page.title}}</h3>
        <p>{{page.description}}</p>
    </div>
</a>
{% endif %}
{% endfor %}
</div>