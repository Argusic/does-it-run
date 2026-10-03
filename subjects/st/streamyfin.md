# streamyfin

**Verdict: runs.** Argusic Score 78.9 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/streamyfin/streamyfin, licensed MPL-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/streamyfin

## Pinned environment

- Project commit: `cb00ae36955b3f9cafd814872ad2298a965e22c0`
- Test commit: `cb00ae36955b3f9cafd814872ad2298a965e22c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 4.3 to 15.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 6.1 | 3 | 3 | [run](https://argusic.com/run/690f8554-883e-43a9-85b3-71a7ec945594) |
| 2 | pass | 100 | 15 | 15.2 | 5 | 5 | [run](https://argusic.com/run/b8e62402-9323-4d3a-9959-2c956c28b074) |
| 3 | fail | 36.67 | 0.5 | 4.3 | 3 | 1 | [run](https://argusic.com/run/0dc63836-4b8f-4105-ad07-a6f7b432cd64) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun command not found: required by project but absent from container`
- 1 min: `Node.js v18.19.1 below project minimum of >=20`
- 0.5 min: `expo-doctor reports 34 expo SDK 57 packages at patch versions below expected: @sentry/react-native major mismatch (7.x vs 8.x) and 33 expo packages at older patch versions`

Attempt 2:

- 2 min: `bun binary not available in container`
- 3 min: `Node.js v18.19.1 too old for expo-doctor (requires >=20.19.4)`
- 1 min: `34 Expo SDK packages at minor/patch versions below SDK 57 expected range`
- 1 min: `Duplicate native modules (expo-asset, expo-constants, expo-font, @expo/log-box) after upgrade`
- 1 min: `React Native DevTools SUID sandbox crash on startup`

Attempt 3:

- `TypeScript typecheck failed with 100 pre-existing errors in Jellyseerr integration code (implicit any types, missing server module declarations)`
- `Expo doctor: 34 SDK packages at minor/patch versions behind SDK 57 + @sentry/react-native major mismatch (8.23.0 vs ~7.11.0). Pre-existing in lockfile.`
- 3 min: `Node.js v18 was outdated; installed nvm + Node v22.23.3 to resolve`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
