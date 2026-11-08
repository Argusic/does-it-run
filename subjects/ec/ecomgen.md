# EcomGen

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linbei0/EcomGen, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ecomgen

## Pinned environment

- Project commit: `894e7fb62d50eb8f1f79959cadba97bb791bdc03`
- Test commit: `894e7fb62d50eb8f1f79959cadba97bb791bdc03`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14.13 | 14.2 | 4 | 4 | [run](https://argusic.com/run/cc63fd74-e3fe-4c9d-9e48-5800d4c958be) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18 - pnpm@11 requires Node 22.13+`
- 2.5 min: `Redis not installed on system (no apt/sudo access)`
- 1 min: `sharp native module not loaded - install script skipped because sharp (and its @img/* optional deps) not in pnpm-workspace.yaml allowBuilds list`
- 0.5 min: `Build failed on packages/ecom-suite-forge - Node 18 doesn't support import.meta.dirname`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
