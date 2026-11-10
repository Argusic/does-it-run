# speech.cpp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nyosegawa/speech.cpp, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/speech-cpp

## Pinned environment

- Project commit: `03555100287c118b41d1b475044e5ab1e07baa8c`
- Test commit: `03555100287c118b41d1b475044e5ab1e07baa8c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 6.5 | 1 | 1 | [run](https://argusic.com/run/9e74e410-3545-4808-b3b6-b43b49dd8011) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Parallel build with -j ran out of memory (OOM killed cc1plus processes) on some compilation units`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
