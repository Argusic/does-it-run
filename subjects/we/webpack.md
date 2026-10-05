# webpack

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/webpack/webpack, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/webpack

## Pinned environment

- Project commit: `089b4c064fc63ea7830c4b1b06ef3dd0cadf864e`
- Test commit: `089b4c064fc63ea7830c4b1b06ef3dd0cadf864e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 57.9 to 87.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.9 | 0 | 0 | [run](https://argusic.com/run/cdfd1d35-ace5-4d6d-b99c-2976a5e5d184) |
| 2 | pass | 93.33 | 4 | 57.9 | 3 | 2 | [run](https://argusic.com/run/06bc1d6b-b4ec-4930-aff5-d134c381be74) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `yarn not found in PATH for automated setup`
- 0.5 min: `yarn not in PATH after npm install yarn to project`
- `webpack --help fails with 'Invalid value used as weak map key'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
