# Awesome-Big-Data-Frameworks

## Top Big Data Frameworks Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Distributed Processing, Cluster Orchestration & Open Data Platform Stacks*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Big Data Frameworks**. These tools enable organizations to process massive datasets across distributed clusters—from managed cloud services that abstract infrastructure away to open-source stacks you assemble yourself on Kubernetes or bare metal.



**Examples** include Cloudera, MapR, Databricks, Amazon EMR, Google Cloud Dataproc, Azure HDInsight, Snowflake, Starburst Galaxy, Teradata Vantage, and Qubole (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, distributed processing, and open data platform assembly—ideal for data engineers, platform teams, and organizations seeking transparent, vendor-independent big data infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Cloudera](https://www.cloudera.com/)**

  **The surviving enterprise Hadoop distribution** after the 2018 Cloudera-Hortonworks merger . **CDP (Cloudera Data Platform)** provides hybrid cloud data management with governance, security, and multi-function analytics. **Note**: Cloudera eliminated its free Community Edition in 2021 and increased prices significantly—a decision that drove many organizations to seek open-source alternatives .



- **[Databricks](https://www.databricks.com/)**

  **The lakehouse platform** built by the original creators of Apache Spark . **Delta Lake** for ACID transactions on data lakes . **Photon engine** for vectorized query execution . **Unity Catalog** for unified governance . **The dominant commercial platform** for data engineering and ML workloads, valued at **$134 billion** .



- **[Amazon EMR](https://aws.amazon.com/emr/)**

  **AWS's managed Hadoop/Spark service** . **EMR uses the open-source Apache distribution of Hadoop by default**, with support for MapR distribution if desired . **Automatic and fine-grained cluster sizing** with tight AWS ecosystem integration . **Strong dependence on AWS** limits multi-cloud flexibility.



- **[Google Cloud Dataproc](https://cloud.google.com/dataproc)**

  **Managed Apache Spark and Apache Hadoop service** . **Fast, easy to use, and low cost** with deep integration into Google Cloud . **The simplest path to managed Spark/Hadoop** on GCP .



- **[Azure HDInsight](https://azure.microsoft.com/en-us/products/hdinsight/)**

  **Microsoft's managed Hadoop service** supporting Spark, Hive, Kafka, HBase, and more . **Deep integration with Azure ecosystem** and cost-effective for existing Microsoft customers .



- **[Snowflake](https://www.snowflake.com/)**

  **The cloud data warehouse that defined the modern analytics stack** . **Separates storage and compute**—scale each independently . **Snowpark** for Python/Java/Scala . **Polaris Catalog** now supports Apache Iceberg—a strategic pivot toward open formats after years of vendor lock-in criticism .



- **[Starburst Galaxy](https://www.starburst.io/)**

  **Fully managed Trino service** for federated analytics . **Query across data lakes, databases, and warehouses** without data movement . **The commercial arm of the open-source Trino project** .



- **[Teradata Vantage](https://www.teradata.com/)**

  **Enterprise data platform** with **massively parallel processing** . **The most mature enterprise data warehouse**—decades of optimization for complex analytical workloads.



- **[Qubole](https://www.qubole.com/)**

  **Self-service platform for big data analytics** built on AWS, Microsoft, and Google Clouds . **Multi-cloud support** with unified interface and cost management . **Acquired by Idera** and no longer actively developed as a standalone platform.



## Open-Source GitHub Projects



- **[Apache Hadoop](https://github.com/apache/hadoop)**

  **The foundational distributed processing framework for large data sets across clusters** (Apache-2.0) . **HDFS** for distributed storage with horizontal scalability through data replication and node addition . **MapReduce** for batch processing . **YARN** for resource management . **The original big data stack** that spawned the entire ecosystem . **Note**: Hadoop is now primarily a storage layer—most processing has moved to Spark and Flink.



- **[Apache Spark](https://github.com/apache/spark)**

  **The unified analytics engine for large-scale data processing** (Apache-2.0) . **The most widely deployed open-source big data processing engine** . **Spark SQL** for structured data, **Spark Streaming** for real-time, **MLlib** for machine learning, **GraphX** for graphs . **Distributed in-memory processing** reduces disk access for iterative workloads . **The foundation of Databricks** and most modern data platforms.



- **[Apache Flink](https://github.com/apache/flink)**

  **Stateful computations over unbounded and bounded data** (Apache-2.0) . **The standard for stream processing** . **Event-time processing**, **exactly-once semantics**, **stateful operations**, and **SQL support** . **Reduces storage overhead by processing continuous streams** . **Operationally more complex** than batch frameworks but essential for real-time pipelines.



- **[Trino](https://github.com/trinodb/trino)**

  **Distributed SQL query engine for federated analytics** (Apache-2.0) . **Query across heterogeneous data sources**—HDFS, S3, relational databases, Cassandra, Kafka . **The open-source engine underlying Starburst Galaxy** . **Supports Apache Iceberg** natively . **The most flexible federated query engine**.



- **[Apache Kafka](https://github.com/apache/kafka)**

  **Distributed event streaming platform** (Apache-2.0) . **High throughput and low latency** for large-scale streams . **The standard for data ingestion** in modern data pipelines . **Requires expertise** to configure, operate, and maintain distributed streaming clusters.



- **[Apache Hive](https://github.com/apache/hive)**

  **Data warehouse software for reading, writing, and managing large datasets** (Apache-2.0) . **The original SQL-on-Hadoop solution** . **HiveQL**, partitioning, bucketing, and storage format abstraction . **Still widely used** for batch SQL workloads on HDFS.



- **[Apache HBase](https://github.com/apache/hbase)**

  **Distributed, scalable, big data store** (Apache-2.0) . **NoSQL database on top of HDFS** . **Random read/write access** to billions of rows . **The standard for real-time read/write access** to big data.



- **[Apache Airflow](https://github.com/apache/airflow)**

  **Platform to programmatically author, schedule, and monitor workflows** (Apache-2.0) . **The standard for data pipeline orchestration** . **Python-defined DAGs** with massive operator ecosystem .



- **[dbt](https://github.com/dbt-labs/dbt-core)**

  **Data build tool for analytics engineering** (Apache-2.0) . **Transform data in your warehouse** using SQL . **The standard for the "T" in ELT** . **Focused on transformation and testing**, requiring complementary orchestration tools.



- **[Trunk Data Platform (TDP)](https://github.com/TOSIT-IO/TDP)**

  **Open-source alternative to Cloudera after its community edition removal** (Apache-2.0) . **Developed by TOSIT (French association)** with contributors including **DGFIP, EDF, SNCF, and BPCE** . **Based approximately on HDP 3.1.5** . **TDP Manager** (Ansible-powered) replaces Ambari for deployment . **In production at DGFIP** since January 2025—migrating from a Cloudera deployment estimated at **€12 million** . **The most credible open-source Cloudera replacement** for organizations fleeing license costs.



- **[Stackable Data Platform](https://github.com/stackabletech)**

  **Kubernetes-native open-source data platform** (open-source components) . **Founded in Germany (2020) by former Cloudera consultants** after Cloudera eliminated its free tier and raised prices 5x . **Infrastructure-as-Code approach** with reproducible deployments . **Includes Apache Kafka, Spark, Trino, Druid, Superset, and NiFi** with automated certificate management via Secret Operator and Listener Operator . **Customers include the UK Ministry of Defence, Atruvia (German banking), and HUK (insurance)** . **The European sovereign alternative** to Databricks and Snowflake.



### Additional Strong Open-Source Options



- **[Apache Doris](https://github.com/apache/doris)** — MPP-based real-time analytical database (Apache-2.0) . **MySQL protocol compatible** with real-time ingestion and lakehouse federation.

- **[StarRocks](https://github.com/StarRocks/starrocks)** — High-performance OLAP database (Apache-2.0) . **Sub-second queries on data lake and warehouse**.

- **[ClickHouse](https://github.com/ClickHouse/ClickHouse)** — Fastest open-source column-oriented OLAP database (Apache-2.0) . **Sub-second queries on billions of rows**.

- **[Apache Iceberg](https://github.com/apache/iceberg)** — Open table format for huge analytic datasets (Apache-2.0) . **The emerging standard for lakehouse tables**.

- **[Delta Lake](https://github.com/delta-io/delta)** — Open-source storage framework for ACID transactions on data lakes (Apache-2.0) .

- **[Apache Hudi](https://github.com/apache/hudi)** — Streaming data lake platform (Apache-2.0) with upserts, deletes, and incremental processing.

- **[DuckDB](https://github.com/duckdb/duckdb)** — In-process analytical database (MIT) . **The SQLite of analytics**—runs anywhere, embedded.

- **[DuckLake](https://github.com/duckdb/ducklake)** — Open-source lakehouse format using SQL metadata (MIT) . **Challenges Iceberg and Delta Lake** by storing metadata in a relational database instead of file-based catalogs .

- **[Apache Bigtop](https://github.com/apache/bigtop)** — Packaging and testing framework for Apache Hadoop ecosystem (Apache-2.0) . **The reference for assembling open-source Hadoop stacks** .

- Community **n8n** workflows for data pipeline orchestration and cluster monitoring automation.



**Frameworks for building custom systems**: Combine **Apache Spark** for batch processing with **Apache Flink** for streaming, **Apache Hadoop HDFS** for storage, **Trino** for federated queries, **Apache Kafka** for ingestion, **dbt** for transformation, and **Apache Airflow** for orchestration—creating a fully self-hosted, enterprise-grade data platform that mirrors the architecture of Stackable and TDP.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Big data frameworks handling enterprise data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.

- **Open-source big data stacks are mature and production-ready.** Spark, Flink, Kafka, HDFS, and Trino are the building blocks of modern data platforms . **These are genuine alternatives to commercial platforms.**

- **The Cloudera exodus created a thriving open-source ecosystem.** After Cloudera eliminated its free Community Edition in 2021 and raised prices 5x, organizations like DGFIP, EDF, and SNCF built **Trunk Data Platform (TDP)** as an open-source alternative . German company **Stackable** emerged from the same frustration, now serving the UK Ministry of Defence and major European enterprises . **The open-source response to vendor lock-in is real and working.**

- **Assembly is the open-source trade-off.** Open-source tools are generally designed for specific purposes—Kafka for ingestion, Spark for processing, HDFS for storage, Airflow for monitoring . **You combine components yourself**, which requires advanced skills in integration, deployment, and maintenance.

- **Kubernetes is the modern substrate.** Stackable's Kubernetes-native architecture provides Infrastructure-as-Code reproducibility across development, test, and production . **This is the emerging standard** for assembling open-source data platforms.

- Self-hosted open-source solutions require proper cluster management, security hardening, and ongoing maintenance. **The "free" software has real operational costs**—plan for expertise, monitoring, and upgrade cycles.



---



**Made for data engineers, platform teams, and organizations building transparent big data solutions.**

Let's make Big Data Frameworks more open, data-driven, and sovereign.
