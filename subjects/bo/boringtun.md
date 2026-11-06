# boringtun

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/boringtun, licensed BSD-3-Clause, written in Rust.

Evidence and recordings: https://argusic.com/subject/boringtun

## Pinned environment

- Project commit: `6dcc889a95ad82400932f785d874421d70308195`
- Test commit: `6dcc889a95ad82400932f785d874421d70308195`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.8 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5 | 1 | 1 | [run](https://argusic.com/run/f7d8e15a-23e0-47a6-877a-ec5a3e871239) |
| 2 | pass with mocks | 92 | 16 | 3.8 | 3 | 3 | [run](https://argusic.com/run/c146c1a5-2eda-4caa-909b-17d7fdbf691d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `sudo not available for integration tests that need TUN/tap devices`

Attempt 2:

- 10 min: `Rust toolchain (rustc, cargo) not found in container`
- 3 min: `sudo not available; cargo config had 'runner = sudo -E' for unix tests`
- `Integration tests require Docker and sudo privileges`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
