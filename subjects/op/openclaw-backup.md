# openclaw-backup

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LeoYeAI/openclaw-backup, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/openclaw-backup

## Pinned environment

- Project commit: `a05a80d554a311c4b36c8ab6c1316ddb35330a9c`
- Test commit: `a05a80d554a311c4b36c8ab6c1316ddb35330a9c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7.1 | 1 | 1 | [run](https://argusic.com/run/f411bdd3-5948-47af-a8ce-a13451ec362a) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `rsync not installed in container - all scripts depend on it`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
