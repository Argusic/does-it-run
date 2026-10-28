# realworlddevopscourse

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/predmijat/realworlddevopscourse, licensed BSD-2-Clause, written in Shell.

Evidence and recordings: https://argusic.com/subject/realworlddevopscourse

## Pinned environment

- Project commit: `2ecbd846945c11d448ec9be239e097fdd313f02c`
- Test commit: `2ecbd846945c11d448ec9be239e097fdd313f02c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 11 | 4 | 4 | [run](https://argusic.com/run/9fe32ca6-e787-45d7-927d-9a33466b72cb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PyYAML 6.0 requires Cython for pip install on Python 3.12 (pre-built wheel handles it fine when available)`
- 5 min: `No MySQL server available in container (port 3306 bindable though)`
- 4 min: `Zulip notification requires real Zulip credentials and network access to zulipchat.com`
- 2 min: `Go was not pre-installed, needed for 'present' slides tool from README`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
