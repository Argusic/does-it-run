# streama

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/streamaserver/streama, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/streama

## Pinned environment

- Project commit: `1fa79534ee09e25f2473cc4787b106996008a442`
- Test commit: `1fa79534ee09e25f2473cc4787b106996008a442`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.2 to 27.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 27.2 | 3 | 3 | [run](https://argusic.com/run/3c85e617-de8c-4391-afa6-33940ef0e5df) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ZipHelper.groovy: bare 'File(...)' resolved to 'streama.File' domain class instead of java.io.File`
- 2 min: `ZipHelperSecuritySpec.groovy: 'File.createTempDir()' is a Guava method, not available`
- 3 min: `OpensubtitlesServiceSecuritySpec.groovy: 'File.createTempDir()' (Guava) and 'Mock(Object)' for settingsService , Mock(Object) can't dispatch getValueForName`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
