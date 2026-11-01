### Hi, I'm Tan

**Lead Data Engineer, 8+ years. I take AI from prototype to production on top of data platforms that hold up.**

I have built data platforms for retail, healthcare and e-commerce: batch and streaming
pipelines (Spark, Kafka, Airflow, dbt), lakehouses on Databricks and Snowflake, and the
governance and data quality that keep them trustworthy. Lately I build the AI layer on top:
knowledge graphs that ground RAG applications, LLM extraction pipelines with schema-validated
output, and the evals that tell you whether a change actually made things better.

Open to AI Engineer, Forward Deployed Engineer and Data Engineer roles, remote or relocation.

#### Open source

| Project | What it shows |
|---|---|
| [**filings-copilot**](https://github.com/tantn89/filings-copilot) · [live demo](https://filings-copilot.vercel.app) | Agentic research assistant over SEC 10-K filings. Numbers come from audited XBRL data through guarded text-to-SQL, explanations from hybrid search with citations. 20/20 on a deterministic eval at $0.010 per question; deployed on Cloud Run and Vercel with spend caps; security-reviewed with every finding kept as a regression test. |
| [**regressgate**](https://github.com/tantn89/regressgate) · [PyPI](https://pypi.org/project/regressgate/) · [docs](https://tantn89.github.io/regressgate/) | Fails CI on real LLM eval regressions, not on noise: repeated trials, a stratified permutation test and per-case exact tests. In simulation, "fail on any drop" raises false alarms on 44% of unchanged pull requests; regressgate on 2%, while catching 92% of single broken cases. |
| [**realtime-lakehouse**](https://github.com/tantn89/realtime-lakehouse) | Streaming lakehouse over live Wikipedia edits: Redpanda, Spark Structured Streaming, Iceberg, dbt, Dagster. A CI crash test kills the stream mid-backlog and proves 0 duplicates and 0 gaps; freshness p95 about 20 s up to 9.6k events/s; a 2-hour AWS run on S3 + Glue + Athena handled 868k events for about $0.52. |

#### Stack

**AI / LLM:** Claude & OpenAI-compatible APIs, tool-use agents, RAG, MCP, evals<br>
**Data:** Python, SQL, Spark, Kafka, Flink, dbt, Airflow, Dagster, DuckDB, Debezium CDC<br>
**Platforms:** Databricks (Delta, Unity Catalog, Feature Store), Snowflake, BigQuery, Redshift, PostgreSQL<br>
**Cloud & ops:** AWS, Azure, GCP, Docker, Kubernetes, Terraform, GitHub Actions

Certified: Google Professional Machine Learning Engineer · Microsoft Azure Administrator Associate · Oracle Database SQL Associate

#### Contact

Telegram: [@tanngoctr](https://t.me/tanngoctr)
