# vscode-front-matter

**Verdict: could not verify.** Argusic Score 30 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/estruyf/vscode-front-matter, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vscode-front-matter

## Pinned environment

- Project commit: `9d74f1c66154eb5cb8aaaef7d9efecbc9aeff1db`
- Test commit: `9d74f1c66154eb5cb8aaaef7d9efecbc9aeff1db`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 4.8 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 0.5 | 4.8 | 2 | 0 | [run](https://argusic.com/run/abd98619-bb91-496b-ad00-ee0b28db9b47) |
| 2 | fail | 30 | 0.9 | 8.1 | 2 | 0 | [run](https://argusic.com/run/e464b2d8-6185-4a3d-b85d-6d459bf14cf0) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `tsc compilation fails on 30+ errors from third-party type declarations (headlessui, react-router, webpack, date-fns-tz, etc.)`
- `No VS Code runtime available , extension cannot be launched`

Attempt 2:

- `No test framework or test files exist in the repository`
- `VS Code runtime not available in container; extension cannot be launched interactively`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
