# Client

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GitLabPHP/Client, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/client

## Pinned environment

- Project commit: `45bac88ea81752b201daf542dfd65521578e2144`
- Test commit: `45bac88ea81752b201daf542dfd65521578e2144`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.5 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 26 | 12.5 | 4 | 3 | [run](https://argusic.com/run/b01dc9a9-9f13-4c3c-80a4-da833475cd74) |

## What was observed on a clean machine

Attempt 1:

- 17 min: `Composer failed to download dist packages: no zip extension, no unzip/7z, no zstd binary`
- 3 min: `PHPUnit install failed: ext-tokenizer missing`
- 2 min: `PHP 8.5 triggers deprecation warning loading xml.so from duplicate ini files`
- 4 min: `Pinned psalm/phar 5.26.1 rejects PHP 8.5 (supports only up to 8.3)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
