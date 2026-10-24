# dscode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thinkany-ai/dscode, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/7838dd76-adf2-4a62-9454-e12b6c2d3607

## Pinned environment

- Project commit: `1ce0328cfa856700f6c955f5429ca00b08d99ea5`
- Test commit: `1ce0328cfa856700f6c955f5429ca00b08d99ea5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.4 | 2 | 2 | [run](https://argusic.com/run/7838dd76-adf2-4a62-9454-e12b6c2d3607) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Test hooks.test.ts failed: No OS sandbox backend available (no Docker, no macOS seatbelt, no unshare permission)`
- 1 min: `package:check fails: requires Go toolchain to build Windows sandbox binary on Linux`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
