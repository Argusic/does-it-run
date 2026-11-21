# pi-from-scratch

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SaladDay/pi-from-scratch, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-from-scratch

## Pinned environment

- Project commit: `599d0ba646c5e737881ca1a576c8009ee065cffd`
- Test commit: `599d0ba646c5e737881ca1a576c8009ee065cffd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.3 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 4.3 | 0 | 0 | [run](https://argusic.com/run/5067c3dd-617c-4e18-8725-1cf3d714e9b4) |
| 2 | pass with mocks | 92 | 4 | 4.7 | 1 | 1 | [run](https://argusic.com/run/eaea80ad-733a-4024-b381-bc36193ad861) |

## What was observed on a clean machine

Attempt 2:

- `Node.js v18.19.1 is too old for the web/ subproject (requires >=22.13.0 for Next.js 16). The core project (src/) compiles and runs fine on v18.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
