# foliate-js

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/johnfactotum/foliate-js, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/foliate-js

## Pinned environment

- Project commit: `78914aef4466eb960965702401634c2cb348e9b1`
- Test commit: `78914aef4466eb960965702401634c2cb348e9b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 14.7 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 17.4 | 0 | 0 | [run](https://argusic.com/run/e8a50c72-19dc-4017-9f0f-c7554ebb4334) |
| 2 | pass with mocks | 92 | 14.8 | 14.7 | 1 | 1 | [run](https://argusic.com/run/179dc8a1-4c59-4135-9864-cdb7c10b2a85) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `JSDOM CDATA handling mismatch: CDATA sections become comment nodes, breaking isTextNode logic in page2 tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
