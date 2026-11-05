# autoharness

**Verdict: runs.** Argusic Score 93.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tigerless-labs/autoharness, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/806fa7ec-2244-4fe9-b478-6daebf25fd15

## Pinned environment

- Project commit: `48500a5ec0aa14a426ef0ba08ba6d3562c040de5`
- Test commit: `48500a5ec0aa14a426ef0ba08ba6d3562c040de5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 5.9 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5.9 | 0 | 0 | [run](https://argusic.com/run/806fa7ec-2244-4fe9-b478-6daebf25fd15) |
| 2 | pass with mocks | 87 | 6 | 7.1 | 4 | 3 | [run](https://argusic.com/run/f7c645a5-368b-41ac-bf4c-41ec4dffb76b) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Unquoted ${CLAUDE_PLUGIN_ROOT} in all four hook commands produced validator warnings and could break under install paths containing spaces.`
- 1 min: `The first mock returned 404 because it did not strip the request query string from /v1/messages?beta=true.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
