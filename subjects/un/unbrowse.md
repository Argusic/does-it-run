# unbrowse

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unbrowse-ai/unbrowse, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/unbrowse

## Pinned environment

- Project commit: `7bcf436b8ca8662d05606a566e063b1b0d9b89b0`
- Test commit: `7bcf436b8ca8662d05606a566e063b1b0d9b89b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 80.3 to 80.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 78 | 80.3 | 5 | 5 | [run](https://argusic.com/run/01d152ac-a220-40e6-987c-432be929bfa8) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `rustup/cargo absent; foundry absent`
- 10 min: `bindgen: libclang not found (btls-sys build)`
- 35 min: `Linux secret-service absent: root key creation failed`
- 5 min: `passkey tests: Chrome crashed without --no-sandbox in container`
- 2 min: `learn_shop tests failed: debug agent-browser not built`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
