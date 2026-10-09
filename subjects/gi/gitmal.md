# gitmal

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/antonmedv/gitmal, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gitmal

## Pinned environment

- Project commit: `83be9ddcf82e8a90ea50a9d54c1ebfc3e22ace16`
- Test commit: `83be9ddcf82e8a90ea50a9d54c1ebfc3e22ace16`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.4 | 2 | 2 | [run](https://argusic.com/run/45662648-6811-4be5-b4ce-ef40429cba91) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.24.0 not installed in container`
- 1 min: `Repo checked out in detached HEAD with no local branches - gitmal requires local refs/heads/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
