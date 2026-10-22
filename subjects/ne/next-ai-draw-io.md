# next-ai-draw-io

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DayuanJiang/next-ai-draw-io, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/next-ai-draw-io

## Pinned environment

- Project commit: `c4ea6957b03095e7fd1940f145c4be53529ab21f`
- Test commit: `c4ea6957b03095e7fd1940f145c4be53529ab21f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.1 to 34.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 32 | 34.1 | 3 | 3 | [run](https://argusic.com/run/5fd7f518-b2f7-4f01-8fad-eefbbbc0807d) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `npm install failed: electron@41 postinstall require() of ES module @electron/get not supported on system Node 18.19.1`
- 2 min: `npm install-scripts gate left esbuild/electron/workerd postinstall binaries unbuilt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
