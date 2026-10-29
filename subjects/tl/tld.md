# tld

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mertcikla/tld, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tld

## Pinned environment

- Project commit: `a67274fc43f99e6acf69a0c624e8801233b8352c`
- Test commit: `a67274fc43f99e6acf69a0c624e8801233b8352c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9 to 9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 9 | 4 | 4 | [run](https://argusic.com/run/7ac40cf7-9eed-4f72-9f75-d1286e720eef) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `go binary not found in container; repo requires Go 1.26.2`
- 6 min: `frontend build required Node >=20.19 but container had Node 18; vite 8 crashed on CustomEvent`
- 4 min: `npm install skipped @rolldown/binding-linux-x64-gnu optional native binding, vite build failed`
- 6 min: `go embed required frontend/dist which did not exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
