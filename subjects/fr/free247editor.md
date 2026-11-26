# free247editor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/riecodes/free247editor, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/free247editor

## Pinned environment

- Project commit: `55f0c92763256a01131d4d25540682f581cc05c7`
- Test commit: `55f0c92763256a01131d4d25540682f581cc05c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.3 | 8 | 8 | [run](https://argusic.com/run/1db928d0-1c03-4e33-b0fc-19321ceec8d1) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node v18 (needs v22+)`
- `npm ci in kit failed: onnxruntime-node CUDA download 404`
- 1 min: `npm run in kit used system Node v18 via PATH`
- 1 min: `sharp native binary missing (npm ci skips optional deps)`
- 2 min: `No Chrome/Chromium installed; hyperframes could not extract its own zip (no unzip)`
- `python command not found (only python3)`
- `faster-whisper Python package not initially available for import`
- `engine --selftest needed npm-cli.js in src-tauri/binaries/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
