# gemini

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FairwindsOps/gemini, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gemini

## Pinned environment

- Project commit: `67ac67d0dd45014dcd145bb46ee223496ca5bca9`
- Test commit: `67ac67d0dd45014dcd145bb46ee223496ca5bca9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 7 | 0 | 0 | [run](https://argusic.com/run/5d909fea-7464-41f0-8bb4-79dcd7a00173) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
