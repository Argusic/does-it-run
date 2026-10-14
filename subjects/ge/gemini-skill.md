# gemini-skill

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WJZ-P/gemini-skill, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/gemini-skill

## Pinned environment

- Project commit: `333e81835c3e83437c988ec7d7c6f2d7419be291`
- Test commit: `333e81835c3e83437c988ec7d7c6f2d7419be291`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 8.9 | 1 | 1 | [run](https://argusic.com/run/00533f2a-3ba6-4975-80c8-3366305425f1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Chrome/Chromium browser binary in container, so gemini_* browser tools cannot drive the web UI (system packages cannot be installed, no root). /browser/acquire returns HTTP 500 with "未找到可用浏览器".`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
