# octomind

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Muvon/octomind, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/octomind

## Pinned environment

- Project commit: `4cc5600403885e1d9bc2cba6750f5c3c42dbed2f`
- Test commit: `4cc5600403885e1d9bc2cba6750f5c3c42dbed2f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 69.5 to 74.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 74.7 | 2 | 2 | [run](https://argusic.com/run/5256c11a-d23f-422a-8b52-0f36bcc9b964) |
| 2 | pass | 100 | 15 | 69.5 | 2 | 2 | [run](https://argusic.com/run/eb8b8073-0057-4e12-825f-cc9b8406b527) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `config/migrations_inline_tests.rs: template threshold changed from 70000 to 105000, 2 tests had stale expectations`
- 2 min: `telemetry_tests.rs: /.dockerenv exists in container, install_source() short-circuits to 'docker' before 'source'`

Attempt 2:

- 2 min: `test failure: migration test expected compression threshold 70000 but template has 105000`
- 1 min: `test failure: telemetry test expected 'source' but returns 'docker' in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
