•	Engineered a metadata-driven ingestion layer using Jinja-templated dbt models and config dictionaries, enabling dynamic table generation that eliminated repetitive static pipeline configs.
•	Implemented lightweight CDC via cursor-based query tracking on a Postgres source (ghost.build), avoiding Debezium/Kafka overhead while maintaining incremental load integrity.
•	Designed ephemeral dbt staging models for transient dimension transformations, reducing materialization costs without persisting intermediate tables.
•	Containerized Airflow via Docker Compose for a fully reproducible local dev environment, removing dependency on managed services like Cloud Composer or MWAA.
•	Ingested unstructured product review data from S3 into a Delta Lake bronze layer via Databricks external locations, establishing the foundation for a medallion architecture.
