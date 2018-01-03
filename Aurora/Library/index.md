---
title: Library
layout: aurora_library
---

# Library

<div class="alert alert-warning" role="alert">
    <em>Library under construction</em>
</div>

<div class="card-columns">

{% for page in site.pages %}
{% if page.categories contains 'library' %}
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
