# CudaText

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Alexey-T/CudaText, licensed MPL-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/cudatext

## Pinned environment

- Project commit: `46653343eb5319e38d41c171352746edc3ccbd24`
- Test commit: `46653343eb5319e38d41c171352746edc3ccbd24`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 8.9 | 1 | 1 | [run](https://argusic.com/run/ebfcb766-1d34-434f-9daa-26282c3477c5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing shared library libharfbuzz-gobject.so.0 required by the prebuilt binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
