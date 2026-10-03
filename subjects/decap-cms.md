# decap-cms

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/decaporg/decap-cms, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/decap-cms

## Pinned environment

- Project commit: `1d5868347d3d8648d7d5f7f59fc1b46595881b29`
- Test commit: `1d5868347d3d8648d7d5f7f59fc1b46595881b29`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18 to 18 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 18 | 2 | 2 | [run](https://argusic.com/run/ff7bcca3-25be-4ccb-aeb5-36326ba3aec6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pnpm not found in PATH; npm install -g failed due to /usr/local permissions`
- 5 min: `clean-stack@5.2.0 overridden in pnpm-workspace.yaml but is ESM-only; aggregate-error@3.1.0 (Cypress dep) uses require('clean-stack'), causing ERR_REQUIRE_ESM in Cypress postinstall`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
