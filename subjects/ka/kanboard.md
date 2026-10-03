# kanboard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kanboard/kanboard, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/kanboard

## Pinned environment

- Project commit: `cf53b54597b67b60140586c09c2fe6132ead013c`
- Test commit: `cf53b54597b67b60140586c09c2fe6132ead013c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 12.4 | 3 | 3 | [run](https://argusic.com/run/7c70adca-ff52-434b-bfed-b6d1c6415a71) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP binary in container`
- 1 min: `No composer`
- 1 min: `No config.php`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
