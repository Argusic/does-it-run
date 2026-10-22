# kiji-proxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dataiku/kiji-proxy, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kiji-proxy

## Pinned environment

- Project commit: `c916161b32a5df519a4d87d0333f878a67d9fae7`
- Test commit: `c916161b32a5df519a4d87d0333f878a67d9fae7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.3 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 27.3 | 9 | 9 | [run](https://argusic.com/run/f1dc16a5-6bcb-4001-9e08-cb302d547777) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node 18.19.1 cannot run Babel 8/@tailwindcss native bindings (ESM 'with' syntax, missing oxide-linux-x64-gnu)`
- 3 min: `@tailwindcss/oxide-linux-x64-gnu optional dependency missing after npm install`
- 4 min: `Electron install.js fails: requires() of ES Module @electron/get@5`
- 1 min: `Electron aborts: SUID sandbox helper not configured (no root)`
- 1 min: `onnxruntime not installed in project .venv (torch-based pyproject omits it)`
- 2 min: `Model files were Git LFS pointers (737MB model.onnx absent)`
- 1 min: `Default ModelVariant 'trained' points to nonexistent model/trained; only model/quantized exists`
- 3 min: `No Go toolchain on PATH`
- 1 min: `uv not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
