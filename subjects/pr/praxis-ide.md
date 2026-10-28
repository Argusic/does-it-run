# praxis-ide

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/toblotron/praxis-ide, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/praxis-ide

## Pinned environment

- Project commit: `b4f732c28f0280ead015094bce893a378a28bec2`
- Test commit: `b4f732c28f0280ead015094bce893a378a28bec2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 8.1 to 24.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 24.7 | 0 | 0 | [run](https://argusic.com/run/48e3e95c-f0e6-4ad8-a0de-23cde4c45668) |
| 2 | pass | 100 | 4 | 8.1 | 1 | 1 | [run](https://argusic.com/run/22245244-8ade-4717-8b53-e8011d6c95bc) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Case-sensitive path mismatch: index.html referenced lib/Slickgrid/plugins/ (lowercase) but directory is lib/Slickgrid/Plugins/ (uppercase P) on Linux, causing 8 JS files to not load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
