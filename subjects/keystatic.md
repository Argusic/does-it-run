# keystatic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Thinkmill/keystatic, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/keystatic

## Pinned environment

- Project commit: `c51af99a27adff9cb82633b788ea0f8c6fc18b6c`
- Test commit: `c51af99a27adff9cb82633b788ea0f8c6fc18b6c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 67.7 to 67.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 67.7 | 3 | 3 | [run](https://argusic.com/run/f53c75b7-39ad-431a-afc1-c4ad9b6dc3a9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 doesn't support .mts files; needed v24`
- `13 snapshot mismatches in markdoc editor tests`
- `18 timeout failures across keystatic (27) and keystar/ui (4) projects (tests exceed 5000ms default)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
