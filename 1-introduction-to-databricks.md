# Databricks Fundamentals Course Notes

## 1. Introduction to Data Management Platforms

### Data Warehouses
* **Data Warehouses**:
  * Pros
    * Great for structured data
    * Highly Performant
    * Schema controlled
  * Cons
    * Can be expensive
    * Cannot support modern applications
    * Note built for ML projects that depend on non-normalized schemas
  * Other Mentions
    * Designed for structured data with predefined schemas.
    * Optimized for OLAP (Online Analytical Processing).
    * Examples: Snowflake, Amazon Redshift, Google BigQuery.

### Data Lakes
* **Data Lakes**:
  * Pros
    * Support for all data use-cases
      * Structured, textual, other unstructured data
    * Flexible
      * Lacks schema enforcement and data consistency features.
    * Cost effective
  * Cons
    * Data can become messy (ie unnormalized schemas)
    * Historically not performant
    * Governance over the data in a data lake creates challenges with security
  * Other Mentions
    * Flexible storage of structured, semi*structured, and unstructured data.
    * Uses low*cost object storage (e.g., AWS S3, Azure Data Lake).
    * Common format: Parquet, ORC, JSON.
    * Data governance concerns
    * Governance over the data in a data lake creates challenges with security, and privacy enforcement due to the unstructured nature of the contents of a data lake
  * Issues
    *Lack of ACID transaction support
    * Lack of schema enforcement
    * Lake of integration with a data catalog
    * Too many small files

### Databricks Lakehouse
* **Lakehouse**:
  * A combined open architecture that combine data lake with the analytical power and controls of a data warehouse.
    * Features: ACID transactions, schema enforcement, unified batch and streaming.
  * Key technology: Delta Lake (open source via Apache spark)
  * Enables ML/AI use cases on a unified platform.

#### Delta Lake
  * Delta is open source data storage file format
    * Benefits:
      * ACID Transactions, Unified Batch and streaming
      * Schema Evolution
      * Table History
      * Time Travel