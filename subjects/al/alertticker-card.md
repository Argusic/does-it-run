# AlertTicker-Card

**Verdict: runs with mocks.** Argusic Score 61 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/djdevil/AlertTicker-Card, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/alertticker-card

## Pinned environment

- Project commit: `522fed1b955484fb3668087c15d2f1998383de68`
- Test commit: `522fed1b955484fb3668087c15d2f1998383de68`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 5.8 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 5 | 6.2 | 1 | 0 | [run](https://argusic.com/run/9a21d5a2-37e4-46a4-8030-8e60dc877f77) |
| 2 | pass with mocks | 92 | 1 | 5.8 | 0 | 0 | [run](https://argusic.com/run/a3da118e-d3c5-4ca1-b4c7-2b4e5c484610) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Home Assistant instance available to install the Lovelace card into; the card is a client-side JS component with no standalone server or test suite.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
