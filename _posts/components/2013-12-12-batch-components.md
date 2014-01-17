---
layout: post
title: "Batch Components"
description: ''
category: components
tags: [Big Data, Lambda, Hadoop]
author: "Nathan Bijnens"
author_twitter: nathan_gs
---
{% include JB/setup %}

## Processing Frameworks

|Technology                                                |Does it fit            |Maturity               |Easyness of use        |Language       |Platforms      |Comments       |
|----------------------------------------------------------|-----------------------|-----------------------|-----------------------|---------------|---------------|---------------|
|Hadoop MapReduce                                          |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |&#9733;                |Java           |Hadoop         |		   |
|Spark MapReduce					   |&#9733;&#9733;&#9733;  |&#9733;		   |&#9733;&#9733;	   |Scala	   |Spark	   |		   |
|Pig                                                	   |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |Pig Latin, Java|Hadoop         |Support planned for Spark and Tez		   |
|Hive                                               	   |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |HiveQL, Java   |Hadoop         |Support planned for Tez. Spark's clone is "Shark"               |
|Cascading / Scalding                                      |&#9733;&#9733;&#9733;  |&#9733;&#9733;         |&#9733;&#9733;         |Java, Scala    |Hadoop         |               |
|Cascalog                                                  |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;                |Clojure        |Hadoop         |               |
|Crunch	/ SCrunch					   |&#9733;&#9733;&#9733;  |&#9733;&#9733;	   |&#9733;		   |Java, Scala    |Hadoop         |Support planned for Spark and Tez               |
|Pangool						   |&#9733;&#9733;&#9733;  |&#9733;		   |&#9733;		   |Java	   |Hadoop	   |               |

## Batch View Databases

|Technology                                                |Does it fit            |Maturity               |Easyness of use        |API Language   |Comments       |
|----------------------------------------------------------|-----------------------|-----------------------|-----------------------|---------------|---------------|
|ElephantDB                                                |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;                |Clojure        |               |
|SploutSQL                                                 |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;&#9733;         |Java	   |	           |
|Voldemort (with a ReadOnly backend)                       |&#9733;&#9733;         |&#9733;&#9733;         |&#9733;&#9733;         |Java	   |               |
|HBase (bulk loading)					   |&#9733;&#9733;	   |&#9733;&#9733;	   |&#9733;&#9733;	   |Java  	   |		   |


