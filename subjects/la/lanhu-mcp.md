# lanhu-mcp

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dsphper/lanhu-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/lanhu-mcp

## Pinned environment

- Project commit: `be942fd26f55aac287676f6897353555de8519ac`
- Test commit: `be942fd26f55aac287676f6897353555de8519ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.5 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 6.7 | 0 | 0 | [run](https://argusic.com/run/fe3983c0-9875-4899-a397-bdde94a4d6a6) |
| 2 | pass | 100 | 3 | 5.5 | 0 | 0 | [run](https://argusic.com/run/1e6d2be4-2e13-48ab-b265-62f75b71e3c0) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
