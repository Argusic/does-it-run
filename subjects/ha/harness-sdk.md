# harness-sdk

**Verdict: runs.** Argusic Score 55 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/strands-agents/harness-sdk, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/harness-sdk

## Pinned environment

- Project commit: `15da9dca2cd6f870684fdc27a2498bebbd00b62d`
- Test commit: `15da9dca2cd6f870684fdc27a2498bebbd00b62d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 68 to 77.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 77.8 | 0 | 0 | [run](https://argusic.com/run/0c30d717-cf5a-4f52-a0cb-67198f9bc4bf) |
| 2 | pass | 90 | 3 | 68 | 2 | 1 | [run](https://argusic.com/run/acfa6b9f-9ce4-4ad6-bbee-4a047fc81fd4) |

## What was observed on a clean machine

Attempt 2:

- 9 min: `test_gather_runs_calls_concurrently flaky timing: expected < 1.1s, took 2.41s in container`
- 5 min: `test_call_tool_sync_image_content missing tests_integ/resources/yellow.png from repo root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
