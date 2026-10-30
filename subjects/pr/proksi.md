# proksi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/luizfonseca/proksi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/proksi

## Pinned environment

- Project commit: `fd6cb0791665bf88645c05de077c8ffcb94f2ddf`
- Test commit: `fd6cb0791665bf88645c05de077c8ffcb94f2ddf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 8.5 | 2 | 2 | [run](https://argusic.com/run/7f6d4f16-3112-4004-a6a0-0e3648cd0c49) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `cargo/rustup build scripts emitted non-fatal '/bin/sh: 1: Bad substitution' bash-isms under the sh shell`
- 3 min: `HTTPS request failed: No certificate found for host mysite.localhost, TLS handshake error, curl code 000`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
