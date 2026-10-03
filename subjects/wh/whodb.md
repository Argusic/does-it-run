# whodb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clidey/whodb, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/whodb

## Pinned environment

- Project commit: `173c807128838fb847d2866074ea97efc471e021`
- Test commit: `173c807128838fb847d2866074ea97efc471e021`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 29.9 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/13fb157a-60be-45dd-bb27-0466e22a8f2a) |
| 1 | pass | 100 | 14 | 29.9 | 4 | 4 | [run](https://argusic.com/run/a79ea10d-1132-4863-b713-73dc25526d4a) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/8641632a-14bf-4b94-8d15-0ff3ca44a965) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.27 not installed; downloaded go1.27.1 tarball`
- 1 min: `Node.js 18 lacks required node:util styleText export; rolldown 1.2.3 needs Node >=21`
- 1 min: `pnpm not available; installed via npm --prefix`
- 1 min: `@rolldown/binding-linux-x64-gnu missing in pnpm lock; vite/rolldown native binding not installed on initial npm+pnpm under Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
