# fredy

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/orangecoding/fredy, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/fredy

## Pinned environment

- Project commit: `1d0c3d70d5808df08dbf5c53780a39a572437ab3`
- Test commit: `1d0c3d70d5808df08dbf5c53780a39a572437ab3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 6.2 | 2 | 2 | [run](https://argusic.com/run/d059234f-2e2e-4a42-91b0-fa3f8c916353) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 installed but project requires >=22.22.0`
- 0.5 min: `yarn not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
