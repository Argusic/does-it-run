# coroot

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coroot/coroot, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/coroot

## Pinned environment

- Project commit: `d40dd882e6ddf978f62897f2926d6881ca33370b`
- Test commit: `d40dd882e6ddf978f62897f2926d6881ca33370b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 11.6 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 11.6 | 5 | 5 | [run](https://argusic.com/run/4b24e8dd-661f-432e-bcd6-64e6895212b1) |
| 2 | fail | 80 | 14 | 13.9 | 3 | 3 | [run](https://argusic.com/run/4b6e0905-67b9-48ab-8ddf-463006a15502) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.25.5 required by go.mod but Go not installed in container`
- 2 min: `Frontend static directory missing - main.go embeds 'static' but front/dist did not exist`
- 1 min: `serialize-javascript v7 uses crypto.getRandomValues() which is undefined in webpack's build context on Node 18`
- 1 min: `liblz4-dev not installed - CGo dependency of DataDog/golz4 needs lz4.h and lz4hc.h headers`
- 1 min: `liblz4.so symlink missing - only liblz4.so.1 present, linker requires liblz4.so`

Attempt 2:

- 1 min: `Go not found in container`
- 2 min: `Frontend build: 'crypto is not defined' from serialize-javascript v7 used by css-minimizer-webpack-plugin (webpack 5 no polyfill)`
- 1 min: `Go build: liblz4-dev headers not found (needed by github.com/DataDog/golz4 CGo binding)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
