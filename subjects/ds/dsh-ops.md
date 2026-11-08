# dsh-ops

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/T-Auto/dsh-ops, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dsh-ops

## Pinned environment

- Project commit: `b963fb29e03ad21ebe76d6f552c70f0544ca92b9`
- Test commit: `b963fb29e03ad21ebe76d6f552c70f0544ca92b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 11.1 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 16.9 | 4 | 4 | [run](https://argusic.com/run/883a1d2f-6b48-4483-aa1a-fe3ff38c54c3) |
| 2 | fail | 20 | n/a | 11.1 | 0 | 0 | [run](https://argusic.com/run/126e04d9-6832-4de3-8c66-341a60ea3f49) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18 too old (requires ^22.19 or >=24)`
- 1 min: `No Rust toolchain installed`
- `First test run had 1 failure in bench-gates suite: baseline materialization test failed because commit hash not found in shallow clone`
- `npm in ~/.local/bin from old node install could not find its modules when node 22 was used`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
