# esphome-panasonic-ac

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DomiStyle/esphome-panasonic-ac, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/esphome-panasonic-ac

## Pinned environment

- Project commit: `c56eb4f85ad93cfbe0e89aee72b646740ee103ae`
- Test commit: `c56eb4f85ad93cfbe0e89aee72b646740ee103ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.1 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 2 | 4.1 | 0 | 0 | [run](https://argusic.com/run/a2d5d350-e18e-4fd8-9508-b4e34016ae15) |
| 2 | pass | 100 | 12 | 4.7 | 1 | 1 | [run](https://argusic.com/run/7709633f-babc-486a-be66-35ba4cdf9108) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `esphome config ac.yaml: Invalid YAML syntax 'mapping values are not allowed here' after hand-editing external_components block (self-inflicted config edit, not a repo defect)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
