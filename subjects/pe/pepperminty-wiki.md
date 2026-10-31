# Pepperminty-Wiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sbrl/Pepperminty-Wiki, licensed MPL-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/pepperminty-wiki

## Pinned environment

- Project commit: `7c5062727234e8101e2de19dda995efc0b185d1b`
- Test commit: `7c5062727234e8101e2de19dda995efc0b185d1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 9.9 | 5 | 5 | [run](https://argusic.com/run/c1829170-a5e5-430d-a92f-d9459e4f0ea8) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `php binary and composer missing from container; npm deps only`
- 4 min: `PHP 8.3 E_DEPRECATED from ${ex_error} string interpolation printed into response body, breaking header()/http_response_code() output on CLI and web; firstrun/CLI output polluted`
- 2 min: `php -S dev server backgrounded by a normal shell exited after first request`
- `php index.php exec version exits 1 (upstream behavior: version is a shell command whose return value is swallowed by the exec dispatch)`
- `php index.php and php index.php exec help on a fresh dir are swallowed by the firstrun 307 redirect until firstrun_complete is set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
