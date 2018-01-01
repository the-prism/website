---
title: Library
layout: aurora_page
---

*Library under construction*

{% for page in site.pages %}
{% if page.categories contains 'library' %}
<div class="item category">
    <a href="{{page.url}}"><h3>{{page.title}}</h3></a>
    <p>{{page.description}}</p>
</div>
{% endif %}
{% endfor %}
