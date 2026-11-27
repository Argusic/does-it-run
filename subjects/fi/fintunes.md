# fintunes

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leinelissen/fintunes, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fintunes

## Pinned environment

- Project commit: `13f25aca597bce0b04d0ed4e6292050cb680bae7`
- Test commit: `13f25aca597bce0b04d0ed4e6292050cb680bae7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.9 | 4 | 4 | [run](https://argusic.com/run/b0015287-09d6-4073-be88-482a8611a3b2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not in PATH`
- 1 min: `pnpm approve-builds needs interactive terminal`
- 2 min: `Jest test suite failed with ESM import syntax`
- 2 min: `Node.js v18 too old (requires >=20.19.4)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
