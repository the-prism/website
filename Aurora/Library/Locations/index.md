---
title: Locations
description: List of aurora locations
categories: [library]
layout: aurora_library
---

*Under construction*

<div class="card-columns">

{% for page in site.pages %}
{% if page.categories contains 'location' %}
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
