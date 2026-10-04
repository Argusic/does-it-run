# jevgrep

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dzhng/jevgrep, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jevgrep

## Pinned environment

- Project commit: `baf2d1c4c719e339f10e7dfb20cf90f9fe402e01`
- Test commit: `baf2d1c4c719e339f10e7dfb20cf90f9fe402e01`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 6.2 | 3 | 3 | [run](https://argusic.com/run/be8e4ad6-111d-446a-bcef-c52168f94390) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js version too old (v18, requires 22+)`
- 1 min: `No bun binary in PATH (npm-installed bun is musl-linked, incompatible with glibc Ubuntu)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
