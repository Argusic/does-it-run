# open-genjutsu

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Anil-matcha/open-genjutsu, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/open-genjutsu

## Pinned environment

- Project commit: `f2045a2a90bdca35e3b4b249f5d4cde9c35ba957`
- Test commit: `f2045a2a90bdca35e3b4b249f5d4cde9c35ba957`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 17.7 | 1 | 1 | [run](https://argusic.com/run/b49acc9b-64b7-4649-a978-1d51612400eb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Self-signed SSL certificate CN mismatch with 127.0.0.1 when connecting to mock API`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
