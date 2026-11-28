# birdview

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Qiuner/birdview, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/birdview

## Pinned environment

- Project commit: `11436ff3a6b1df70a3e17ea4e95e335a5304f730`
- Test commit: `11436ff3a6b1df70a3e17ea4e95e335a5304f730`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 6.6 | 4 | 4 | [run](https://argusic.com/run/d288fd5a-4122-4065-9185-4b6a223bb3ce) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `The shell's time wrapper was unavailable, causing the initial install command to fail.`
- 0.2 min: `node scripts/check-install.mjs exits with 'Run through npm run check:install.'`
- 0.2 min: `npm audit reports one moderate vulnerability in fast-uri.`
- 0.5 min: `An interaction probe timed out clicking the hidden English option in a native select.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
