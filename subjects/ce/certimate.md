# certimate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/certimate-go/certimate, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/certimate

## Pinned environment

- Project commit: `6968e672329ea1df617879fe73bee1d7de2f93b7`
- Test commit: `6968e672329ea1df617879fe73bee1d7de2f93b7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 16.8 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/3614c39e-001c-4d47-8d4d-141152d0bdc2) |
| 2 | pass | 100 | 17 | 16.8 | 5 | 5 | [run](https://argusic.com/run/5bcd57a8-414c-42d3-8fd0-2561251315f4) |

## What was observed on a clean machine

Attempt 2:

- 9 min: `Go 1.27.1 compiler crashed with SIGSEGV on alibabacloud-go/esa package`
- 2 min: `Git submodule pkg/sdk3rd-forked empty (SSH URL, no SSH key)`
- 3 min: `Node.js 18 too old for vite 8.x (missing styleText export)`
- `npm 10 rejected by devEngines (requires >=11.10.0)`
- 1 min: `rolldown native binding not found after Node upgrade`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
