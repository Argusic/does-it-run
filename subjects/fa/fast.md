# fast

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jonatas/fast, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/fast

## Pinned environment

- Project commit: `d2068730ef68fe6090268da9a61fd7442057fc57`
- Test commit: `d2068730ef68fe6090268da9a61fd7442057fc57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.8 to 33.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 33.8 | 1 | 1 | [run](https://argusic.com/run/c8c1e781-44e0-409e-b6d9-30527d139178) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `Ruby runtime not present in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
