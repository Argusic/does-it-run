# agenticos

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vstorm-co/agenticos, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agenticos

## Pinned environment

- Project commit: `376adfdaf07e3bb64574735ed6fcc9e5dab43911`
- Test commit: `376adfdaf07e3bb64574735ed6fcc9e5dab43911`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 15 | 2 | 2 | [run](https://argusic.com/run/eaf62f69-0ced-4995-b1d5-0301dda8b30d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Frontend vitest requires Node 20+ for the styleText API; bun 1.4.4 works as runtime but one test (diagnostics.test.ts) fails due to zod import incompatibility`
- `Backend app and integration tests need PostgreSQL with pgvector and Redis , not available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
