# headscale

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/juanfont/headscale, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/headscale

## Pinned environment

- Project commit: `f227d68781a1777c41f16036f4260b27f01ab014`
- Test commit: `f227d68781a1777c41f16036f4260b27f01ab014`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 83.2 to 83.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 1.5 | 83.2 | 3 | 0 | [run](https://argusic.com/run/6ebb1eee-4b5b-4679-8977-9177726efd7a) |

## What was observed on a clean machine

Attempt 1:

- `tscli binary not found in PATH`
- `tofu binary not found in PATH`
- `No Docker daemon available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
