# pagible

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aimeos/pagible, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/pagible

## Pinned environment

- Project commit: `992c715ad334c38499b0069056d619ca24dce941`
- Test commit: `992c715ad334c38499b0069056d619ca24dce941`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 43.3 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 43.3 | 3 | 3 | [run](https://argusic.com/run/615882e0-1dab-4a1c-b35a-8bb0bacf3d43) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP and Composer not available in container`
- 1 min: `Path repo version mismatch: sub-packages had git-hash versions but root required dev-master`
- 1 min: `Security advisories blocked enshrined/svg-sanitize package installation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
