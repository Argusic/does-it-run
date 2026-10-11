# PiDeck

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ayuayue/PiDeck, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pideck

## Pinned environment

- Project commit: `4105d98e823031b129d115fef71b6990dee8f4b1`
- Test commit: `4105d98e823031b129d115fef71b6990dee8f4b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.9 to 15.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 15.9 | 3 | 3 | [run](https://argusic.com/run/a34fe5e6-523d-44d7-9a6d-c7bee3e42531) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node 18.19.1 / npm 9.2.0 too old (needs Node >=20.17 and npm ^11.6.2)`
- `5 pre-existing test failures in extensionManager.test.mjs (TypeScript compilation error in loadTsCommonJs helper, 'Unexpected token :')`
- `2 pre-existing test failures in docsSharedImages.test.mjs and markdownPathTailTruncation.test.mjs (ErrUnknownFileExtension for .ts imports)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
