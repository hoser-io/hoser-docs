# Introduction
Hoser is framework that makes data pipelining open and easy. Data pipelining is a super common task and existing solutions are limited, overly complex, or both. Hoser fills this need by having a open library of connectors, a repo of community developed and shareable pipeline examples, and providing a framework to run and monitor your pipelines.

Hoser is built on the idea that data pipelines should be as easy as they are common. 

## What's Data Pipelining?
The majority of us who have had to work with software in a organization are all too familiar with this problem: Data in one system has to be moved to another. Many times there's also one or more operations happening in the middle such as filtering, map reduce, transformation, or content enrichment. A system that moves data with potential operations in the middle is a data pipeline. 

For example, documents in a MongoDB collection that have to be manipulated and exported to a legacy XML format, a set of CSV files in an Amazon S3 bucket have to be filtered and pushed to a SQL instance, or a couple of records from some scraped web pages need to be pushed to a Kafka topic. 

## A Re-invented Wheel?
Some of you may be thinking *hasn't this been done a dozen time already?* or *so this is yet another attempt at tooling for [enterprise integration patterns](https://www.enterpriseintegrationpatterns.com/) and [ETL](https://www.informatica.com/resources/articles/what-is-etl.html)*, and to some degree you'd be right. There are tools offered by [Informatica](https://www.informatica.com/), [Talend](https://www.talend.com/), [Snowflake](https://www.snowflake.com/), [JBoss Fuse](https://access.redhat.com/documentation/en-us/red_hat_jboss_fuse/6.2.1/html/getting_started/index) as well as some open source options like [Apache Camel](https://camel.apache.org/). However, spend 10 minutes trying to use these tools and find they are either a) more complicated than they need to be b) don't support the connectors for all our use cases or c) cost a lot of money.

Hoser expands on the novel idea that for most use cases, data pipelines don't have to any more compolicated that a [series of unix pipes](https://adamdrake.com/command-line-tools-can-be-235x-faster-than-your-hadoop-cluster.html), and can be done so without any loss of performance!
