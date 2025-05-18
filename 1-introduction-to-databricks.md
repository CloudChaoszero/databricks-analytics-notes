# Databricks Fundamentals Course Notes

## 1. Introduction to Data Management Platforms

- **Data Warehouses**:
  - Designed for structured data with predefined schemas.
  - Optimized for OLAP (Online Analytical Processing).
  - Examples: Snowflake, Amazon Redshift, Google BigQuery.
  - Limitations: not well-suited for real-time or unstructured data.

- **Data Lakes**:
  - Flexible storage of structured, semi-structured, and unstructured data.
  - Uses low-cost object storage (e.g., AWS S3, Azure Data Lake).
  - Lacks schema enforcement and data consistency features.
  - Common format: Parquet, ORC, JSON.
  - Data governance concerns
    - Governance over the data in a data lake creates challenges with security, and privacy enforcement due to the unstructured nature of the contents of a data lake
  - Issues
    -Lack of ACID transaction support
    - Lack of schema enforcement
    - Lake of integration with a data catalog
    - Too many small files
- **Lakehouse Architecture**:
  -a combined open architecture that combine data lake with the analytical power and controls of a data warehouse.
  - Merges advantages of data lakes and warehouses.
  - Features: ACID transactions, schema enforcement, unified batch and streaming.
  - Key technology: Delta Lake.
  - Enables ML/AI use cases on a unified platform.