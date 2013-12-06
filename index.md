---
layout: page
title: Welcome to Lambda Architecture.
tagline: A repository of information, examples and good practices around the Lambda Architecture
---
{% include JB/setup %}

* Intro
* Examples
* Resources: slide decks, Dr Dobbs article, playground, etc.
* table with components for different layers

## Blog
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



