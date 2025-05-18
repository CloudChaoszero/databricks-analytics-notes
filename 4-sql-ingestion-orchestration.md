# Databricks Fundamentals Course Notes

## 6. Data Warehousing

- **Databricks SQL**:
  - Native support for BI tools (Tableau, Power BI, Looker).
  - Materialized views and result caching.
  - Query federation with external databases.

- **Performance Optimizations**:
  - Z-ordering for query pruning.
  - Delta Lake file compaction (OPTIMIZE).
  - Query profiling and cost-based optimizer (CBO).

## 7. Orchestration

- **Databricks Workflows**:
  - Supports notebooks, Python scripts, JARs, and SQL tasks.
  - Retry policies, success/failure triggers, email alerts.
  - REST API and CLI support.

- **Delta Live Tables**:
  - Declarative pipeline syntax.
  - Supports SCD Type 1/2 and CDC patterns.
  - Auto lineage and quality constraints via expectations.

## 8. ETL and Real-Time Analytics

- **Streaming Support**:
  - Structured Streaming API in PySpark and Scala.
  - Trigger options: continuous, once, and micro-batch.
  - Supports Kafka, Auto Loader, and Delta as sources.

- **Auto Loader**:
  - Efficient file discovery using cloud events.
  - Scales to millions of files with low-latency ingestion.

- **ETL Best Practices**:
  - Use Delta Live Tables for quality and observability.
  - Optimize data layout (partitioning, Z-ordering).
  - Monitor pipelines using metrics and lineage.