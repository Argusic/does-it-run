# nimbalyst

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nimbalyst/nimbalyst, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nimbalyst

## Pinned environment

- Project commit: `34b14f33e48fd639d32c0f5eb7d77561bdccd2a4`
- Test commit: `34b14f33e48fd639d32c0f5eb7d77561bdccd2a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 22.2 to 40.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 22.2 | 4 | 4 | [run](https://argusic.com/run/8b376c02-117e-4267-80d5-0340ac816615) |
| 2 | pass | 100 | 41 | 40.6 | 6 | 6 | [run](https://argusic.com/run/35b9ec16-f690-4b9c-9455-77e76d2fed63) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js is v18.19.1, project requires >=24, npm 9.2 requires >=11`
- 1 min: `vite build out of memory (FATAL ERROR: Ineffective mark-compacts near heap limit)`
- 1 min: `typecheck failed in nimbalyst-memory workspace: engine dist not built`
- `2 unit tests fail: 'zip: command not found'`

Attempt 2:

- 1 min: `Node 18 installed but project requires Node 24+`
- 2 min: `OOM during runtime build with default heap`
- 3 min: `zip command not found (marketplace tests)`
- 2 min: `unzip command not found (marketplace tests)`
- 3 min: `extension-sdk dist missing; collab-bundle build failed`
- 2 min: `collab-bundle dist missing; docsUiStoreBinding test failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
