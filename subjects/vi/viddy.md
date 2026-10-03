# viddy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sachaos/viddy, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/viddy

## Pinned environment

- Project commit: `b56efe0876f255ade025d6b77fb9f3f30099675b`
- Test commit: `b56efe0876f255ade025d6b77fb9f3f30099675b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 10.2 | 2 | 2 | [run](https://argusic.com/run/f9b2269e-909a-49c6-84d9-f187e25254a1) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not found (no rustc/cargo)`
- 0.5 min: `Runtime panic 'attempt to subtract with overflow' at exec_result.rs:188 when area.width is 0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
