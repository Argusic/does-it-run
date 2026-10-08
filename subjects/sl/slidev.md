# slidev

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/slidevjs/slidev, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/slidev

## Pinned environment

- Project commit: `73053ab2b9653ed475960301b56e1ce4439d9c75`
- Test commit: `73053ab2b9653ed475960301b56e1ce4439d9c75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 9.1 | 3 | 3 | [run](https://argusic.com/run/d45e35c3-a657-4544-b677-a1df62d9e245) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in container`
- 1 min: `Node.js v18 installed, requires >=22.12.0`
- 1 min: `One inline snapshot test mismatched (base64 encoding difference)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
