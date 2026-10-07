# tsdproxy

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/almeidapaulopt/tsdproxy, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/tsdproxy

## Pinned environment

- Project commit: `75bd326c09158efe48603f2a51f0af066a77876b`
- Test commit: `75bd326c09158efe48603f2a51f0af066a77876b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.9 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 6.9 | 1 | 1 | [run](https://argusic.com/run/ce957cac-2718-43f1-86bd-0278b9b2ba96) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `goleak_test.go missing ignore for http2 readLoop goroutine in tailscale package`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
