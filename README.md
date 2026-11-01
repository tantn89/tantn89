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
| [**warehouse-mcp**](https://github.com/tantn89/warehouse-mcp) · [PyPI](https://pypi.org/project/warehouse-mcp/) | MCP server that gives AI agents governed, read-only access to DuckDB, Postgres and BigQuery: semantic layer, SQL guard, row policies, PII pseudonymized at the source, audit log, cost caps. 104 red-team attempts with 0 leaks on each engine; identical answers on all three engines; a Claude agent scored 78/78 at $0.0016 per question, gated in CI by regressgate. Includes a deployment playbook for rolling it out at a customer. |
| [**uplift-experimentation**](https://github.com/tantn89/uplift-experimentation) | A/B testing and uplift modeling with statistics that survive scrutiny. Peeking at a naive t-test gives 24.8% false positives against 0.98% for mSPRT. CUPED is reported honestly: −2.6% variance on Hillstrom, 0.51 variance ratio when the covariate is strong. Uplift models trained on 13.98M Criteo rows on Databricks: targeting the top 10% gives 63.7 extra visits per 1,000 contacts against 10.3 for treating everyone. The champion is chosen by a pre-declared rule, registered in Unity Catalog and served by FastAPI on Cloud Run, with drift checks and a CI metric gate. |

#### Stack

**AI / LLM:** Claude & OpenAI-compatible APIs, tool-use agents, RAG, MCP, evals<br>
**Data:** Python, SQL, Spark, Kafka, Flink, dbt, Airflow, Dagster, DuckDB, Debezium CDC<br>
**Platforms:** Databricks (Delta, Unity Catalog, Feature Store), Snowflake, BigQuery, Redshift, PostgreSQL<br>
**Cloud & ops:** AWS, Azure, GCP, Docker, Kubernetes, Terraform, GitHub Actions

Certified: Google Professional Machine Learning Engineer · Microsoft Azure Administrator Associate · Oracle Database SQL Associate

#### Contact

Telegram: [@tanngoctr](https://t.me/tanngoctr)
