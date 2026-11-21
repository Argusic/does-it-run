# FridayOS1.0

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Robinson-AI-Lab/FridayOS1.0, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fridayos1-0

## Pinned environment

- Project commit: `eaf305360eb365bd28b03abf4e9c81b95bf1dcb7`
- Test commit: `eaf305360eb365bd28b03abf4e9c81b95bf1dcb7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 5.2 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 8.8 | 2 | 2 | [run](https://argusic.com/run/2b4d2c11-ec27-4786-af52-8bafcdefc8aa) |
| 2 | pass with mocks | 92 | 12 | 5.2 | 7 | 7 | [run](https://argusic.com/run/72934191-8d02-493d-8784-3126cfb126c6) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `FridayOS-Lite示例大脑生成器.py had hardcoded absolute BASE path '/sessions/friendly-upbeat-wozniak/...' causing PermissionError`
- 2 min: `docs/images/gif/node.gif has LZW decode error in one frame (202/210 frames decode)`

Attempt 2:

- 2 min: `npm global install EACCES: /usr/local/lib/node_modules not writable`
- 1 min: `Python brain generator hardcoded BASE path to /sessions/... (PermissionError)`
- `node.gif LZW decode failed (corrupted media asset)`
- `cc-switch and Obsidian are GUI-only apps; no headless install possible`
- `No test framework, CI pipeline, or package.json found in repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
