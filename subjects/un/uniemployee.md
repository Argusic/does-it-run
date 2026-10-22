# UniEmployee

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zj-unicom-ai/UniEmployee, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/uniemployee

## Pinned environment

- Project commit: `7d5edf5480d077ba30d9ab3605aa95d8ba327f21`
- Test commit: `7d5edf5480d077ba30d9ab3605aa95d8ba327f21`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 38 to 38 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 38 | 6 | 6 | [run](https://argusic.com/run/b1448939-d36c-4882-8fc3-a30f80519ef7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `deepagents version mismatch: requirements.txt specifies 0.7.13 but lock file pins 0.7.5 causing API incompatibility`
- 8 min: `admin account seeded with must_change_password=true blocking all admin API calls used by tests`
- 3 min: `Argusic proxy on port 8787 returns 502 for all requests; tests hardcode BASE=http://localhost:8787`
- 5 min: `Port 8787 occupied by argusic proxy that auto-restarts on kill; cannot bind uvicorn there`
- 3 min: `Playwright browser tests require frontend/dist/ which is not built and Node.js 18 cannot build it (needs 20+)`
- 2 min: `Additional dependencies (duckdb, sqlglot, openpyxl, jieba, rank-bm25, SQLAlchemy, opensandbox, langchain-sandbox-opensandbox) not in lock file but required by requirements.txt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
