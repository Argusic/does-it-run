# theia-ide

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eclipse-theia/theia-ide, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/theia-ide

## Pinned environment

- Project commit: `2db26f3162e722bb6cbd530c5c7ae459f9bdbf2e`
- Test commit: `2db26f3162e722bb6cbd530c5c7ae459f9bdbf2e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8.4 to 15.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 15.3 | 3 | 3 | [run](https://argusic.com/run/0c76578a-f98a-4c95-84ad-1af32ad54f7b) |
| 2 | pass with mocks | 92 | 8 | 8.4 | 5 | 5 | [run](https://argusic.com/run/6118e028-60db-4028-a820-a9f9eb8dd937) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js version 18.19.1 is installed but project requires >=24; yarn not found`
- `Puppeteer postinstall fails trying to download Chrome`
- 10 min: `native-keymap native addon fails to build: missing libx11-dev and libxkbfile-dev`

Attempt 2:

- 2 min: `Node.js v18.19.1 in container but project requires >=24`
- 1 min: `yarn not available on PATH`
- 1 min: `puppeteer postinstall fails to download Chrome (no unzip)`
- 2 min: `native-keymap node-gyp rebuild fails: missing libx11-dev and libxkbfile-dev headers`
- 1 min: `yarn engine check blocks run commands even with node 24`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
