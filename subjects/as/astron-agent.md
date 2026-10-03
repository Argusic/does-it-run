# astron-agent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iflytek/astron-agent, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/astron-agent

## Pinned environment

- Project commit: `b4f8ed57460cbfb32016a4afd3fd7212987d33c3`
- Test commit: `b4f8ed57460cbfb32016a4afd3fd7212987d33c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.8 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 13.8 | 8 | 8 | [run](https://argusic.com/run/e75a9154-7d0f-4722-a310-b76054526296) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm peer dependency conflict with react-json-view requiring React 17`
- 0.5 min: `Python externally-managed environment blocks pip install`
- 2 min: `Agent pyproject.toml flat-layout confuses setuptools discovery`
- 3 min: `Frontend Vite build runs out of heap memory (JS OOM)`
- 0.5 min: `Missing jsonschema dependency in common/.venv`
- 1 min: `Missing snowflake-id dependency in common/venv (vs .venv)`
- 2 min: `Missing botocore in common/.venv (not listed in pyproject.toml deps)`
- 1 min: `common module tests need PYTHONPATH to resolve 'common.*' imports`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
