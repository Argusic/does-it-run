# cadence

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cadence-workflow/cadence, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/cadence

## Pinned environment

- Project commit: `33704b3a5fc2e9ea61a6d62ba1076cebf081b759`
- Test commit: `33704b3a5fc2e9ea61a6d62ba1076cebf081b759`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.8 to 22.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 22.8 | 2 | 2 | [run](https://argusic.com/run/23f05625-5eeb-4533-9088-eb65366a1efc) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Go 1.25.14 not pre-installed , downloaded and installed from golang.org`
- 1 min: `unzip not installed , downloaded .deb and extracted manually`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
