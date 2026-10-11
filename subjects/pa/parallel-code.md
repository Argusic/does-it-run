# parallel-code

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/johannesjo/parallel-code, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/parallel-code

## Pinned environment

- Project commit: `4026365ae53502740cea98c816e8a2ef68ce6a5f`
- Test commit: `4026365ae53502740cea98c816e8a2ef68ce6a5f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 16.6 | 3 | 3 | [run](https://argusic.com/run/7947f082-b6f4-4c8e-8a5f-b97f59911b5e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node v18.19.1 too old for Vite 8/Electron 40 toolchain (npm install failed to start; package.json engines field missing)`
- 1 min: `npm run test:unit: 5 failures in electron/documents/setup.test.ts because git commit failed with 'Author identity unknown' in fresh container`
- 4 min: `Packaged Electron main process hit FATAL 'GPU process isn't usable. Goodbye.' (SIGTRAP) after ~44s on Xvfb when launched with only --no-sandbox`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
