# otari

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mozilla-ai/otari, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/otari

## Pinned environment

- Project commit: `1fbdc65e2d9e0d54d265522319165110fe0d52a1`
- Test commit: `1fbdc65e2d9e0d54d265522319165110fe0d52a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.3 to 20.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 20.3 | 2 | 2 | [run](https://argusic.com/run/32ad4d21-d634-4f4f-8017-885f057491bb) |

## What was observed on a clean machine

Attempt 1:

- 0.03 min: `Python 3.13 not available on system (only 3.12)`
- 0.1 min: `uv not installed on the system`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
