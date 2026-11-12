# Crawler-Detect

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JayBizzle/Crawler-Detect, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/crawler-detect

## Pinned environment

- Project commit: `a96c1a5fdc3d4949a524e5e9edebba9db0290db8`
- Test commit: `a96c1a5fdc3d4949a524e5e9edebba9db0290db8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.8 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.8 | 0 | 0 | [run](https://argusic.com/run/1732a888-582e-4466-95fb-cd931d318107) |
| 2 | pass | 100 | 10 | 18.1 | 5 | 5 | [run](https://argusic.com/run/8deaaac7-21c7-468a-afdb-140529d0aa14) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `PHP and Composer not preinstalled; had to extract php8.3-cli from .deb`
- 1 min: `Composer installer required phar and iconv extensions`
- 2 min: `composer install required ext-dom, ext-xmlwriter, ext-tokenizer`
- 2 min: `php8.3-zip .so failed to load (libzip.so.4 missing from system)`
- 2 min: `composer install --prefer-source took several minutes due to git clones`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
