# fluent-bit

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fluent/fluent-bit, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/fluent-bit

## Pinned environment

- Project commit: `046accf6aded7906f66a1baf0202da349e521736`
- Test commit: `046accf6aded7906f66a1baf0202da349e521736`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 36.2 to 36.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 30 | 36.2 | 5 | 4 | [run](https://argusic.com/run/9c7e36d9-fb60-470e-a966-556cb01dcddd) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `m4 not installed (required for flex/bison build)`
- 5 min: `flex not installed (required by CMake find_package)`
- 8 min: `bison not installed (required by CMake find_package)`
- 5 min: `libyaml-dev not installed (required by FLB_CONFIG_YAML)`
- `flb-it-network fails due to IPv6 disabled in container (nosuid noexec container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
