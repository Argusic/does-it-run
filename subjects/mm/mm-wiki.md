# mm-wiki

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/phachon/mm-wiki, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mm-wiki

## Pinned environment

- Project commit: `d976d0c604847503bfcea2829489ce278e2c6cf7`
- Test commit: `d976d0c604847503bfcea2829489ce278e2c6cf7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 33.8 to 45.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 45.6 | 4 | 4 | [run](https://argusic.com/run/36295279-8a55-4797-9d32-1e0cbe32269c) |
| 2 | pass with mocks | 92 | 8 | 33.8 | 6 | 6 | [run](https://argusic.com/run/8b4231bf-0fab-4057-92d0-f042303d55ad) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 5 min: `MariaDB not installed in container`
- 3 min: `Database schema not set up`
- `2 pre-existing test failures in app/utils (zipx_test.go use hardcoded developer paths)`

Attempt 2:

- 2 min: `Go compiler not pre-installed - downloaded Go 1.21.13 tarball`
- 15 min: `MySQL/MariaDB not available - no root access to install system packages`
- 10 min: `Mock MySQL did not support COM_STMT_PREPARE (prepared statements) initially`
- 8 min: `COM_STMT_EXECUTE parameter value parsing was incorrect (wrong byte offsets, types/values interleaved, string encoding)`
- 5 min: `Login failed with binary protocol results since text row format was used after COM_STMT_EXECUTE`
- 2 min: `mw_log table schema was missing path, post, get, referer, message, user_agent columns in mock`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
