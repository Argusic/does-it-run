# code-mode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/universal-tool-calling-protocol/code-mode, licensed MPL-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/code-mode

## Pinned environment

- Project commit: `e5fdc319bfae1ceec57e7bce37048337635ffb51`
- Test commit: `e5fdc319bfae1ceec57e7bce37048337635ffb51`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.5 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 17.5 | 3 | 3 | [run](https://argusic.com/run/af4a1796-5c72-48c9-a152-b149e56a9e6b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Python CodeModeUtcpClient missing abstract close() method`
- 10 min: `isolated-vm@6.x requires Node.js >=22, container has Node 18`
- 8 min: `Built isolated-vm@5.0.4 from source; linker missing unversioned .so symlinks (z, uv, brotli, cares, nghttp2, crypto, ssl, icu)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
