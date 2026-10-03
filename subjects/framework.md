# framework

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/observablehq/framework, licensed ISC, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/framework

## Pinned environment

- Project commit: `85e843e6acfa3dbe93129c125156352c9c50b697`
- Test commit: `85e843e6acfa3dbe93129c125156352c9c50b697`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.6 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.5 | 15.6 | 2 | 0 | [run](https://argusic.com/run/211faec5-10cc-45dd-a036-05b73f69496d) |

## What was observed on a clean machine

Attempt 1:

- `Test failure: archives.posix - zip binary not found in container`
- `Test failure: within() asserts CWD named framework, but dir is repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
