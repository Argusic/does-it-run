# scipio-erp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ilscipio/scipio-erp, licensed NOASSERTION, written in Java.

Evidence and recordings: https://argusic.com/subject/scipio-erp

## Pinned environment

- Project commit: `c27e6f9964165c8e6e346ee7c88a73b6947c9406`
- Test commit: `c27e6f9964165c8e6e346ee7c88a73b6947c9406`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.9 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 16.9 | 2 | 2 | [run](https://argusic.com/run/29f046d8-18ab-4a0a-8477-ab664ca1fc15) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java (JDK 11/17/21) not pre-installed in container`
- 3 min: `UtilPropertiesTests.testReadXmlLangOldStyle and testReadXmlLangNewStyle NPE - getProperties(Locale) used locale.toString() which returns en_AU (underscore) but keys stored with hyphen (en-AU)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
