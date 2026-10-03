# fabric-video-editor

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AmitDigga/fabric-video-editor, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fabric-video-editor

## Pinned environment

- Project commit: `0d428f6433aa147a20032759bc613bfe5df26ec3`
- Test commit: `0d428f6433aa147a20032759bc613bfe5df26ec3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 4.8 to 26.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.17 | 4.8 | 0 | 0 | [run](https://argusic.com/run/af29de9a-bca3-4fe9-90ca-7b94f61a18bf) |
| 2 | fail | 80 | 25.8 | 26.1 | 3 | 3 | [run](https://argusic.com/run/a42582a8-bac9-4f9a-9336-19f24726b5b3) |

## What was observed on a clean machine

Attempt 2:

- `npm install has 26 vulnerabilities (3 critical)`
- 15 min: `next build fails with OOM (exit 137) during 'Collecting page data' phase - only 770MB RAM available, fabric.js+ffmpeg imports exceed memory during SSR pre-rendering`
- 5 min: `node-canvas (canvas npm package) cannot be installed - pixman-1 dev library missing and no root to install system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
