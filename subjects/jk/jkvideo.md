# JKVideo

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tiajinsha/JKVideo, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jkvideo

## Pinned environment

- Project commit: `3592d036b1930af19d78e4a08bf3e60399c54467`
- Test commit: `3592d036b1930af19d78e4a08bf3e60399c54467`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 6.6 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.3 | 6.6 | 3 | 3 | [run](https://argusic.com/run/a3b47a83-82eb-49de-9318-4ac6eb9758f0) |
| 2 | fail | 80 | 18.47 | 7.8 | 4 | 4 | [run](https://argusic.com/run/930ce265-df20-4638-b1e2-4159414a4117) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 was outdated , required >=20.19.4 for React Native 0.83 packages`
- 1 min: `sentry shim had JSX parsing ambiguity on generic <T>`
- `Expo DevTools chrome-sandbox error (non-fatal, root needed)`

Attempt 2:

- 2.1 min: `Node.js v18 is too old for React Native 0.83 / Expo SDK 55 (requires >=20.19.4)`
- 1.5 min: `Expo export fails on Node 18 with 'parseEnv is not a function'`
- 0.5 min: `shims/sentry-react-native.web.tsx: generic <T> interpreted as JSX tag in TSX, TS17008/TS1382 errors`
- 4 min: `TypeScript errors in 8 files: fontWeight type, Image pointerEvents, FileSystem.getInfoAsync size option type deprecated, undefined vs null mismatch, react-native-video shim event handler signatures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
