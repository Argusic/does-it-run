# poznote

**Verdict: runs.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/timothepoznanski/poznote, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/poznote

## Pinned environment

- Project commit: `c6c3f1010814788d6f2962b29745676f6ad8aa85`
- Test commit: `c6c3f1010814788d6f2962b29745676f6ad8aa85`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 9.3 to 36.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 36.3 | 3 | 3 | [run](https://argusic.com/run/84f565a5-8b80-4142-9ef7-8f5a83797d64) |
| 2 | pass with mocks | 72 | 2 | 9.3 | 3 | 0 | [run](https://argusic.com/run/0ca37127-ee4e-43ff-b72f-48bb0f3cdb3b) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Static PHP CLI binary built-in server crashes on router-based request handling; requires router-free '-t src/' mode`
- 2 min: `Cannot install Python packages (pip not available) - MCP server tests skipped`
- `No root access in container - used static PHP binary instead of apt packages`

Attempt 2:

- `PHP not installed (needed for web app)`
- `Docker not installed (needed for compose deployment)`
- `Node.js v18 incompatible with Vite 8+ (CustomEvent undefined)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
