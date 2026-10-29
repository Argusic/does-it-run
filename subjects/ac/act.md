# act

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nektos/act, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/act

## Pinned environment

- Project commit: `a34fa0cf7317d08d9cb3835624092ced76538155`
- Test commit: `a34fa0cf7317d08d9cb3835624092ced76538155`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.3 to 23.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 11 | 23.3 | 4 | 4 | [run](https://argusic.com/run/b2232403-8fee-4f2d-98b0-11a4e1aa752b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go toolchain (1.26+) not installed`
- 2 min: `make install copies to $(PREFIX)/bin/act; default PREFIX=/usr/local not writable`
- 2 min: `Git tests (TestGitFindRef) fail: no user.email/user.name in global config`
- `Docker daemon cannot run in unprivileged container (seccomp blocks user namespaces)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
