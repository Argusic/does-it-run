# Koito

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gabehf/Koito, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/koito

## Pinned environment

- Project commit: `a079fa693569d21e03c00df163f20ac5e137c490`
- Test commit: `a079fa693569d21e03c00df163f20ac5e137c490`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 36.9 to 55.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 36.9 | 4 | 4 | [run](https://argusic.com/run/180a99a5-f0bd-483a-9448-ae125a0c27f1) |
| 2 | pass | 100 | 57 | 55.7 | 4 | 4 | [run](https://argusic.com/run/2bac8618-27fa-47c8-84a0-9a802a640751) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain not installed`
- 15 min: `libvips-dev not available (CGO dependency for bimg image processing)`
- 5 min: `Yarn 4 not available for client build`
- 2 min: `Node.js 18 too old for react-router build`

Attempt 2:

- 2 min: `Go 1.25 not pre-installed`
- 28 min: `libvips-dev and CGo dependencies (glib, pcre2, etc.) not pre-installed`
- 15 min: `bimg/vips.h naming conflict with system <vips/vips.h>`
- 10 min: `Linker resolution of transitive shared libs (HDF5, Imath, libsz, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
