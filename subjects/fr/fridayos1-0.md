# FridayOS1.0

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Robinson-AI-Lab/FridayOS1.0, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fridayos1-0

## Pinned environment

- Project commit: `eaf305360eb365bd28b03abf4e9c81b95bf1dcb7`
- Test commit: `eaf305360eb365bd28b03abf4e9c81b95bf1dcb7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.8 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 8.8 | 2 | 2 | [run](https://argusic.com/run/2b4d2c11-ec27-4786-af52-8bafcdefc8aa) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `FridayOS-Lite示例大脑生成器.py had hardcoded absolute BASE path '/sessions/friendly-upbeat-wozniak/...' causing PermissionError`
- 2 min: `docs/images/gif/node.gif has LZW decode error in one frame (202/210 frames decode)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
