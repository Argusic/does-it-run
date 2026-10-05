# PanWatch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TNT-Likely/PanWatch, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/panwatch

## Pinned environment

- Project commit: `d2d2a869b735e6c3c83f4ec6aa61c142dc91a3e3`
- Test commit: `d2d2a869b735e6c3c83f4ec6aa61c142dc91a3e3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6.3 | 7.8 | 2 | 2 | [run](https://argusic.com/run/8f096899-ad65-4d52-a052-dddd5bef77ce) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `pnpm not installed globally, needed for frontend builds`
- 2.5 min: `No CJK fonts on system; WeasyPrint PDF tests failed asserting Chinese text in PDF text layer`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
