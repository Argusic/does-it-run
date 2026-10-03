# grav

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/getgrav/grav, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/grav

## Pinned environment

- Project commit: `64c39ae93fcca07bd28f360801871d8316a8543d`
- Test commit: `64c39ae93fcca07bd28f360801871d8316a8543d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7.5 | 6.7 | 3 | 3 | [run](https://argusic.com/run/25adb46b-6d31-4a60-a18d-12862ed47514) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `GLOB_BRACE undefined in AssetsTest.php on static PHP 8.3.0`
- 1.5 min: `ComposerTest::testGetComposerLocation failed: command -v composer returned empty`
- 1 min: `Static PHP 8.3.0 lacked GD JPEG and WebP support`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
