# watchstate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arabcoders/watchstate, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/watchstate

## Pinned environment

- Project commit: `23a7fb2eff8fe268974f2ac3bd97616d9e4c179c`
- Test commit: `23a7fb2eff8fe268974f2ac3bd97616d9e4c179c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.3 to 21.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 21.3 | 4 | 4 | [run](https://argusic.com/run/ad48175a-4c17-434c-8c06-98c6b16ad328) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `FrankenPHP v1.13.0 php-cli does not support -v flag and requires .php file extension for scripts - non-.php scripts like bin/console are interpreted as Caddy subcommands`
- 2 min: `Yaml::parseFile returns null on empty files, causing array_replace_recursive TypeError on first HTTP request`
- 2 min: `in_container() returns true due to /.dockerenv, making Config::get(path) default to /config instead of WS_DATA_PATH`
- 5 min: `2 WorkerCommandTest failures: test_incomplete_session and test_child_command - subprocess spawn via bin/console shebang fails with frankenphp php-cli`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
