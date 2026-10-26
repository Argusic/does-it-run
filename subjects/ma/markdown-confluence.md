# markdown-confluence

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/markdown-confluence/markdown-confluence, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/markdown-confluence

## Pinned environment

- Project commit: `185e9027e6719760416060707f4d21ba9821e982`
- Test commit: `185e9027e6719760416060707f4d21ba9821e982`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.7 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.7 | 3 | 3 | [run](https://argusic.com/run/3925f13f-022a-44ca-a0e0-452447387a6d) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node.js v18.19.1 in container; repo requires v24.15.0`
- 3 min: `Puppeteer browser download failed , no 'unzip' on system and incomplete cache`
- 1 min: `Chrome crashpad handler missing execute permission`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
