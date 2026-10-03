# vibecode-pro-max-kit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/withkynam/vibecode-pro-max-kit, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/vibecode-pro-max-kit

## Pinned environment

- Project commit: `3bcb2f9891308fcaa305e2b64027bd0a7dc8251e`
- Test commit: `3bcb2f9891308fcaa305e2b64027bd0a7dc8251e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.5 to 27.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 17.5 | 5 | 5 | [run](https://argusic.com/run/592be4e1-c53c-4540-89da-bdf2de8f5c39) |
| 2 | pass | 100 | 8 | 27.8 | 3 | 3 | [run](https://argusic.com/run/32c108e4-b46b-4e35-9e10-9657bf7fe886) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18 lacks fs.globSync (needs 22+)`
- 2 min: `AC-5 assertion too narrow for process/general-plans/ and process/_seeds/ paths`
- 3 min: `transcript-parser assertDeepEquals fails on extra agentId:null key`
- 5 min: `chatMessages shares _signalIndex inflating control-signal indices`

Attempt 2:

- 2 min: `Node.js v18 , kit needs v22+ for fs.globSync`
- 3 min: `resolve-manifest.mjs: fs.globSync with exclude:[] array silently fails (must be function)`
- 1 min: `e2e test AC-5 assertion too narrow , rejected valid kit-owned paths in legacyDeletions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
