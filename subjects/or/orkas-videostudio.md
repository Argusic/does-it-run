# Orkas-VideoStudio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Orkas-AI/Orkas-VideoStudio, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/orkas-videostudio

## Pinned environment

- Project commit: `c0c3c3eac359f9a3e8e3fbe65fd5426fad03dc4b`
- Test commit: `c0c3c3eac359f9a3e8e3fbe65fd5426fad03dc4b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.8 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.8 | 5 | 5 | [run](https://argusic.com/run/e696a34f-734c-49f0-a889-1f606c79b4b0) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node v18.19.1 below required >=22`
- 1 min: `pnpm not found`
- 2 min: `Build scripts blocked for esbuild/onnxruntime-node/sharp`
- 2 min: `chrome-headless-shell zip extraction failed (no unzip/yauzl)`
- 1 min: `E2E test failed on unclassified [SystemMemory] stderr lines`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
