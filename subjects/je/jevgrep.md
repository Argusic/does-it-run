# jevgrep

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dzhng/jevgrep, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jevgrep

## Pinned environment

- Project commit: `baf2d1c4c719e339f10e7dfb20cf90f9fe402e01`
- Test commit: `baf2d1c4c719e339f10e7dfb20cf90f9fe402e01`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.5 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 6.2 | 3 | 3 | [run](https://argusic.com/run/be8e4ad6-111d-446a-bcef-c52168f94390) |
| 2 | pass | 100 | 25 | 4.5 | 3 | 3 | [run](https://argusic.com/run/de7e93a9-1974-408e-a09d-e60128b47783) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js version too old (v18, requires 22+)`
- 1 min: `No bun binary in PATH (npm-installed bun is musl-linked, incompatible with glibc Ubuntu)`

Attempt 2:

- 3 min: `System Node.js 18.19.1 does not meet the >=22 requirement`
- 1 min: `bun not pre-installed in the container`
- 2 min: `node --experimental-strip-types not supported in v22.0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
