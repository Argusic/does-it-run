# github-act-runner

**Verdict: runs with mocks.** Argusic Score 77 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ChristopherHX/github-act-runner, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/github-act-runner

## Pinned environment

- Project commit: `25b9930ac6e8c65185dcbba863ce2ee221ce7273`
- Test commit: `25b9930ac6e8c65185dcbba863ce2ee221ce7273`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 77 | 3 | 7.8 | 4 | 1 | [run](https://argusic.com/run/b470a00e-c571-49b9-ac1a-c892063a36e3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.24 not installed in container`
- `uuidgen system tool not available, caused grouping.yml test failure`
- `Docker not available, prevented container-based workflow tests`
- `README states go 1.21 required but go.mod requires go 1.24`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
