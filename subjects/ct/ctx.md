# ctx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ctxrs/ctx, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/ctx

## Pinned environment

- Project commit: `e61850204eb3f2b7b57bb06345630c912b8e9642`
- Test commit: `e61850204eb3f2b7b57bb06345630c912b8e9642`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 3.7 | 1 | 1 | [run](https://argusic.com/run/3166e3ef-3327-4669-9206-44410f50bb4c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `ctx setup (auto-run during install) failed with 'History refresh failed: all_provider_terminal_coverage_unavailable' , no agent history sources exist in this fresh container (expected).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
