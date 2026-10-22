# Markdown-Viewer

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ThisIs-Developer/Markdown-Viewer, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/markdown-viewer

## Pinned environment

- Project commit: `5b29c569960d31027df3e6f6820612c9980e581a`
- Test commit: `5b29c569960d31027df3e6f6820612c9980e581a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.8 | 0 | 0 | [run](https://argusic.com/run/f45482ea-b5c1-4409-be7c-a46db9dedab2) |
| 2 | pass | 100 | 6.1 | 10 | 2 | 2 | [run](https://argusic.com/run/c4fd36f4-dc29-4fd1-a2ef-ebd454e0422d) |

## What was observed on a clean machine

Attempt 2:

- 2.1 min: `Node.js 18 present, project requires >=22`
- 1 min: `desktop-app/resources/libs/ missing , 29 CDN libraries not downloaded`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
