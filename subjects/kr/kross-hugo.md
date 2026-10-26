# kross-hugo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/themefisher/kross-hugo, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/kross-hugo

## Pinned environment

- Project commit: `b73d76f8ccd0ed2d0863f572759ae2275154e6a5`
- Test commit: `b73d76f8ccd0ed2d0863f572759ae2275154e6a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 10.2 | 3 | 3 | [run](https://argusic.com/run/02641299-6e71-4221-b984-3faa179df7fc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Hugo binary not found in PATH`
- 1 min: `Go binary not found in PATH (required for Hugo modules)`
- 1 min: `npm run project-setup not run yet`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
