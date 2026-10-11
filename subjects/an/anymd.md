# anymd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SylphxAI/anymd, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/anymd

## Pinned environment

- Project commit: `0a70224816e39d89bd34caa58c105eb9115abc8f`
- Test commit: `0a70224816e39d89bd34caa58c105eb9115abc8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.1 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 16.1 | 2 | 2 | [run](https://argusic.com/run/219dc9e2-0a68-487a-93b4-f86f5dc98b0e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Rust toolchain installed`
- 1 min: `No bun installed; bun.sh installer failed (no unzip)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
