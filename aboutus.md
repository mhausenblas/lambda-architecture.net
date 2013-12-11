---
layout: page
title : About us
header : About us
group: navigation
permalink: aboutus/index.html
---
{% include JB/setup %}

We're two Lambda Architecture believers who think the time has come to start
gathering and documenting material around it. This ranges from good practices
over case studies where and how the LA has been applied to review of components.

### Entries

<ul class="posts">
  {% for post in site.categories.organizational %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a> by <a href="http://twitter.com/{{ post.author_twitter }}">{{ post.author }}</a></li>
  {% endfor %}
</ul>
