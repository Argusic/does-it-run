# ccs

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kaitranntt/ccs, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ccs

## Pinned environment

- Project commit: `f45fa923f231ecb95b782d3a9edde3cad3476d48`
- Test commit: `f45fa923f231ecb95b782d3a9edde3cad3476d48`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18 to 18 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 11 | 18 | 3 | 3 | [run](https://argusic.com/run/0da4efc4-8223-4954-97c6-d995cec84b1a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `bun not found in PATH`
- 2 min: `config.yaml had version: '2.0' as a string; isUnifiedConfig() requires a number`
- 5 min: `3 tool-sanitization proxy tests failed: forwardJsonBuffered passed transfer-encoding alongside content-length headers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
