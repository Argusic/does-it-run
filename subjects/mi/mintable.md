# mintable

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kevinschaich/mintable, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mintable

## Pinned environment

- Project commit: `6d6c4255eda1954f94102ee41b92a58516f34922`
- Test commit: `6d6c4255eda1954f94102ee41b92a58516f34922`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 2.9 | 1 | 1 | [run](https://argusic.com/run/791c3143-c5e9-43b8-bfa8-837d89bde50d) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `TypeScript 3.8.3 fails to compile node_modules from latest @types/minimatch which uses TS syntax not supported in TS 3.8`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
