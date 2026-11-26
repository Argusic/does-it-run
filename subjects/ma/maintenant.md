# maintenant

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kOlapsis/maintenant, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/maintenant

## Pinned environment

- Project commit: `fa25b92c2485135d51a69a76ff4e71a1fa1f6bde`
- Test commit: `fa25b92c2485135d51a69a76ff4e71a1fa1f6bde`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.1 to 10.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.1 | 1 | 1 | [run](https://argusic.com/run/dd929fab-46a9-4bbf-a0ea-3d6e77b13779) |
| 2 | pass | 100 | 10 | 10.5 | 4 | 4 | [run](https://argusic.com/run/f133e1eb-6704-4655-9054-6f7f8bfb94e1) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`

Attempt 2:

- 2 min: `Go binary not installed in container`
- 2 min: `Node.js 18 incompatible with frontend test dependencies`
- 1 min: `@tailwindcss/oxide native binary missing in npm install`
- 3 min: `jsdom ESM incompatibility with @exodus/bytes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
