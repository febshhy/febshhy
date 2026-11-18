# febshhy

**Non-deterministic rule-based expert system software engineer**  
(a.k.a. AI `.md` engineer)

I’m interested in distributed systems, high-volume data, and figuring out where the milliseconds went. I like following the whole path from an event coming in to a number showing up on a dashboard.

```text
AI limit utilization  [██████████] 100%  <- the only SLO I've never missed
```

## What I’m building

### Heimdall for Codex

Heimdall helps Codex trace affected code paths, keep changes focused, and report what it verified.

[Repository](https://github.com/febshhy/heimdall-codex) · [How it works](https://github.com/febshhy/heimdall-codex/blob/main/marketing/HOW_IT_WORKS.md) · [Engineering playbook](https://github.com/febshhy/heimdall-codex/blob/main/marketing/ENGINEERING_PLAYBOOK.md)

### Mimir for Codex CLI

Mimir helps Codex CLI trace data from source records to dashboards or ML outputs and verify results against known records.

[Repository](https://github.com/febshhy/mimir-codex) · [Captured revenue example](https://github.com/febshhy/mimir-codex/blob/main/marketing/HOW_IT_WORKS.md#example-captured-revenue-from-source-to-dashboard) · [Data playbook](https://github.com/febshhy/mimir-codex/blob/main/marketing/DATA_PLAYBOOK.md)

## What I like working on

- **Distributed systems.** What happens to the rest of the system when one dependency gets slow? Where do the retries pile up?
- **Data engineering and BI.** I like working across ingestion, modeling, and dashboards. If a number changes, I want to be able to trace it back to the events and transformations that produced it.
- **Performance and operations.** I like the detective work of finding which part of a request is slow, then checking whether the fix made a difference.

## Rule base

### Writing and profiling

| IF | THEN |
| --- | --- |
| It needs a service | Go |
| It needs a script | Python or Bash |
| It needs numerical or columnar work | NumPy, JAX, or Polars |
| It’s slow | pprof for Go, Chrome DevTools for the browser |

### Storing and moving data

| IF | THEN |
| --- | --- |
| It fits in one file | SQLite for the app, DuckDB for the analysis |
| It needs a database server | Postgres for transactions, ClickHouse for analytics |
| It needs a batch pipeline | Airflow for scheduling, dbt for SQL transformations, Spark for distributed processing |
| It needs an event stream | Redpanda |
| It needs a dashboard | Metabase or Power BI |

### Deploying and operating

| IF | THEN |
| --- | --- |
| It needs to run somewhere | systemd for a service on one host, Kubernetes for workloads on a cluster |
| It needs infrastructure | OpenTofu or Terraform |
| It needs a reverse proxy | nginx or Traefik |
| It needs observability | VictoriaMetrics for metrics, Grafana’s LGTM stack for logs, dashboards, traces, and metrics |

## Working memory

- **Learning now** · TypeScript
- **On the list** · Swift and C++
