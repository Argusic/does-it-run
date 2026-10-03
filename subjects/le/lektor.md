# lektor

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lektor/lektor, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/lektor

## Pinned environment

- Project commit: `9ebd5dcbaa44f50c59e971c2e1d22039c548e230`
- Test commit: `9ebd5dcbaa44f50c59e971c2e1d22039c548e230`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 25 | 11.3 | 2 | 1 | [run](https://argusic.com/run/f9e2bb1e-0c8a-4ec9-b03f-d6c789c85468) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18 cannot natively run .ts files via 'node build.ts'`
- `jsdom@29 requires Node >=20, breaks ToggleGroup.test.tsx (JS test)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
