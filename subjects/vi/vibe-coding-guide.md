# Vibe_coding_guide

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Lling0000/Vibe_coding_guide, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/vibe-coding-guide

## Pinned environment

- Project commit: `5fea8fc17f2058132c27eb9bf0eacb0abbb3ba5e`
- Test commit: `5fea8fc17f2058132c27eb9bf0eacb0abbb3ba5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 5.6 | 4 | 4 | [run](https://argusic.com/run/98ecf63d-38a1-42e7-b751-b09dd648df99) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `pip install blocked by PEP 668 externally-managed environment`
- 8 min: `puppeteer browser download failed: no zip archiver available (system lacks unzip)`
- 3 min: `Chrome launch crash: chrome_crashpad_handler Permission denied`
- 2 min: `background http.server died between exec invocations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
