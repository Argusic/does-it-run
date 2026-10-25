# gately

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wangwanjie/gately, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gately

## Pinned environment

- Project commit: `51f1471988b6cdee234f9c92f98c912f6cce2298`
- Test commit: `51f1471988b6cdee234f9c92f98c912f6cce2298`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.7 | 5 | 5 | [run](https://argusic.com/run/ebef7062-0ad4-4b9a-8a89-15a3bfbae41f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`
- 1 min: `pnpm not found (needed for web frontend build)`
- 1 min: `Node.js v18 (bundled) too old for Vite 8 / rolldown , missing node:util.styleText`
- 1 min: `Rolldown native binding @rolldown/binding-linux-x64-gnu not installed by pnpm on this platform`
- `Docker socket unavailable: /var/run/docker.sock not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
