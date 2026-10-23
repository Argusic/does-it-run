# pi-app

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/justhil/pi-app, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-app

## Pinned environment

- Project commit: `c26373f70cdd775584ecb868e9959f602dd01ca6`
- Test commit: `c26373f70cdd775584ecb868e9959f602dd01ca6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5.5 | 2 | 2 | [run](https://argusic.com/run/ef90a854-91b1-4c13-9b68-dd493c0cf69d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 was too old (requires >=22.19.0)`
- 1 min: `Electron sandbox not usable inside container (chrome-sandbox not owned by root with setuid)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
