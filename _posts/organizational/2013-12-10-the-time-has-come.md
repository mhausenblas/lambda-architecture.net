---
layout: post
title: "Why are we doing this and why are we doing this now?"
description: ''
category: organizational
tags: []
author: "Michael Hausenblas"
author_twitter: mhausenblas
---
{% include JB/setup %}

You might have heard about the Lambda Architecture (LA) already.
[Nathan Marz](https://twitter.com/nathanmarz) came up with this term for a
generic data processing architecture, based on his experience working on
distributed data processing systems at Backtype and Twitter.
Really, people have been architecting and deploying LA-like systems for decades.
In a sense, the LA is an extended [event sourcing](http://martinfowler.com/eaaDev/EventSourcing.html)
system, taking into account streaming data, at scale.

We (Nathan Bijnens and Michael Hausenblas) have been advocating the LA for a bit
now, deploying it at customers, talking with colleagues at events about it and
trying to collect material that helps people interested in the LA to do their
job. This site is dedicated to document known cases of where the LA has been applied
and sharing the lessons learned that come with it. Be it in terms of component
selection, workflow optimization or query mediation. 

Last but not least, this site depends on **you**. Yes, you. Because unlike the
LA, neither Nathan nor I scale well, so we depend on [community contributions](../../contribute/):
You built a system according to the LA? Great, let us know. Gave a talk on the LA?
Wonderful, why not issuing a pull request? Have a project up on GitHub that contributes
to the LA? Brilliant, [raise an issue](https://github.com/mhausenblas/lambda-architecture.net/issues)
here and we'll add it, eventually.

And now thanks for your time and enjoy the LA as much as we do!