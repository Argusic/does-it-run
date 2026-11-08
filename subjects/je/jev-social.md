# jev-social

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/socai-io/jev-social, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/jev-social

## Pinned environment

- Project commit: `2f02e6f4c60943e679993634ad1017b0c97efff5`
- Test commit: `2f02e6f4c60943e679993634ad1017b0c97efff5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 2.7 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10 | 10.7 | 2 | 2 | [run](https://argusic.com/run/f01b33e2-0ced-4e21-b071-5b292a66ce84) |
| 2 | pass with mocks | 92 | 0.2 | 2.7 | 2 | 2 | [run](https://argusic.com/run/669475e1-906a-4442-b0f8-cb9611baa768) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18 insufficient (needs >=22, .nvmrc says 24). .toSorted() missing in Node 18`
- 1 min: `Shallow git clone missing pinned release commits referenced by tests`

Attempt 2:

- 1 min: `Three git-dependent tests failed because immutable release commit SHAs (8369621fd..., 5b8fcf3f...) were not present in the shallow clone`
- 3 min: `Node.js was v18 but project requires >=22 (engines.node)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
