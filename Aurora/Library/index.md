---
title: Library
layout: aurora_library
---

*Library under construction*

<div>
{% for page in site.pages %}
{% if page.categories contains 'library' %}
<a href="{{page.url}}" class="category">
    <div class="item">
        <h3>{{page.title}}</h3>
        <p>{{page.description}}</p>
    </div>
</a>
{% endif %}
{% endfor %}
</div>