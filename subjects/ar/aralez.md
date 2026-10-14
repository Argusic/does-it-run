# aralez

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sadoyan/aralez, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/aralez

## Pinned environment

- Project commit: `ea09efed4d9cb14d64c19d71824e78eb5054b6b1`
- Test commit: `ea09efed4d9cb14d64c19d71824e78eb5054b6b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 57.9 to 57.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 57.9 | 2 | 2 | [run](https://argusic.com/run/3e0cf842-b0f0-4140-9ddb-b49dc3b79a03) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Upstream YAML hostnames must be under 'upstreams:' key, not at top level`
- 5 min: `Healthcheck connection drained non-threaded Python echo server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
