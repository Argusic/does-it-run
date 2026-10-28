# dot-hugo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gethugothemes/dot-hugo, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dot-hugo

## Pinned environment

- Project commit: `874804ff411974c4b95bfdb731646d5aa3f0ed31`
- Test commit: `874804ff411974c4b95bfdb731646d5aa3f0ed31`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3 | 4 | 4 | [run](https://argusic.com/run/cd890633-4ed0-4881-9cc9-076d3d3c5871) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `pnpm not found`
- 0.3 min: `Hugo not found`
- 0.3 min: `Go not in PATH`
- 0.5 min: `Node v18 incompatible with Hugo 0.163 POSTCSS flags`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
