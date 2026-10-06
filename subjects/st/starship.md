# starship

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/starship/starship, licensed ISC, written in Rust.

Evidence and recordings: https://argusic.com/subject/starship

## Pinned environment

- Project commit: `d4d0459c5c24ba8f64663af8714f7858d7fb357b`
- Test commit: `d4d0459c5c24ba8f64663af8714f7858d7fb357b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 80.7 to 80.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 80.7 | 1 | 1 | [run](https://argusic.com/run/e2e9392e-4c5b-4f24-9b77-99b946bf9aff) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Git 2.43.0 does not support --ref-format=reftable (requires 2.45+). COMMON_GIT_PROVIDERS and BARE_GIT_PROVIDERS test fixture arrays included reftable:true variants causing 97 test failures.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
