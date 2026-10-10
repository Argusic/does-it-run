# ShahanPanel

**Verdict: runs with mocks.** Argusic Score 52.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HamedAp/ShahanPanel, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/shahanpanel

## Pinned environment

- Project commit: `19d74866d7cf3196a5f2b9892df667b3f7dae5e5`
- Test commit: `19d74866d7cf3196a5f2b9892df667b3f7dae5e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 65.9 to 80.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 13.33 | 20 | 65.9 | 3 | 2 | [run](https://argusic.com/run/83feb10f-16eb-4c02-ac23-f8ad625aac46) |
| 2 | pass with mocks | 92 | 100 | 80.7 | 3 | 3 | [run](https://argusic.com/run/a2ef3309-891f-4d8f-96ef-faf9fc086088) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `PHP CLI and mysqli/ionCube runtime missing from clean container; built PHP 8.1.30 from source and loaded ionCube Loader v15.5.1 to compensate`
- 12 min: `No MySQL/MariaDB server present; built MariaDB 10.11.19 from source (submodules replaced, ncurses/bison/m4 built) and started mariadbd on 127.0.0.1:3306 as uid 1001`
- 10 min: `The panel code is ionCube-encoded with a key not available in this container; every encoded entrypoint (p/index.php, p/login.php, apiV1/api.php, user/index.php, sub.php, newbot/bot.php) in the official 10.1/10.3.1/11.0 release zips dies wit`

Attempt 2:

- 30 min: `release panel files (p/*.php, user/login.php) are ionCube-encrypted with an encoder key the official loader cannot find; root installer requires a real Ubuntu root shell, unavailable in this container`
- 20 min: `static PHP 8.1 binaries segfault when executing ionCube-encoded files while the standard PHP 8.1.34 CLI decodes them cleanly`
- 15 min: `panel wired to absolute /var/www/html/p paths and hardcoded localhost DB socket`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
