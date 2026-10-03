# nightingale

**Verdict: runs.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ccfos/nightingale, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/nightingale

## Pinned environment

- Project commit: `6392c79de4bf7495b6ac9d41ef5a6f872dbc0743`
- Test commit: `6392c79de4bf7495b6ac9d41ef5a6f872dbc0743`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13.4 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/3496e5ac-06e8-41f2-9e10-8d07cd400bab) |
| 2 | pass | 88 | 7.5 | 13.4 | 5 | 2 | [run](https://argusic.com/run/2d168c7f-3e89-4a1e-bc6b-79d3245ba792) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Go compiler not installed in container`
- 0.2 min: `statik binary not found, fe.sh failed`
- `pkg/unit: timestamp tests fail in UTC timezone (expect Asia/Shanghai dates)`
- `pkg/ormx, models/migrate, dskit/mysql, dskit/clickhouse, dskit/victorialogs: tests require external MySQL/Postgres/ClickHouse/VictoriaLogs services`
- `pkg/promql: TestGetLabelsAndMetricNameWithReplace ordering issue in promql parser (pre-existing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
