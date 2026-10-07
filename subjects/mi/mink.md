# Mink

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/minkphp/Mink, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/mink

## Pinned environment

- Project commit: `1efa659944300f34e4109178fab1118472370df6`
- Test commit: `1efa659944300f34e4109178fab1118472370df6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.5 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 11.5 | 5 | 5 | [run](https://argusic.com/run/34c83609-ee98-41f6-a83c-2253c4aab82a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP runtime installed in container`
- 3 min: `PHP extensions missing (phar, iconv, mbstring, dom, xml, tokenizer, ctype, curl)`
- 4 min: `Composer could not extract zip dist packages: no unzip/7z binary and PHP zip extension unloadable (libzip.so.4 missing)`
- 1 min: `PHPStan crashed with 128M default memory limit`
- `PHP zip extension could not load (libzip.so.4 shared library absent; no root to install libzip)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
