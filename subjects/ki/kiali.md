# kiali

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kiali/kiali, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kiali

## Pinned environment

- Project commit: `da2138100483733b4a7f6b1a9c050ade1a7c50b5`
- Test commit: `da2138100483733b4a7f6b1a9c050ade1a7c50b5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.3 to 32.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 32.3 | 4 | 4 | [run](https://argusic.com/run/6781ce49-8f72-40f2-9ddc-2afea92884af) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.26.3 required but not installed in environment`
- 11 min: `Node.js 18 lacks corepack support and yarn 4 at packageManager version`
- `npm install --legacy-peer-deps with Node 18 failed on peer dependency conflict (monaco-editor)`
- 3 min: `yarn 4.12.0 (packageManager field) is not published to npm; only yarn 1.22.22 and 2.4.3 available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
