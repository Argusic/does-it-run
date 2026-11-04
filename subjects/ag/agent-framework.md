# agent-framework

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/agent-framework, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-framework

## Pinned environment

- Project commit: `6f1522a50b66f117da34cc25ea299ba24a528b15`
- Test commit: `6f1522a50b66f117da34cc25ea299ba24a528b15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 25.8 to 28 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 28 | 0 | 0 | [run](https://argusic.com/run/2fda2f59-ce63-401b-b715-ccd88db0e49b) |
| 2 | pass with mocks | 92 | 0.2 | 25.8 | 4 | 4 | [run](https://argusic.com/run/a4cd8aab-f972-4146-b558-eee93b2f69b2) |

## What was observed on a clean machine

Attempt 2:

- 0.2 min: `uv was absent, although DEV_SETUP requires it.`
- 13 min: `uv run poe test -P core hung for over 13 minutes because pytest-xdist -n auto saw 192 logical CPUs while the container affinity allowed 4 CPUs.`
- 4 min: `DevUI retained sparse EntityInfo type unknown after lazy loading, logged Unsupported entity type: unknown, and returned HTTP 200 with empty output text.`
- 3 min: `The first local Responses mock returned non-streaming JSON while DevUI executes Agent.run(stream=True), producing empty mapped text.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
