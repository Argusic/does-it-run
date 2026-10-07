# soprano

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ekwek1/soprano, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/soprano

## Pinned environment

- Project commit: `12fac06eb8fa53bad8b3941d3cb11e9c869477c4`
- Test commit: `12fac06eb8fa53bad8b3941d3cb11e9c869477c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.4 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.4 | 1 | 1 | [run](https://argusic.com/run/d21c3100-eba2-431f-8be0-ac56a26142db) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `sounddevice unconditionally imports at module level in soprano/utils/streaming.py, raising OSError('PortAudio library not found') when the system lacks PortAudio`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
