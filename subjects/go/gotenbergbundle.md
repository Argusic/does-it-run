# GotenbergBundle

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sensiolabs/GotenbergBundle, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/gotenbergbundle

## Pinned environment

- Project commit: `02aea1653b4debfd45bd52cfe5d6e435867ea3dd`
- Test commit: `02aea1653b4debfd45bd52cfe5d6e435867ea3dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 9.1 | 7 | 7 | [run](https://argusic.com/run/5d861e0e-e8be-4920-b79e-d6ab09612462) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No PHP runtime installed in container`
- 1 min: `Composer not installed`
- 1 min: `PHP extensions phar/mbstring/iconv not loaded for composer`
- 1 min: `No unzip or 7z command for Composer ZipDownloader`
- 1 min: `PHPStan parallel workers could not find Phar class`
- 0.5 min: `PHPStan memory limit exceeded during analysis`
- 1 min: `PHPStan reports Symfony 8 ViewEvent class.notFound and ignore.unmatched for tests/Kernel.php config drift`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
