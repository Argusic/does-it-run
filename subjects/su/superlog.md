# superlog

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/superloglabs/superlog, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/superlog

## Pinned environment

- Project commit: `b6f3223ac6721bb53f35f142e5be63baff857751`
- Test commit: `b6f3223ac6721bb53f35f142e5be63baff857751`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 45.7 to 45.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 45.7 | 4 | 4 | [run](https://argusic.com/run/bc7ab21b-f019-4c87-a94e-eaae7d69db24) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Node.js 18.19.1 was installed, project requires >=20; Docker is not available (no root), cannot run postgres/clickhouse/collector containers`
- 5 min: `DATABASE_URL is not set , real Postgres required for API server, web server, and most integration tests`
- `127 DB migrations (23MB) cause pglite-based migration test to timeout/run very slowly`
- `Docker compose unavailable , cannot start postgres, clickhouse, or collector services`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
