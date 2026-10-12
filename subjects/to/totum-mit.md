# totum-mit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/totumonline/totum-mit, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/totum-mit

## Pinned environment

- Project commit: `45980e25653d06a23682ec51cd2100aa51a0850a`
- Test commit: `45980e25653d06a23682ec51cd2100aa51a0850a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.8 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.8 | 6 | 6 | [run](https://argusic.com/run/a0516445-7129-4cd1-9795-59e550d99033) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP not installed in container`
- 1 min: `Composer not installed`
- 3 min: `PostgreSQL not installed`
- 1 min: `Missing ext-soap and ext-xsl in static PHP`
- 1 min: `CLI.totum.php.ini missing`
- 1 min: `FrankenPHP php-server needs Host header routing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
