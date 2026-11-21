# LightAgent

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wanxingai/LightAgent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/lightagent

## Pinned environment

- Project commit: `827c6b5bbb616fe5d0f879eaead1b229228522d6`
- Test commit: `827c6b5bbb616fe5d0f879eaead1b229228522d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 1.4 to 1.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 1.7 | 0 | 0 | [run](https://argusic.com/run/b589bf89-a42c-41c1-a979-04c33401d794) |
| 2 | pass with mocks | 92 | 1.4 | 1.4 | 1 | 1 | [run](https://argusic.com/run/3eed60fc-1b4a-460c-9abb-e3664959f787) |

## What was observed on a clean machine

Attempt 2:

- 0.3 min: `mcp 1.10.1 requires pydantic._internal._typing_extra.eval_type_backport which was removed in pydantic 2.14.x`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
