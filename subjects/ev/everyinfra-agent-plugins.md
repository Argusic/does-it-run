# everyinfra-agent-plugins

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/everyinfra/everyinfra-agent-plugins, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/everyinfra-agent-plugins

## Pinned environment

- Project commit: `75983ac2b120990787cdf8090e379a968554e9c0`
- Test commit: `75983ac2b120990787cdf8090e379a968554e9c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.2 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 3.2 | 0 | 0 | [run](https://argusic.com/run/09a23c05-e9ed-405b-92d8-43dd41036657) |
| 2 | pass | 100 | 8 | 7.1 | 2 | 2 | [run](https://argusic.com/run/9dac3939-532c-41b4-970a-ca0113bc0a67) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `pip3 install everyinfra failed: externally-managed-environment (PEP 668)`
- 0.3 min: `unzip not available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
