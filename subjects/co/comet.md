# comet

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gotzmann/comet, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/comet

## Pinned environment

- Project commit: `710a821abb197e7340fd012da91f720092f7bc77`
- Test commit: `710a821abb197e7340fd012da91f720092f7bc77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 3.2 | 2 | 2 | [run](https://argusic.com/run/49c11d8d-055c-4b54-939d-ced1219038ea) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP not installed in container`
- 1 min: `Composer not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
