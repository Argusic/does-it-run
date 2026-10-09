# OpenContext

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0xranx/OpenContext, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/opencontext

## Pinned environment

- Project commit: `0649e7134346f6f5038a9b29cc5c824ae6a54f3f`
- Test commit: `0649e7134346f6f5038a9b29cc5c824ae6a54f3f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 4.4 | 3 | 3 | [run](https://argusic.com/run/e4b673a3-ada8-4dd4-84ea-b273a975c7b2) |

## What was observed on a clean machine

Attempt 1:

- `npm install engine warnings: commander, vectra, react-router, undici, cheerio require node>=20 but container has node 18`
- `Rust tests skipped: cargo not found in container`
- `4 native tests skipped: optional @aicontextlab/core-native not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
