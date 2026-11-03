# valaxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/YunYouJun/valaxy, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/valaxy

## Pinned environment

- Project commit: `3e13c49d364cd9f883437566e7cb1069c1f2e6ea`
- Test commit: `3e13c49d364cd9f883437566e7cb1069c1f2e6ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 30.3 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 30.3 | 4 | 4 | [run](https://argusic.com/run/291d07e8-7751-4331-b7eb-ff10bdb5a8d6) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 required >=22.12.0`
- 1 min: `pnpm not found on PATH`
- 1 min: `OOM during devtools unbuild with default heap`
- 10 min: `release.test.ts fails because npm_execpath env var is set by vitest to npm-cli.js instead of pnpm, causing release script to run wrong command`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
