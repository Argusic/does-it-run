# gpt-load

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tbphp/gpt-load, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gpt-load

## Pinned environment

- Project commit: `ae59a0ae85159ef009f6b182756104eb7f57849e`
- Test commit: `ae59a0ae85159ef009f6b182756104eb7f57849e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 8.1 to 20.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 8.9 | 0 | 0 | [run](https://argusic.com/run/6ee45d33-464d-4568-9e2b-cf3321cc07a7) |
| 2 | pass | 100 | 45 | 20.3 | 5 | 5 | [run](https://argusic.com/run/b1acd6c9-92ad-4080-a2fc-3b19ac1731ea) |
| 3 | pass | 100 | 10 | 8.1 | 3 | 3 | [run](https://argusic.com/run/3ec3c17c-ff33-49a0-8431-bafad2efcdc6) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go compiler not found in environment`
- 2 min: `Node.js v18.19.1 too old; web UI requires >=24.11.0`
- 2 min: `corepack not in PATH so pnpm was unavailable`
- 2 min: `Web UI build failed: @rolldown/binding-linux-x64-gnu missing (frozen lockfile skips optional deps)`
- `Docker compose contract tests fail: docker not in PATH (6 subtest failures)`

Attempt 3:

- 2 min: `Go 1.27 not pre-installed in container`
- 2 min: `Node.js v18.19.1 too old (requires >=24.11.0), pnpm not installed`
- 1 min: `6 tests fail in internal/webui (container_contract_test.go) - docker not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
