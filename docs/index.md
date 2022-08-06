# Welcome!
Hoser is framework that makes data pipelining open and easy. Data pipelining is a super common task but most solutions are limited, overly complex, or both. Hoser fills this need by providing a open library of connectors, a repo of community developed  pipeline examples, and simple tools to run and monitor your pipelines.

Hoser is built on the idea that data pipelines should be as easy as they are common. 

## What's Data Pipelining?
If you've worked in IT very long, you are all probably all too familiar with this problem: Data in one system must be moved to another. Often there are also operations that need to happen in the middle such as filtering, transformation, content enrichment, generating events.

A data pipeline is a set of processes or components used to ingest data and move it to a destiation or trigger actions on a target system.

For example, you may have documents in a MongoDB collection that have to be manipulated and exported to a legacy XML format, a set of CSV files in an Amazon S3 bucket have to be filtered and pushed to a SQL instance, or records scraped from web pages that need to be pushed to a Kafka topic to trigger an event if they contain specific content.

## Why another tool?
Some of you may be thinking *aren't there a dozen different tools for this already?* or *is this is yet another attempt at tooling for [enterprise integration patterns](https://www.enterpriseintegrationpatterns.com/) and [ETL](https://www.informatica.com/resources/articles/what-is-etl.html)*. 

To some degree, you're right. There are tools offered by [Informatica](https://www.informatica.com/), [Talend](https://www.talend.com/), [Snowflake](https://www.snowflake.com/), [JBoss Fuse](https://access.redhat.com/documentation/en-us/red_hat_jboss_fuse/6.2.1/html/getting_started/index) as well as some open source options like [Apache Camel](https://camel.apache.org/). However, just spend 10 minutes trying to use these tools and you'll find they are more complicated than they need to be, don't support  connectors for all your use cases, or cost a lot of money.

Hoser expands on the idea that data pipelines don't have to any more compolicated that a [series of unix pipes](https://adamdrake.com/command-line-tools-can-be-235x-faster-than-your-hadoop-cluster.html) and can be implemented this way without performance issues for most use cases!
