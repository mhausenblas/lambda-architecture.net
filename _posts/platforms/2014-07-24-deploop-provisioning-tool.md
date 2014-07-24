---
layout: post
title: "Deploop: A Lambda Architecture Provisioning Tool"
description: 'Deploop is a tool for provisioning, managing and monitoring Apache Hadoop clusters focused in the Lambda Architecture.'
category: platforms
tags: [Deploop, Ambari, Lambda, Deployment]
author: "Javi Roman"
author_twitter: javiromanredoop
---
{% include JB/setup %}

## Overview

Deploop is a tool for LA clusters deployments. 

Deploop system is based on three software components:

* The Deploop engine: This is a Ruby application used for take the control of the 
cluster layers. With this command line tools, you can bootstrap a new cluster 
layer (batch layer, speed layer, serving layer), query the layer, start, stop o 
whatever.

* The Deploop Puppet Enviroments Catalog: The configurations of these complex 
architectures are handle by means of Puppet, a set of Puppet recipes are the core 
of the architecture.

* The Deploop Mcollective Agent: The orchestration engine Marionette Collective 
is the other core component in the Deploop architecture. The cluster operations 
are handle by means of this components and by means of a special MCollective 
agent: mcollective-deploop-agent plugin.

* The Deploop GUI: This is a Ruby on Rails application in development, 
it's a front end of the CLI engine.

## Usage examples

    deploop -f conf/cluster.json --deploy batch

    deploop -f conf/cluster.json --deploy batch,speed,bus,serving

    deploop --cluster production --layer batch --stop

    deploop --cluster production --layer batch --start

## Resources

* [The Deploop Project Page](http://deploop.github.io/)
* [The GitHub repository](https://github.com/deploop)
* [The Deploop Puppet Enviroments Catalog](https://github.com/deploop/deploop-environments)

