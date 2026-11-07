# YouDub-webui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liuzhao1225/YouDub-webui, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/youdub-webui

## Pinned environment

- Project commit: `0f6c75935e7a208c4b8ea56140e31c5316953fec`
- Test commit: `0f6c75935e7a208c4b8ea56140e31c5316953fec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 19.3 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 20.2 | 3 | 3 | [run](https://argusic.com/run/d0073f21-4784-4c52-9347-6162e06e7049) |
| 2 | pass | 100 | 45 | 19.3 | 5 | 5 | [run](https://argusic.com/run/20c66b3b-24e6-4df1-9cf2-129353077040) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `diffq failed to build from source (missing Python.h, no root for python3-dev)`
- 1 min: `Node.js v18.19.1 too old for Next.js 16 (requires >=20.9.0) and vitest 4 (requires >=22)`
- 1 min: `socksio missing for SOCKS proxy test`

Attempt 2:

- 8 min: `pip install -r requirements.txt failed: diffq sdist build needs Python.h (python3-dev) and we have no root`
- 6 min: `torchaudio resolved to CUDA build from PyPI which fails to load (libcudart.so.13 missing) against CPU torch`
- 2 min: `uvicorn missing from backend/requirements-test.txt so backend launch failed (No such file or directory)`
- 5 min: `System node v18 too old for Next.js 16 (requires Node 20+)`
- 3 min: `End-to-end task failed at translate stage because my initial mock returned a plain string instead of the required JSON object`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
