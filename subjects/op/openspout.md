# openspout

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openspout/openspout, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/openspout

## Pinned environment

- Project commit: `f6a027ad119abe7c1986cee397bae0694e2af4bd`
- Test commit: `f6a027ad119abe7c1986cee397bae0694e2af4bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 9.4 to 20.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 20.1 | 4 | 4 | [run](https://argusic.com/run/6ba9d62e-b123-456a-ba27-ebd7298cf3d0) |
| 2 | pass with mocks | 92 | 5 | 9.4 | 5 | 5 | [run](https://argusic.com/run/926cc072-75f4-43a5-87ef-d83958342e95) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP and Composer not pre-installed`
- 1 min: `Static PHP warns extensions can't be dynamically loaded`
- 1 min: `phpunit.xml failOnAllIssues=true blocks tests due to coverage warning`
- 2 min: `libxml 2.12.5 max amplification check breaks quadratic blowup test`

Attempt 2:

- 3 min: `PHP and composer not pre-installed; PHP 8.4.16 was downloaded from pmmp/PHP-Binaries as a static binary, Composer 2.11.2 from getcomposer.org`
- 8 min: `ext-iconv not available; library uses iconv for encoding conversions and tests called iconv() directly from namespaced context`
- 5 min: `ODS quadratic blowup test readSheetsVisibility expands entities causing PHP memory exhaustion; libxml2 2.15.1 limits entity amplification but ODS reader still generates >1M rows before protection kicks in`
- 3 min: `XLSX quadratic blowup test failed because libxml2 2.15.1 correctly blocks entity amplification, throwing IOException instead of processing the file`
- 1 min: `No code coverage driver available; pcov/xdebug not present in static PHP binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
