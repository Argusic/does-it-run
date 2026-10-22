# infinite-image-browsing

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zanllp/infinite-image-browsing, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/infinite-image-browsing

## Pinned environment

- Project commit: `67ce3a77c4be9a927101df0571666b539910e69a`
- Test commit: `67ce3a77c4be9a927101df0571666b539910e69a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 9.8 | 4 | 4 | [run](https://argusic.com/run/0bd62c1a-0eb0-4053-a1b8-c2f406e12167) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Python is PEP 668 externally-managed; pip install failed without sudo`
- 8 min: `av==14.4.0 has no cp312 binary wheel and its sdist build needs ffmpeg dev headers (not installed, no root)`
- 5 min: `hnswlib has no cp312 binary wheel and its sdist build needs Python.h/C++ toolchain (not installed, no root)`
- 7 min: `install.py crashed: ModuleNotFoundError: No module named 'launch'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
