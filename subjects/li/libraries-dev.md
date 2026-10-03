# Libraries.dev

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jakubantalik/Libraries.dev, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/libraries-dev

## Pinned environment

- Project commit: `8670e9ade04725598dd458ce277a130a9f3fafda`
- Test commit: `8670e9ade04725598dd458ce277a130a9f3fafda`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 4.9 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 2.5 | 4.9 | 0 | 0 | [run](https://argusic.com/run/2f2c8656-e207-4010-b6dc-86990f251756) |
| 2 | fail | 80 | 5 | 6.5 | 1 | 1 | [run](https://argusic.com/run/7ad3019a-8689-49eb-a661-70b9ea96ea58) |

## What was observed on a clean machine

Attempt 2:

- `Container Node version (18.19.1) below repository minimum (>=20 in .node-version), causing EBADENGINE warnings`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
