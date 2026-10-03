# hugo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gohugoio/hugo, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/hugo

## Pinned environment

- Project commit: `079c76f0104de25c3e8f5b7d77878291bd8c8c2c`
- Test commit: `079c76f0104de25c3e8f5b7d77878291bd8c8c2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 53.3 to 53.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 53.3 | 2 | 2 | [run](https://argusic.com/run/116f14fc-92fc-41d4-b6bc-6d1036fd94b7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.27.0 not installed on the system`
- 1 min: `codegen/methods.go panic: the ProjectRootDir guard (!strings.Contains(c.ProjectRootDir, "hugo")) failed because the repo is cloned to /work/repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
