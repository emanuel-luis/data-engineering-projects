# Data engineering projects

An index of my public data-engineering repositories, all built on open or synthetic data. The
badges show each project's CI on `main`.

The [profile README](https://github.com/emanuel-luis) is the canonical overview, with more detail
per project, the publications and the open-source contributions. This page only lists the
repositories; if the two ever disagree, the profile is right. When a project is added or renamed,
update the profile first, then this list.

## Ingestion

| Project | What it does | CI |
| --- | --- | --- |
| [books-scraping](https://github.com/emanuel-luis/books-scraping) | Re-runnable crawl of the Books to Scrape sandbox into raw HTML, validated Parquet and a DuckDB serving layer. | [![CI](https://github.com/emanuel-luis/books-scraping/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/books-scraping/actions/workflows/ci.yml) |
| [ecommerce-scraping](https://github.com/emanuel-luis/ecommerce-scraping) | Scrapy crawler for three Brazilian fashion stores that reads product JSON-LD into Parquet and DuckDB views. | [![CI](https://github.com/emanuel-luis/ecommerce-scraping/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/ecommerce-scraping/actions/workflows/ci.yml) |
| [ingestion-toolkit](https://github.com/emanuel-luis/ingestion-toolkit) | CLI that turns validated ingestion configs (full scan, incremental watermark, CDC) into Airflow 3 DAGs. | [![CI](https://github.com/emanuel-luis/ingestion-toolkit/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/ingestion-toolkit/actions/workflows/ci.yml) |
| [mssql-cdc-pyspark](https://github.com/emanuel-luis/mssql-cdc-pyspark) | PySpark streaming source for SQL Server CDC with a `finalized_until` completeness signal. [Docs](https://emanuel-luis.github.io/mssql-cdc-pyspark/), [PyPI](https://pypi.org/project/mssql-cdc-pyspark/). | [![CI](https://github.com/emanuel-luis/mssql-cdc-pyspark/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/mssql-cdc-pyspark/actions/workflows/ci.yml) |

## Streaming and CDC

| Project | What it does | CI |
| --- | --- | --- |
| [cdc-streaming-demo](https://github.com/emanuel-luis/cdc-streaming-demo) | Postgres changes through Debezium and Kafka (Protobuf) into Delta Lake with Spark Structured Streaming, then dbt-duckdb marts. | [![CI](https://github.com/emanuel-luis/cdc-streaming-demo/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/cdc-streaming-demo/actions/workflows/ci.yml) |
| [kafka-streaming-lakehouse](https://github.com/emanuel-luis/kafka-streaming-lakehouse) | Avro events through Kafka into Apache Iceberg bronze, silver and gold, queried with Trino. | [![CI](https://github.com/emanuel-luis/kafka-streaming-lakehouse/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/kafka-streaming-lakehouse/actions/workflows/ci.yml) |

## Lakehouse and modeling

| Project | What it does | CI |
| --- | --- | --- |
| [de-lakehouse-pipeline](https://github.com/emanuel-luis/de-lakehouse-pipeline) | Polars ingestion and dbt marts on DuckDB, run by Airflow 3 through Astronomer Cosmos. [dbt docs and Elementary report](https://emanuel-luis.github.io/de-lakehouse-pipeline/). | [![CI](https://github.com/emanuel-luis/de-lakehouse-pipeline/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/de-lakehouse-pipeline/actions/workflows/ci.yml) |
| [vaccine-warehouse](https://github.com/emanuel-luis/vaccine-warehouse) | Kimball-style vaccination warehouse built with dbt, plus a live speed layer (Spring Boot API) and a React dashboard. | [![CI](https://github.com/emanuel-luis/vaccine-warehouse/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/vaccine-warehouse/actions/workflows/ci.yml) |

## ML pipelines

| Project | What it does | CI |
| --- | --- | --- |
| [covid19-xray-pipeline](https://github.com/emanuel-luis/covid19-xray-pipeline) | DVC pipeline for COVID-19 chest X-ray classification with leakage-safe splits, handcrafted features and a ResNet-18. | [![CI](https://github.com/emanuel-luis/covid19-xray-pipeline/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/covid19-xray-pipeline/actions/workflows/ci.yml) |
| [necrohub](https://github.com/emanuel-luis/necrohub) | Synthetic pt-BR necropsy reports: generation, de-identification, fine-tuned encoders and pgvector retrieval. | [![CI](https://github.com/emanuel-luis/necrohub/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/necrohub/actions/workflows/ci.yml) |

## Applications

| Project | What it does | CI |
| --- | --- | --- |
| [bank-credit](https://github.com/emanuel-luis/bank-credit) | Credit-request workflow with an append-only event log, SLA analytics in SQL views and contract-checked exports. | [![CI](https://github.com/emanuel-luis/bank-credit/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/emanuel-luis/bank-credit/actions/workflows/ci.yml) |

## License

[MIT](LICENSE).
