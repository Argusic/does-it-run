# dingo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dingodb/dingo, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/dingo

## Pinned environment

- Project commit: `bb96a7414c86746733a7527639363d22394427e5`
- Test commit: `bb96a7414c86746733a7527639363d22394427e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.5 to 10.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.5 | 4 | 4 | [run](https://argusic.com/run/807efefe-9256-4f1d-b6f9-ceae38b474a2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No JDK available in container`
- 1 min: `dingo-expr and calcite versions 5.0.0-SNAPSHOT not found in Maven`
- 2 min: `API ExprCompiler.getAdvancedExprCompiler() not found in dingo-expr 4.0.0`
- 1 min: `Git submodule dingo-proto not initialized`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
