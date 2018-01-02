---
title: Characters
description: A list of characters relevant to the aurora story.
layout: aurora_library
categories: [library]
---

<div class="card-columns">

{% for page in site.pages %}
{% if page.categories contains 'character' %}
<div class="card">
  <div class="card-body">
    <h5 class="card-title">{{page.title}}</h5>
    <p class="card-text">{{page.description}}</p>
    <a href="{{page.url}}" class="btn btn-primary">View</a>
  </div>
</div>
{% endif %}
{% endfor %}

</div>
