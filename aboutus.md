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


### Nathan Bijnens

>  Nathan is a developer with a passion for great code, the web and Big Data. 
>  He's interested in programming and system administration, especially where
>  they meet, from scaling platforms to designing the architecture of new and 
>  existing products and everything in between.
>  He's focused on data analysis and building Big Data Applications. Using Hadoop, 
>  in combination with Hadoop Pig, Hive and Cascading. Nathan follows the rise of 
>  real-time big data closely, actively developing applications on top of Storm. 
>  And designing Lambda-like architectures. 

### Michael Hausenblas

>  Michael is [MapR's](http://mapr.com) Chief Data Engineer where he's helping people to tap the potential of Big Data. 
>  He's bridging the technical (architecture, reliability, scalability, etc.) and the business side (SLAs, RoI, TCO, etc.).
>  His background is in large-scale data integration, the Internet of Things, and Web
>  applications and he's experienced in advocacy and standardisation. Michael has been
>  using NoSQL datastores and Hadoop ecosystem components since 2008. Nowadays he's 
>  sharing his experience with the Lambda Architecture, distributed systems and 
>  polyglot persistence through blog posts and public speaking engagements. 
>  Last but not least, Michael is contributing to [Apache Drill](http://incubator.apache.org/drill/),
>  a distributed system for interactive, ad-hoc analysis and query of large-scale datasets.


#### Organizational Updates

<ul class="posts">
  {% for post in site.categories.organizational %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a> by <a href="http://twitter.com/{{ post.author_twitter }}">{{ post.author }}</a></li>
  {% endfor %}
</ul>
