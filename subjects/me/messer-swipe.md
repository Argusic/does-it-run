# messer-swipe

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jakobbjelver/messer-swipe, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/messer-swipe

## Pinned environment

- Project commit: `68e9e75c2f064c157d6a7b6630fa148aa37c56fb`
- Test commit: `68e9e75c2f064c157d6a7b6630fa148aa37c56fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 6.8 | 4 | 4 | [run](https://argusic.com/run/02903478-33fe-42e2-bd3e-56ec50111820) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 installed but project requires >=24`
- 1 min: `npm install scripts for esbuild and sharp needed approval`
- 2 min: `next start does not work with output: standalone configuration, must use node .next/standalone/server.js instead`
- 1 min: `Standalone server bound to container hostname, not reachable via localhost`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
