---
layout: post
title: "Batch Components"
description: ''
category: components
tags: [Big Data, Lambda, Hadoop]
author: "Michael Hausenblas"
author_twitter: mhausenblas
---
{% include JB/setup %}

## Processing Frameworks

|Technology             |Does it fit            |Maturity               |Ease of use            |Language                 |Platforms      |Comments                          |
|-----------------------|-----------------------|-----------------------|-----------------------|-------------------------|---------------|----------------------------------|
|[Hadoop MapReduce][MR] |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |&#9733;                |Java                     |Hadoop         | Very low-level, not re-usable   |
|[Spark][SPARK]         |&#9733;&#9733;&#9733;  |&#9733;&#9733;         |&#9733;&#9733;&#9733;  |Scala, Java, Python      |Spark          | In-memory|
|[Hive][HIVE]           |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |HiveQL, Java             |Hadoop         | Support planned for Tez |
|[Spark SQL][SPARKSQL]  |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;&#9733;         |SQL, Scala, Java, Python |Spark          | Successor of Shark |
|[Pig][PIG]             |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |&#9733;&#9733;&#9733;  |Pig Latin, Java          |Hadoop         | Support planned Tez|
|[Spork][SPORK]         |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;&#9733;&#9733;  |Pig Latin, Java          |Spark          | |
|Cascading/Scalding     |&#9733;&#9733;&#9733;  |&#9733;&#9733;         |&#9733;&#9733;         |Java, Scala              |Hadoop         | |
|Cascalog               |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;                |Clojure                  |Hadoop         | |
|Crunch/SCrunch        |&#9733;&#9733;&#9733;  |&#9733;&#9733;         |&#9733;                |Java, Scala              |Hadoop         | Support planned for Spark and Tez |
|Pangool                |&#9733;&#9733;&#9733;  |&#9733;                |&#9733;                |Java                     |Hadoop         | |


[MR]: http://hadoop.apache.org/docs/stable/api/org/apache/hadoop/mapreduce/package-summary.html "Java doc: org.apache.hadoop.mapreduce"
[SPARK]: https://spark.apache.org/docs/latest/ "Entry point for API Docs"
[HIVE]: http://hive.apache.org/ "Apache Hive project"
[SPARKSQL]: https://spark.apache.org/docs/latest/sql-programming-guide.html "Spark SQL Programming Guide"
[PIG]: http://pig.apache.org/ "Apache Pig project"
[SPORK]: https://github.com/mateiz/spork "Pig for Spark"