# online-shopping-system-advanced

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PuneethReddyHC/online-shopping-system-advanced, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/online-shopping-system-advanced

## Pinned environment

- Project commit: `46403f8fbe4f19b9f85d1abbb217b21e7eab8433`
- Test commit: `46403f8fbe4f19b9f85d1abbb217b21e7eab8433`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 21.5 to 44.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 22 | 44.5 | 4 | 4 | [run](https://argusic.com/run/e9fe88cc-e288-45c0-ac43-151e546c234b) |
| 2 | pass | 100 | 21 | 21.5 | 6 | 6 | [run](https://argusic.com/run/71207686-6706-48d7-9ee2-cd13796a6a00) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP not installed in container`
- 15 min: `MySQL server not available and cannot be installed (no root)`
- 1 min: `mysqli_close() not initially in shim (used by admin/manageuser.php)`
- 2 min: `admin/server/server.php had its own mysqli_connect() call without the shim`

Attempt 2:

- 5 min: `Missing PHP runtime in container`
- 8 min: `Missing MariaDB/MySQL server in container`
- 2 min: `libncurses.so.6 missing for mariadb client`
- 1 min: `liburing.so.2 missing for mariadbd server`
- 1 min: `Database config uses Unix socket (localhost) but only TCP works`
- 2 min: `SQL dump has trailing comma in reviews INSERT and missing user for FK constraint`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
