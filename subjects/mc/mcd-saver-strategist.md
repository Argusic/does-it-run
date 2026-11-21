# mcd-saver-strategist

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hujjun/mcd-saver-strategist, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcd-saver-strategist

## Pinned environment

- Project commit: `6e2c462c1fd19ff446676034d5f290486942f8ec`
- Test commit: `6e2c462c1fd19ff446676034d5f290486942f8ec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 1 | 0 | 0 | [run](https://argusic.com/run/688da090-2536-4431-b6a9-0aaa5ff486a5) |
| 2 | pass | 100 | 1 | 3.1 | 2 | 2 | [run](https://argusic.com/run/0a6df50d-1c2a-44eb-9a89-911ba02a832f) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `mcp_probe.py needs real MCD_MCP_TOKEN from open.mcd.cn`
- 1 min: `optimizer.py --json prints non-JSON prefix line before the JSON payload`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
