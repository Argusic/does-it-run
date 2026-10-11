# OpenLore

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aakarim/OpenLore, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/openlore

## Pinned environment

- Project commit: `77e3534b7e5eaf21154c028803a94758cd960545`
- Test commit: `77e3534b7e5eaf21154c028803a94758cd960545`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.3 | 2 | 2 | [run](https://argusic.com/run/36e392ac-8970-4f66-944f-86bfd248d32f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`
- 1 min: `Server failed to start: missing ./config/lore.json auth config`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
