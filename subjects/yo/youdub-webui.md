# YouDub-webui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liuzhao1225/YouDub-webui, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/youdub-webui

## Pinned environment

- Project commit: `0f6c75935e7a208c4b8ea56140e31c5316953fec`
- Test commit: `0f6c75935e7a208c4b8ea56140e31c5316953fec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.2 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 20.2 | 3 | 3 | [run](https://argusic.com/run/d0073f21-4784-4c52-9347-6162e06e7049) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `diffq failed to build from source (missing Python.h, no root for python3-dev)`
- 1 min: `Node.js v18.19.1 too old for Next.js 16 (requires >=20.9.0) and vitest 4 (requires >=22)`
- 1 min: `socksio missing for SOCKS proxy test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
