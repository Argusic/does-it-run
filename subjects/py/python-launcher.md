# python-launcher

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brettcannon/python-launcher, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/python-launcher

## Pinned environment

- Project commit: `3c9f207c07d5fed612b04dbf2980f67d40aa24b3`
- Test commit: `3c9f207c07d5fed612b04dbf2980f67d40aa24b3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.7 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.7 | 1 | 1 | [run](https://argusic.com/run/33aad2c2-2c0e-4487-8941-bdb2260b2545) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Rust toolchain in container (rustc/cargo not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
