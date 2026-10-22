# ubi

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/houseabsolute/ubi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/ubi

## Pinned environment

- Project commit: `bcccac9e7e1cc479cdefb2d28984ca154e1f2311`
- Test commit: `bcccac9e7e1cc479cdefb2d28984ca154e1f2311`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 8 | 0 | 0 | [run](https://argusic.com/run/3162e2f8-e5ae-4204-bc03-b30508782584) |
| 2 | pass | 100 | 1.2 | 4.8 | 2 | 2 | [run](https://argusic.com/run/8ca39800-2dee-49bb-be54-4b7425023908) |

## What was observed on a clean machine

Attempt 2:

- `23 CLI integration tests fail needing GITHUB_TOKEN to authenticate with GitHub API (401 Unauthorized)`
- 1.2 min: `No Rust toolchain was pre-installed in the container; installed via rustup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
