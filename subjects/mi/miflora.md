# miflora

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/basnijholt/miflora, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/miflora

## Pinned environment

- Project commit: `e092814334b062a75a09c5173cfed8e24a940607`
- Test commit: `e092814334b062a75a09c5173cfed8e24a940607`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 1.3 to 1.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 1.3 | 2 | 2 | [run](https://argusic.com/run/31b16645-4335-4998-ad50-297abdd775fa) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `externally-managed-environment blocked system-wide pip install`
- 1 min: `git-based version detection produced invalid version 'unknown+ge092814' (no git tags)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
