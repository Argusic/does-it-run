# lcu

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amontlabs/lcu, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/lcu

## Pinned environment

- Project commit: `748303e9315eea4f1877413bd69f00cb270e3d12`
- Test commit: `748303e9315eea4f1877413bd69f00cb270e3d12`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 44 | 7.1 | 2 | 2 | [run](https://argusic.com/run/0cae5d53-24d4-46f6-8896-2e4388ba6346) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npm adapter tests: 4 Node 18 MockTimers.enable signature mismatches`
- `npm adapter tests: 3 test files require OMP/Pi harness installations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
