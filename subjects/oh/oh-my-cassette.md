# oh-my-cassette

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Cassette-Editor/oh-my-cassette, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/oh-my-cassette

## Pinned environment

- Project commit: `fd19f89353d768878bb193ad6d58a59d7035bda9`
- Test commit: `fd19f89353d768878bb193ad6d58a59d7035bda9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 9.7 | 3 | 3 | [run](https://argusic.com/run/0a92efef-ff4b-40a3-aace-d4d085ce1350) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `uv was not on PATH and 'pip install --user uv' was rejected with an externally-managed-environment (PEP 668) error`
- 2 min: `llms-install.md claimed 'uvx oh-my-cassette==0.6.0 --version' prints 'oh-my-cassette 0.5.0', but it printed 0.6.0`
- 3 min: `uv.lock still locked oh-my-cassette 0.5.0 and 'uv lock --check' reported the lockfile needs updating`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
