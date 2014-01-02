---
layout: post
title: "Speed Components"
description: ''
category: components
tags: [Big Data, Lambda, stream processing, Apache]
author: "Michael Hausenblas"
author_twitter: mhausenblas
---
{% include JB/setup %}

## Stream Processing Frameworks

|Technology            |Does it fit            |Maturity               |Complexity     |Language       |Comments                  |
|----------------------|-----------------------|-----------------------|---------------|---------------|--------------------------|
|[Apache Storm][STORM] |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |&#9733;        |Clojure        | originates from Twitter  |
|[Apache Samza][SAMZA] |&#9733;&#9733;&#9733;  |&#9733;&#9733;         |&#9733;&#9733; |Scala/Java     | originates from LinkedIn |
|[Apache S4][S4]       |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;        |Java           | originates from Yahoo!   |


## Cloud-based  (XaaS) Offerings

|Technology         |Does it fit            |Maturity        |Complexity     |API     |Comments                |
|-------------------|-----------------------|----------------|---------------|--------|------------------------|
|[Kinesis][KINESIS] |&#9733;&#9733;&#9733;  |&#9733;&#9733;  |&#9733;&#9733; |Java    | introduced in 11/2013  |


## Further Resources

For an introduction into stream processing, have a look at a survey article on
[Data Stream and Complex Event Processing Systems][STREAMOVERVIEW].

If you're interested in doing machine learning over streams, check out Yahoo!'s
Scalable Advanced Massive Online Analysis ([SAMOA][SAMOA]). 

[Getting Started with Storm][GETTINGSTARTEDSTORM] is a hands-on guide into 
real-time data analysis with Storm, incl. a real-life example with Node.js and Redis.

The [Storm Applied][STORMAPPLIED] book provides a gentle introduction and in-depth
guidance for the advanced. *Note that as of 01/2014 this book is in its early days, 
only three chapters are available, online.*



[STORM]: http://storm-project.net/ "Storm: Distributed and fault-tolerant realtime computation"
[SAMZA]: http://samza.incubator.apache.org/ "Samza is a distributed stream processing framework"
[S4]: http://incubator.apache.org/s4/ "S4 is a distributed, scalable, fault-tolerant, pluggable platform that allows programmers to develop applications for processing continuous unbounded streams of data"
[KINESIS]: http://aws.amazon.com/kinesis/ "Amazon Kinesis is a fully managed service for real-time processing of streaming data at massive scale"
[STREAMOVERVIEW]: http://home.deib.polimi.it/margara/papers/survey.pdf "Processing Flows of Information: From Data Stream to Complex Event Processing"
[SAMOA]: http://yahoo.github.io/samoa/ "SAMOA is a distributed streaming machine learning framework that contains a programing abstraction for distributed streaming ML algorithms"
[GETTINGSTARTEDSTORM]: http://shop.oreilly.com/product/0636920024835.do "Getting Started with Storm: Continuous streaming computation with Twitter's cluster technology by Jonathan Leibiusky, Gabriel Eisbruch, Dario Simonassi"
[STORMAPPLIED]: http://manning.com/sallen/ "Strategies for real-time event processing by Sean T. Allen, Peter Pathirana, and Matthew Jankowski"