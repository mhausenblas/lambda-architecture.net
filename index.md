---
layout: home
title: Lambda Architecture
tagline: A repository dedicated to the Lambda Architecture (LA). We collect and publish examples and good practices around the LA.
---
{% include JB/setup %}


### Updates

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a> by <a href="http://twitter.com/{{ post.author_twitter }}">{{ post.author }}</a></li>
  {% endfor %}
</ul>

### What is the Lambda Architecture?

[Nathan Marz](https://twitter.com/nathanmarz) came up with the term
Lambda Architecture (LA) for a generic, scalable and fault-tolerant data
processing architecture, based on his experience working on distributed data
processing systems at Backtype and Twitter.

The LA aims to satisfy the needs for a robust system that is fault-tolerant,
both against hardware failures and human mistakes, being able to serve a wide 
range of workloads and use cases, and in which low-latency reads and updates are 
required. The resulting system should be linearly scalable, and it should scale out 
rather than up. 

Here's how it looks like, from a high-level perspective:

![LA overview](img/la-overview_small.png "LA overview")

1. All **data** entering the system is dispatched to both the batch layer and the speed layer for processing.
1. The **batch layer** has two functions: (i) managing the master dataset (an immutable, append-only set of raw data), and (ii) to pre-compute the batch views.
1. The **serving layer** indexes the batch views so that they can be queried in low-latency, ad-hoc way. 
1. The **speed layer** compensates for the high latency of updates to the serving layer and deals with recent data only.
1. Any incoming **query** can be answered by merging results from batch views and real-time views.


### Resources

* [Big Data](http://manning.com/marz/), book by Nathan Marz and James Warren
* [Applying the Big Data Lambda Architecture](http://www.drdobbs.com/database/applying-the-big-data-lambda-architectur/240162604), Dr. Dobb's article by Michael Hausenblas
* [The Lambda architecture: principles for architecting realtime Big Data systems](http://jameskinley.tumblr.com/post/37398560534/the-lambda-architecture-principles-for-architecting), blog post by James Kinley
* [Lambda Architecture: Achieving Velocity and Volume with Big Data](http://www.semantikoz.com/blog/lambda-architecture-velocity-volume-big-data-hadoop-storm/), article by Christian Prokopp


### Who is behind this?

See the [about us](aboutus/) section for details.