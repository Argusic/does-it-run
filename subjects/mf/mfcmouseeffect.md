# MFCMouseEffect

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sqmw/MFCMouseEffect, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/mfcmouseeffect

## Pinned environment

- Project commit: `4a6bdf289c788b42767993c605e95fd66df93474`
- Test commit: `4a6bdf289c788b42767993c605e95fd66df93474`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 46.3 to 46.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 46.3 | 1 | 1 | [run](https://argusic.com/run/6098416c-acb9-44eb-86b4-20ec5478f0ac) |

## What was observed on a clean machine

Attempt 1:

- 55 min: `POSIX regression suite scaffold HTTP smoke check hung on 'printf 'exit ' | binary -mode=background' because the embedded HTTP server's accept() was not interrupted by close() on Linux.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
