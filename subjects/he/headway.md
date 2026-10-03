# headway

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/headwaymaps/headway, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/headway

## Pinned environment

- Project commit: `82e3a00b40983bc9ffc5793f3a656b9e53d84b86`
- Test commit: `82e3a00b40983bc9ffc5793f3a656b9e53d84b86`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 10.2 | 4 | 4 | [run](https://argusic.com/run/afe93863-fef6-449f-9db5-27a0232ed803) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install on frontend failed due to incompatible Node version (v18.19.1, requires >=20) and yarn engine constraint`
- 1 min: `vitest requires Node >= 22 (rolldown imports styleText from node:util)`
- 1 min: `pelias generate_config tests failed: missing areas.csv symlink and outdated test expectations for planet builds (dataHost field)`
- `Docker not available in container - cannot run integration or browser tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
