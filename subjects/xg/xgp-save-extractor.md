# XGP-save-extractor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Z1ni/XGP-save-extractor, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/xgp-save-extractor

## Pinned environment

- Project commit: `3e1bf319a9760a476968239c563e76f1c741c467`
- Test commit: `3e1bf319a9760a476968239c563e76f1c741c467`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.7 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 12.7 | 4 | 4 | [run](https://argusic.com/run/ddac7cdc-3fd0-4cd3-9151-46930d913c3c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `os.path.expandvars does not expand Windows %VAR% on Linux`
- 0.5 min: `Backslash path separators cause Path.exists() to fail on Linux`
- 2 min: `UTF-16 decode with BOM fails on XGP container data (uses UTF-16-LE without BOM)`
- 1 min: `input() raises EOFError in CI/headless environments`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
