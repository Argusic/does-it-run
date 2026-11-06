# abacusai-bot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/abacusai/abacusai-bot, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/abacusai-bot

## Pinned environment

- Project commit: `68c307fe16b5dfbf140fa0a800c6bcf571e70529`
- Test commit: `68c307fe16b5dfbf140fa0a800c6bcf571e70529`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.7 | 2 | 2 | [run](https://argusic.com/run/601a96e2-e87a-4c90-b994-fef9b8f8ec8e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js was v18, project requires v22`
- 2 min: `Electron binary not downloaded at install time, missing LICENSES.chromium.html`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
