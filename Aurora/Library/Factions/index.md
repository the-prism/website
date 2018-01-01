---
title: Factions
description: List of factions in the aurora universe.
categories: [library]
layout: aurora_page
---

*Under construction*

<div>
{% for page in site.pages %}
{% if page.categories contains 'faction' %}
<a href="{{page.url}}" class="category">
    <div class="item">
        <h5>{{page.title}}</h5>
        <p>{{page.description}}</p>
    </div>
</a>
{% endif %}
{% endfor %}
</div>