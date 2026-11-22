# kraken-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/krakenfx/kraken-cli, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/kraken-cli

## Pinned environment

- Project commit: `671cdd7f1483409f7b45554725f2a07ac5abd33f`
- Test commit: `671cdd7f1483409f7b45554725f2a07ac5abd33f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.9 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.5 | 9.1 | 0 | 0 | [run](https://argusic.com/run/51efd390-33b9-430e-ae9a-db94c7f51f79) |
| 2 | pass | 100 | 2 | 7.9 | 2 | 2 | [run](https://argusic.com/run/ede4eed1-b6f9-40ea-9797-e614dab23215) |

## What was observed on a clean machine

Attempt 2:

- 0.2 min: `Rust toolchain not installed in container`
- 0.1 min: `Initial paper buy failed with lock contention`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
