# huddol

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ImFeH2/huddol, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/huddol

## Pinned environment

- Project commit: `0470d41a38f9f15144d1bd86961c2d5b4ace10f6`
- Test commit: `0470d41a38f9f15144d1bd86961c2d5b4ace10f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30 to 30 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 30 | 7 | 7 | [run](https://argusic.com/run/204f5675-86da-4389-aad8-a920b162b424) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain installed`
- 1 min: `uv (Python package manager) not found`
- 2 min: `pnpm not available`
- 2 min: `Python 3.13 required but only 3.12 available`
- 1 min: `bubblewrap (bwrap) sandbox binary not available and cannot be apt-installed (no root)`
- 3 min: `Node.js v18 too old for webui build (needs 20+)`
- 1 min: `@tailwindcss/oxide native binary missing for linux-x64-gnu`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
