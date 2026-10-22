# backup-x

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jeessy2/backup-x, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/backup-x

## Pinned environment

- Project commit: `5cf544f99ad45ca23e9b2db2322833ee0351d6b1`
- Test commit: `5cf544f99ad45ca23e9b2db2322833ee0351d6b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 2.9 | 1 | 1 | [run](https://argusic.com/run/7b49d11d-4aee-4a78-88bd-42e4cc22f570) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
