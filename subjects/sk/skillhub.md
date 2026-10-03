# skillhub

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iflytek/skillhub, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/skillhub

## Pinned environment

- Project commit: `735259728f19a4904c7d8f634da2e467e7771e3c`
- Test commit: `735259728f19a4904c7d8f634da2e467e7771e3c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 35.7 to 88.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 35.7 | 0 | 0 | [run](https://argusic.com/run/337034ee-6748-4ac4-b11f-d369e9089d82) |
| 2 | timeout | none | 21 | 88.5 | 5 | 3 | [run](https://argusic.com/run/f232c919-5404-46be-9830-ef0a271c1ebe) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Java 21 not installed , required by project`
- 0.5 min: `pnpm not installed , required by frontend`
- `Docker not available , 6 Testcontainers tests fail`
- `Postgres/Redis/MinIO unavailable via Docker Compose , app cannot start`
- `Frontend typecheck and bulk test suite OOM on 2GB RAM`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
