# cli

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cli/cli, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/ac773231-c01b-485b-8993-7c777a807a2a

## Pinned environment

- Project commit: `31d9601e292365301cb5d66c73b4e12334895be1`
- Test commit: `31d9601e292365301cb5d66c73b4e12334895be1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 17.2 to 27.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 17.2 | 0 | 0 | [run](https://argusic.com/run/ac773231-c01b-485b-8993-7c777a807a2a) |
| 2 | pass with mocks | 92 | 27 | 27.5 | 3 | 3 | [run](https://argusic.com/run/a28976b4-8fbc-4860-89e4-086ae6cc0902) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go 1.27+ not installed in container`
- 1 min: `Test failure in internal/ghcmd: PAGER and GH_PAGER env var values in container leaked into test, causing pager precedence tests to fail`
- 1 min: `Test failure in pkg/surveyext: NO_COLOR=1 env var in container disabled ANSI colors, causing color-output tests to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
