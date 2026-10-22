# runn

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k1LoW/runn, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/runn

## Pinned environment

- Project commit: `651af61c6e8d976c2a81f4cab550fdda999bf8a5`
- Test commit: `651af61c6e8d976c2a81f4cab550fdda999bf8a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 44.4 to 75.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 75.8 | 0 | 0 | [run](https://argusic.com/run/421af589-8606-4a2e-9448-47d427244e87) |
| 2 | pass with mocks | 92 | 14 | 44.4 | 5 | 5 | [run](https://argusic.com/run/1b11f483-773e-4188-98b5-ba4ebb783624) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `go toolchain missing in container (go.mod requires go 1.26.8; no root for apt)`
- 42 min: `github:// and gist:// fetch tests fail with 'no credentials found' (real GitHub API/keys required)`
- 17 min: `TestHTTPRunnerRunUsingGitHubAPI fails with real GitHub 401 with placeholder token; its /users/{id} OpenAPI spec lacked a 401 response`
- 1 min: `TestRunnerRenew and TestHostRules/CDP fail: exec google-chrome not found`
- `TestUseParentStore fails: no /var/run/docker.sock`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
