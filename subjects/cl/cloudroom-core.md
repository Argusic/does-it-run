# cloudroom-core

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/davidondrej/cloudroom-core, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cloudroom-core

## Pinned environment

- Project commit: `e760393ec748bedd51f02598b6832010f6876b3a`
- Test commit: `e760393ec748bedd51f02598b6832010f6876b3a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.1 to 33.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 32 | 33.1 | 4 | 4 | [run](https://argusic.com/run/81369796-def0-4dac-881a-0b1e9dd6aa83) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No cargo/rustc in container (README requires Rust 1.89+)`
- 8 min: `cargo test --locked --all-targets failed: 2 observability tests panic (unsafe diagnostic directory) under container umask 0002`
- 10 min: `core_fixture IPv6 subtest fails: '[::1]:0' bind returns EADDRNOTAVAIL (no IPv6 in container)`
- 14 min: `No Docker/postgresql service to run the repo's own core_e2e/foundation suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
