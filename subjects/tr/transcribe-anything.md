# transcribe-anything

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zackees/transcribe-anything, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/transcribe-anything

## Pinned environment

- Project commit: `c4a1808e6acfd8024729f8bf86d37db0907e633d`
- Test commit: `c4a1808e6acfd8024729f8bf86d37db0907e633d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.8 to 20.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 20.8 | 2 | 2 | [run](https://argusic.com/run/838b749b-cb4a-49c1-a705-f34f8259a909) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv (the project's package manager) not found on PATH`
- 1 min: `whisper iso-env requires Python 3.10 (requires-python = "==3.10.*") but only 3.11+ was available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
