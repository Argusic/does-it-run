# aeria

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aeria-org/aeria, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/aeria

## Pinned environment

- Project commit: `0a4e587b579c59a61ab5ca92064969a137a4dc5e`
- Test commit: `0a4e587b579c59a61ab5ca92064969a137a4dc5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 2 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 2 | 0 | 0 | [run](https://argusic.com/run/d7afb55e-c094-426b-8a6b-04e5d7008c25) |
| 2 | pass | 100 | 8.5 | 6.5 | 5 | 5 | [run](https://argusic.com/run/0e12ade9-22da-474d-8612-27b25f326c58) |

## What was observed on a clean machine

Attempt 2:

- 2.5 min: `Node.js v18 installed but project requires >=23`
- 1 min: `pnpm not available`
- 1 min: `.npmrc prefix setting conflicted with nvm`
- 0.5 min: `core postinstall script ran before build (no dist/__scripts__)`
- 0.5 min: `reference.spec.ts timed out at default 5s`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
