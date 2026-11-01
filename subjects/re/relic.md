# relic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/heycupola/relic, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/relic

## Pinned environment

- Project commit: `e59f980d2dddf2d8094bc1c14597eeb8b93f5052`
- Test commit: `e59f980d2dddf2d8094bc1c14597eeb8b93f5052`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 61.3 to 61.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 44 | 61.3 | 5 | 5 | [run](https://argusic.com/run/d2a6bbb4-ab28-4cb1-bac0-52ce7886ca31) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Bun not available (no root, unzip missing for curl install)`
- `cargo (Rust) unavailable - packages/runner cannot build or test`
- 5 min: `Bun mock.module leaking between test files in apps/cli - exportSecretsViaServiceToken missing from mock`
- 5 min: `convexTest setUp timed out in beforeEach hooks when running backend tests concurrently`
- `Pre-existing flaky test: should reject an expired API key (timing-dependent race condition)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
