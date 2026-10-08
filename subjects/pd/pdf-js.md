# pdf.js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mozilla/pdf.js, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/pdf-js

## Pinned environment

- Project commit: `638bcdf0ada7a677c1bace3f11d32ff9090ed7b1`
- Test commit: `638bcdf0ada7a677c1bace3f11d32ff9090ed7b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.5 to 13.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13.5 | 3 | 3 | [run](https://argusic.com/run/cef3ff2b-b9f0-43e8-bd80-d1f34fc7bb38) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 too old; engine requires >=22.22.3`
- `14 CLI unit tests fail with 'Document/OffscreenCanvas is not supported in Node.js'`
- `Puppeteer browser tests cannot run , no Chrome binary available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
