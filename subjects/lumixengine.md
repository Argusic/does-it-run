# LumixEngine

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nem0/LumixEngine, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/lumixengine

## Pinned environment

- Project commit: `c1d6f677101b892d3f28f2f15a3e5495d04f107b`
- Test commit: `c1d6f677101b892d3f28f2f15a3e5495d04f107b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.7 to 77.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1.7 | 0 | 0 | [run](https://argusic.com/run/adb24309-982b-457b-9469-21ec1f4c6fd3) |
| 2 | pass | 100 | 0 | 77.4 | 3 | 3 | [run](https://argusic.com/run/4bd4e8d0-266e-4d69-b880-182bce79e3e9) |

## What was observed on a clean machine

Attempt 2:

- `Hardcoded absolute paths in tests.make LINKCMD pointed to wrong filenames (libbz2.so.1.0.4 vs libbz2.so)`
- `Missing HashFunc<Path> specialization in engine_hash_funcs.h caused undefined references`
- `Empty libPhysX.a (8 bytes archive header) and missing libpng/brotli symbols needed by Freetype static lib`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
