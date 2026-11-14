# selectolax

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rushter/selectolax, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/selectolax

## Pinned environment

- Project commit: `fd9fe8f13c8b18a0319abdbed9977113045dd9bf`
- Test commit: `fd9fe8f13c8b18a0319abdbed9977113045dd9bf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.5 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.5 | 3 | 3 | [run](https://argusic.com/run/d3859149-26d2-4191-8b68-a1e9e55d62aa) |
| 2 | pass | 100 | 6 | 6.7 | 4 | 4 | [run](https://argusic.com/run/3d1afe3f-4584-4ee7-bfa4-913dffd4a946) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally managed Python environment: pip install rejected`
- 2 min: `Missing Python C header files (Python.h, pyconfig.h): python3.12-dev not installed`
- 1 min: `pip editable install rebuild fails because CFLAGS not forwarded to build subprocess`

Attempt 2:

- 1 min: `Git submodule for lexbor engine not initialized`
- 2 min: `Missing Python.h (python3.12-dev headers not installed)`
- 1 min: `Missing patchlevel.h and other dev headers`
- 1 min: `Missing x86_64-linux-gnu/python3.12/pyconfig.h`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
