# ViralForge

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fendouai/ViralForge, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/viralforge

## Pinned environment

- Project commit: `cf08c8c87b049d0e28977ea90ee2827366cf1516`
- Test commit: `cf08c8c87b049d0e28977ea90ee2827366cf1516`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 4.1 | 4 | 4 | [run](https://argusic.com/run/bb1d153d-baae-4243-b11a-8c6f298eb84b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 installed but engine requires >=22.15`
- `Playwright system deps failed to install (no root, su auth failure)`
- 3 min: `MCP server analyze_video tool failed: python3 couldn't import cv2 (opencv-python-headless not installed in system python due to PEP 668)`
- 1 min: `MCP test expected shotCount: 5 but analyze.py returns 4 for glow.mp4`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
