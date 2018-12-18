---
layout: default
title: Home
---

<div class="header200px" style="background-image: url(/website/images/head.jpg);">
&nbsp;
</div>

## Bienvenue sur the-prism.github.io,

Vous trouverez plusieurs de mes projets sur ma page personnelle github ainsi que quelques articles sur mon blog.

## Projets

* Jekyll theme based on bootstrap _it's the theme used on this page_: <https://github.com/the-prism/Jekyll-Bootstrap>
* Command line application for handling batch files with pandoc : <https://github.com/the-prism/Pandoc-Tools>
* UI wrapper for pandoc in windows and java (_incomplete_) : <https://github.com/the-prism/Pandoc-UI>
* Windows application for dungeons and dragons : <https://github.com/the-prism/DungeonsAndDragons>
* Fitness Habits, _prototype android app for fitness tracking_ : <https://github.com/the-prism/FitnessHabits>
* Ping a heroku server to check if it's up : <https://github.com/the-prism/HerokuPing>
* Dino Revenge 3D : <https://github.com/the-prism/dino-revenge>
* Pokédex witten in PHP : <https://github.com/the-prism/php-pokedex>
* C++ shell emulator : <https://github.com/the-prism/cpp-shell-emulator>
* C linked list example : <https://github.com/the-prism/C-linked-list>
* Java matrix calculator : <https://github.com/the-prism/Java-Matrix-Calculator>
* Windows Universal Application : <https://github.com/the-prism/UWP-Spy-Project>

<h1>Blog</h1>

<div class="posts">
  {% for post in paginator.posts %}
    <article class="post">

      <h3><a href="{{ site.baseurl }}{{ post.url }}" class="link-unstyled">{{ post.title }}</a></h3>

      <div class="entry">
        {{ post.excerpt }}  
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&laquo; Prev</a>
  {% else %}
    <span>&laquo; Prev</span>
  {% endif %}

  {% for page in (1..paginator.total_pages) %}
    {% if page == paginator.page %}
      <em>{{ page }}</em>
    {% elsif page == 1 %}
      <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">{{ page }}</a>
    {% else %}
      <a href="{{ site.paginate_path | prepend: site.baseurl | replace: '//', '/' | replace: ':num', page }}">{{ page }}</a>
    {% endif %}
  {% endfor %}

  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Next &raquo;</a>
  {% else %}
    <span>Next &raquo;</span>
  {% endif %}
</div>
{% endif %}
