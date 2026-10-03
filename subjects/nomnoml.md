# nomnoml

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/skanaar/nomnoml, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nomnoml

## Pinned environment

- Project commit: `3f30d38556e93b89231d7c11ef7ef93faf525d90`
- Test commit: `3f30d38556e93b89231d7c11ef7ef93faf525d90`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.6 to 1.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.16 | 1.6 | 1 | 1 | [run](https://argusic.com/run/f82afbd8-e8df-43d1-a233-c5f83262cfe1) |

## What was observed on a clean machine

Attempt 1:

- 0.16 min: `graphre dependency not pre-installed (npm install had never been run)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
