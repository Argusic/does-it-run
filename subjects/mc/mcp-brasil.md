# mcp-brasil

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mcp-Brasil/mcp-brasil, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-brasil

## Pinned environment

- Project commit: `2efb258370b125bbf190884283ae10f209b9d335`
- Test commit: `2efb258370b125bbf190884283ae10f209b9d335`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 3.3 | 0 | 0 | [run](https://argusic.com/run/6f452b5c-6f1c-4617-a2ab-88dfaf2c79f4) |
| 2 | pass with mocks | 92 | 4 | 5.3 | 0 | 0 | [run](https://argusic.com/run/04a0e054-6c02-4c49-ad12-a5be5574dd58) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
