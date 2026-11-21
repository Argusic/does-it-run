# commonly

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Team-Commonly/commonly, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/commonly

## Pinned environment

- Project commit: `670f723930e58334388c34e3c2dc1095c014968e`
- Test commit: `670f723930e58334388c34e3c2dc1095c014968e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 52.6 to 79 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 79 | 4 | 4 | [run](https://argusic.com/run/ad0c8970-589b-4657-999a-dbb1c7bff9f1) |
| 2 | pass | 80 | 47 | 52.6 | 3 | 0 | [run](https://argusic.com/run/e81ed00a-921e-4fb3-b9ff-fac2d4a0aa97) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `Backend test grants.mint.test.js hardcoded expiresAt 2026-10-01, now in the past, so mint returned 400 invalid_expiry`
- 22 min: `MCP grant route tests failed with 400 Parse error: ReferenceError: crypto is not defined (MCP SDK calls bare crypto.randomUUID; jest-environment-node on Node 18 lacks the crypto global)`
- 25 min: `Full backend jest runs intermittently lost worker processes (SIGTERM/SIGKILL, V8 heap-out-of-memory near 2GB cap under the 8GB cgroup with per-suite in-memory mongod); 2-5 suites per run died at suite level with no assertion failures`
- 3 min: `README install.sh requires Docker/Compose v2 which this container lacks (no root); documented quick-start path could not run`

Attempt 2:

- `Docker not available in container , install.sh requires Docker Compose v2, cannot start full stack via Docker`
- `Full backend test suite runs OOM on Node 18 with default heap limit (~4GB used across 50+ sequential mongo-memory-server instances). All 60+ test files pass individually when run in smaller batches.`
- `Some service tests (threading.*) have pre-existing skips due to PG dependency , not a failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
