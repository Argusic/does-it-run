# qinglong

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/whyour/qinglong, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/qinglong

## Pinned environment

- Project commit: `a67d44cde54fbf2943f62a9e01051f54166540ee`
- Test commit: `a67d44cde54fbf2943f62a9e01051f54166540ee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.1 | 6.6 | 0 | 0 | [run](https://argusic.com/run/25e47619-edc3-4d11-88ae-b0d2f46d9b32) |
| 2 | pass | 100 | 1 | 6.6 | 3 | 3 | [run](https://argusic.com/run/3c024293-303e-4cdf-9e7c-b95623fb6c2e) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pnpm 8.3.1 not available globally (no root), and pnpm is the required package manager`
- 1 min: `.env file missing at project root , back/config/index.ts throws on missing .env`
- 1 min: `Data subdirectories (config, scripts, log, db, etc.) missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
