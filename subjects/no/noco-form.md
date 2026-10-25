# noco-form

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nocokit/noco-form, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/noco-form

## Pinned environment

- Project commit: `28fec8c27b11b40824185e80c6f01767cd44a474`
- Test commit: `28fec8c27b11b40824185e80c6f01767cd44a474`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.7 | 3 | 3 | [run](https://argusic.com/run/263badd2-5f66-4e94-84db-b9a96fc32d2d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing @rollup/rollup-linux-x64-gnu (npm optional dependency bug)`
- 5 min: `unplugin v3 incompatible with Node 18 , unplugin-vue-components v32 requires Node >=20.19`
- 1 min: `Case-sensitive import: Outline.svg vs outline.svg in comp-icon.ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
