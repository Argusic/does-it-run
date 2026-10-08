# jellyfin-audio-player

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leinelissen/jellyfin-audio-player, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jellyfin-audio-player

## Pinned environment

- Project commit: `13f25aca597bce0b04d0ed4e6292050cb680bae7`
- Test commit: `13f25aca597bce0b04d0ed4e6292050cb680bae7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.7 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 8.7 | 4 | 4 | [run](https://argusic.com/run/7bec3dc8-841c-4f02-9b1f-c250002efc58) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH after npm install -g`
- 1 min: `pnpm approve-builds requires interactive terminal`
- 3 min: `Jest fails: Cannot use import statement outside a module on react-native/jest/setup.js caused by pnpm virtual store paths not matching transformIgnorePatterns`
- 3 min: `Metro fails: configs.toReversed is not a function (Node 18 lacks Array.prototype.toReversed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
