# MOSS-TTSD

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenMOSS/MOSS-TTSD, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/moss-ttsd

## Pinned environment

- Project commit: `46973e425da227bfa3b315dcd7a4aba8b6be5574`
- Test commit: `46973e425da227bfa3b315dcd7a4aba8b6be5574`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.3 to 25.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 25.3 | 2 | 2 | [run](https://argusic.com/run/d03528ea-cef1-4517-8010-0664bac3cb57) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install blocked by PEP 668 (externally-managed-environment) on Debian-based container`
- 1 min: `processor(text=...) kwarg raised KeyError: conversations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
