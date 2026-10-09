# json-machine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/halaxa/json-machine, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/json-machine

## Pinned environment

- Project commit: `03d006d2994872ab8a70b70a7c3d7f0a52493c21`
- Test commit: `03d006d2994872ab8a70b70a7c3d7f0a52493c21`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 3.9 | 1 | 1 | [run](https://argusic.com/run/35948dd1-2e0b-46af-a638-0b9edcd7ff37) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `sh: php: not found - AutoloadingTest subprocess invoked php which was not on PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
