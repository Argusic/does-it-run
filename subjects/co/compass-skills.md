# compass-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dongshuyan/compass-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/compass-skills

## Pinned environment

- Project commit: `1b2e556ce6f293ba12e95e18d51995d6a969d52f`
- Test commit: `1b2e556ce6f293ba12e95e18d51995d6a969d52f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 6 | 1 | 1 | [run](https://argusic.com/run/e595f674-bbcc-457d-86a4-427657c84807) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npx skills add dongshuyan/compass-skills --list failed: npm package skills@1.7.2 requires Node.js >=22.20.0, but container has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
