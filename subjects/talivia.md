# talivia

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/talivia-group/talivia, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/talivia

## Pinned environment

- Project commit: `6e2f5531548e4ba7e7da6d329704eee079d48422`
- Test commit: `6e2f5531548e4ba7e7da6d329704eee079d48422`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 25.7 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/7df3a8ef-4c39-4c3f-9567-c6b861d1e55d) |
| 2 | pass | 100 | 28 | 25.7 | 6 | 6 | [run](https://argusic.com/run/3d064114-58f6-4b50-b943-f15e1fdbd18e) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Node.js v18 installed, project requires Node.js 22+`
- 1 min: `pnpm not installed for Node 22`
- 1 min: `APP_SECRET not set in .env`
- 10 min: `Next.js production build OOM (killed at page data collection with 119 workers) - only ~1GB RAM available`
- 5 min: `Next.js dev server (Turbopack) crashes with EMFILE/too many open files due to pnpm's deeply nested node_modules symlinks`
- 8 min: `PostgreSQL not available in container (no Docker, no apt install permission)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
