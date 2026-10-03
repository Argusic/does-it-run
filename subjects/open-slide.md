# open-slide

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-slide/open-slide, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-slide

## Pinned environment

- Project commit: `65914fea5f70a746f2be4d695aea3c2a44c88b33`
- Test commit: `65914fea5f70a746f2be4d695aea3c2a44c88b33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 5 | 0 | 0 | [run](https://argusic.com/run/60ca8515-8885-4b8f-9cb3-4ae89652580b) |
| 2 | pass | 100 | 4.5 | 5 | 4 | 4 | [run](https://argusic.com/run/ee3cf67c-7cc3-45ba-a6b4-fa259777d743) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Node.js v18.19.1 too old , rolldown needs styleText from node:util, Next.js needs >=20.9.0`
- 0.3 min: `pnpm not available with the system Node.js 18`
- 0.2 min: `tsdown bundler failed: 'Failed to import module unrun'`
- 3 min: `web:build (Next.js marketing site) killed by OOM (exit 137)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
