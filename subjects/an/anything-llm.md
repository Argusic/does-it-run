# anything-llm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mintplex-Labs/anything-llm, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/anything-llm

## Pinned environment

- Project commit: `58ae6fee08e10e649ca13d0cfc55598d90422cf8`
- Test commit: `58ae6fee08e10e649ca13d0cfc55598d90422cf8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.9 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.3 | 16.9 | 1 | 1 | [run](https://argusic.com/run/c8e4f9f4-6e3c-43a6-a31d-2da53120dc26) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Production mode fails because server/.env is not created by yarn setup:envs (only .env.development is). STORAGE_DIR env var is missing, causing a crash in server/utils/files/index.js at path.resolve().`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
