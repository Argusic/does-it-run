# TW5-TiddlyMap

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/felixhayashi/TW5-TiddlyMap, licensed BSD-2-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/tw5-tiddlymap

## Pinned environment

- Project commit: `03fb186d890cb97b312e2fbd98c381d8ba027d05`
- Test commit: `03fb186d890cb97b312e2fbd98c381d8ba027d05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.1 to 12.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 12.1 | 2 | 2 | [run](https://argusic.com/run/3c9f7aa9-a8e1-41b8-bdf7-168800a906bf) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing vis-network plugin dependency (felixhayashi/vis)`
- 3 min: `Babel compilation strips TW module headers from dist JS files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
