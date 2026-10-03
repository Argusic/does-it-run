# knowledge-catalog

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GoogleCloudPlatform/knowledge-catalog, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/knowledge-catalog

## Pinned environment

- Project commit: `22efaa5402775a7c4d4c37f89e41258daaf3cb65`
- Test commit: `22efaa5402775a7c4d4c37f89e41258daaf3cb65`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 9.5 | 10.1 | 2 | 0 | [run](https://argusic.com/run/3a13feb0-385c-4da6-b551-aa00d410c467) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npm install for toolbox/enrichment hangs indefinitely (depends on file:../mdcode and hits resolution deadlock)`
- 0.5 min: `2 kcmd tests fail: missing gcloud CLI binary (expected for GCP-dependent components)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
