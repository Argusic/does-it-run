# vonage-node-sdk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Vonage/vonage-node-sdk, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vonage-node-sdk

## Pinned environment

- Project commit: `5c08b42bfe5db95aaa8aa75619866a605fd36c58`
- Test commit: `5c08b42bfe5db95aaa8aa75619866a605fd36c58`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 5.1 | 1 | 1 | [run](https://argusic.com/run/6f163c50-dcf8-455a-96d9-6134ccde7d11) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container has Node v18 but repo engineStrict requires Node >=22; npm install refused due to engine mismatch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
