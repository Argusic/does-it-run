# petdex

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crafter-station/petdex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/petdex

## Pinned environment

- Project commit: `a1b229116968cbe9f3a9b2141634a9baa0819864`
- Test commit: `a1b229116968cbe9f3a9b2141634a9baa0819864`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 10.6 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.8 | 24 | 3 | 3 | [run](https://argusic.com/run/1ff4a376-63b1-421a-9616-6c8c596665b2) |
| 2 | pass | 100 | 1.5 | 10.6 | 3 | 3 | [run](https://argusic.com/run/fa7fcadb-a3e8-489b-9aaa-20a419daca20) |

## What was observed on a clean machine

Attempt 1:

- 1.2 min: `bun not in PATH; not installed`
- 1 min: `Node.js 18.19.1 is too old for Next.js 16 (needs >=20.9.0)`
- 0.5 min: `next build OOM killed during 'Collecting page data using 90 workers' on 8GB cgroup`

Attempt 2:

- 10 min: `Next.js build fails: Node 18.19.1 < 20.9.0 required by Next 16; using bun's node shim triggers Turbopack panic in CSS pipeline`
- 5 min: `Next.js build OOM-killed during page data collection (90 workers) in constrained container`
- 3 min: `CLI asset-hosts allowlist out of sync with server when R2_PUBLIC_BASE env is set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
