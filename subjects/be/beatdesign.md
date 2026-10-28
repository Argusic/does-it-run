# BeatDesign

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BeatAPI/BeatDesign, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/beatdesign

## Pinned environment

- Project commit: `d2ef270174426da119574e9aa096e86edb777b5d`
- Test commit: `d2ef270174426da119574e9aa096e86edb777b5d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 27 | 6.1 | 4 | 4 | [run](https://argusic.com/run/819be58b-1b65-4379-b65f-62822454f552) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node 18.19.1 shipped in container (requires >=22); pnpm not available`
- 2 min: `paraglide-js compilation failed on Node 18 (crypto.subtle undefined in tsx)`
- 3 min: `Vite 8 required Node >=22.12 but downloaded Node 22.0.0`
- `TypeScript typecheck errors (routeTree.gen.ts not found at typecheck time, createFileRoute generic mismatch)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
