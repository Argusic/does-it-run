# metamcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/metatool-ai/metamcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/metamcp

## Pinned environment

- Project commit: `ff4ff2de9d25453c52dcc7be32680b30700a6012`
- Test commit: `ff4ff2de9d25453c52dcc7be32680b30700a6012`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 10.8 | 3 | 3 | [run](https://argusic.com/run/5076bf16-8634-46a4-8961-885bb176b1f4) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not available - installed via npm --prefix`
- 3 min: `PostgreSQL not installed - extracted from deb packages and started statically`
- 0.5 min: `Database tables did not exist - needed drizzle migrations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
