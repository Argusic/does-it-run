# omg.dev

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BennyKok/omg.dev, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/omg-dev

## Pinned environment

- Project commit: `015f45a98970f5709f2f2ab4b3de49237b29fdc9`
- Test commit: `015f45a98970f5709f2f2ab4b3de49237b29fdc9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 38.5 to 38.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 62 | 38.5 | 3 | 2 | [run](https://argusic.com/run/6cd7c896-e07c-465e-bdd6-1f5ea9e35418) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not found in container, installed via npm --prefix ~/.local`
- 1 min: `thinking level test failed because opencode now has reasoning levels in the local model catalog cache`
- `44 test failures are environment-specific (Chromium/desktop, mobile/native, dbus, AI agent subscriptions, hosted service) , see test_depth note`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
