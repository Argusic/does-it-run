# GoGogot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aspasskiy/GoGogot, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gogogot

## Pinned environment

- Project commit: `88859aa02799f490cca118cfa33f7723c97b6fbe`
- Test commit: `88859aa02799f490cca118cfa33f7723c97b6fbe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9 to 9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 9 | 3 | 3 | [run](https://argusic.com/run/899f2df7-c4a9-483c-a4d5-272e00c71242) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go binary not found in container`
- 4 min: `Telegram bot library calls getMe on init requiring real credentials`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
