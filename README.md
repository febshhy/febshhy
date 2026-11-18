# febshhy

**Non-deterministic rule-based expert system software engineer**  
(a.k.a. AI `.md` engineer)

I like distributed systems, high-volume data, and figuring out where the milliseconds went. I’m happy anywhere between the event stream and the dashboard.

```text
AI limit utilization  [██████████] 100%  <- the only SLO I've never missed
```

## What I’m building

[**Heimdall**](https://github.com/febshhy/heimdall-codex) gives Codex a workflow for tracing which code paths a change affects, keeping the diff focused, and showing what it actually verified.

## Rule base

| IF | THEN |
| --- | --- |
| It needs a service | Go |
| It needs a script | Python or Bash |
| It fits in one file | SQLite for the app, DuckDB for the analysis |
| It needs a server | Postgres for transactions, ClickHouse for analytics |
| It needs a pipeline | Airflow + dbt for batch, Redpanda for streams |
| It needs to run somewhere | systemd or Kubernetes |
| It’s slow | pprof or Chrome DevTools |

**Learning now** · TypeScript
