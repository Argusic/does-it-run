# react-konva

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/konvajs/react-konva, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-konva

## Pinned environment

- Project commit: `92117241d76bd4b50979fd9607f82ed9b717afe7`
- Test commit: `92117241d76bd4b50979fd9607f82ed9b717afe7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.8 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 9.8 | 0 | 0 | [run](https://argusic.com/run/1e89eaaa-c501-4d73-9d23-3a400c6cd200) |
| 2 | pass | 100 | 13 | 30.3 | 2 | 2 | [run](https://argusic.com/run/418c983a-95ac-4508-b866-45a3d4380429) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `npm install failed on Node 18: Cannot read properties of null (reading 'edgesOut') - peer dependency conflict with vitest@4 requiring Node >=20`
- 3 min: `Playwright and vitest@4 require Node >=20 but only Node 18 was available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
