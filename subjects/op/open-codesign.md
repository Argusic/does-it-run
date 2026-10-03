# open-codesign

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenCoworkAI/open-codesign, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-codesign

## Pinned environment

- Project commit: `26c84984809b82f816eb9907a10eb706718f14af`
- Test commit: `26c84984809b82f816eb9907a10eb706718f14af`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 60 to 60 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 60 | 60 | 4 | 4 | [run](https://argusic.com/run/69931dcc-c720-4fd2-9af3-e3b1b766d6e6) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18 installed but project requires 22+`
- 1 min: `pnpm not found`
- 3 min: `Build scripts blocked for esbuild, koffi, protobufjs, @google/genai, electron-winstaller`
- 3 min: `3 web-research tests failed: System Chrome not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
