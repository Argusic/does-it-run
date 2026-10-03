# pikiwidb

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenAtomFoundation/pikiwidb, licensed BSD-3-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/pikiwidb

## Pinned environment

- Project commit: `54693ce5882f89590e3e1357605deaa1e4521102`
- Test commit: `54693ce5882f89590e3e1357605deaa1e4521102`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 31.7 to 51.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9.5 | 31.7 | 3 | 3 | [run](https://argusic.com/run/836b0ac5-d729-4f38-83cd-bab9d1a5fe4e) |
| 2 | pass | 100 | 27 | 45.6 | 2 | 2 | [run](https://argusic.com/run/56f4b3e9-f220-4902-83ac-7b590aaab1a8) |
| 3 | fail | 20 | n/a | 51.5 | 0 | 0 | [run](https://argusic.com/run/0bca64ad-f955-4f9e-995d-058588eddaa8) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `autoconf not installed in container`
- 4 min: `OOM from -j192 (container reports 192 cores, only 8GB RAM)`
- 0.5 min: `pika.conf missing databases parameter, default 0 causes FATAL`

Attempt 2:

- 3 min: `autoconf not found on system, no root to install packages`
- 24 min: `cmake detected 192 CPU cores from /proc/cpuinfo causing OOM kills`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
