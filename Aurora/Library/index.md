---
title: Library
layout: aurora_library
---

<div class="jumbotron">
  <h1 class="display-4">Library</h1>
  <p class="lead">
    <div class="alert alert-warning" role="alert">
      <em>Library under construction</em>
    </div>
  </p>
  <hr class="my-4">
  <p>There is a lot more content coming soon.</p>
  <p class="lead">
    <a class="btn btn-primary btn-lg" href="/blog" role="button">Learn more</a>
  </p>
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
