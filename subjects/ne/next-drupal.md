# next-drupal

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chapter-three/next-drupal, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/next-drupal

## Pinned environment

- Project commit: `80a89f1466bcdc980b4de529241b42de296b2a7d`
- Test commit: `80a89f1466bcdc980b4de529241b42de296b2a7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 14 | 2 | 2 | [run](https://argusic.com/run/03573e01-33b3-4eb1-9c01-8d68077fb3ac) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `yarn not found in container`
- 5 min: `No Drupal backend available for integration tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
