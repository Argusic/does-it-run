# lx-music-mobile

**Verdict: runs with mocks.** Argusic Score 82.4 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lyswhut/lx-music-mobile, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lx-music-mobile

## Pinned environment

- Project commit: `d2956044533150057d65bfeaf2ae0fb5179433f5`
- Test commit: `d2956044533150057d65bfeaf2ae0fb5179433f5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 3; wall time 11.3 to 23.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 1.5 | 13.8 | 3 | 2 | [run](https://argusic.com/run/f6a0bb3a-6c09-4a77-a18a-308cc07b772a) |
| 2 | pass with mocks | 92 | 3 | 23.5 | 5 | 5 | [run](https://argusic.com/run/96641936-885f-4a4d-8019-8260990e9f2d) |
| 3 | fail | 70 | 2 | 11.3 | 2 | 1 | [run](https://argusic.com/run/0c822c23-78dd-45bd-a06f-a34c4b1d77ee) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Metro bundler killed by cgroup memory limit when using default parallelism (192 workers on 8GB limit)`
- `TypeScript check found 5 pre-existing type errors (no fix needed, pre-existing repo issues)`
- `No Android SDK or Java installed, cannot build native APK or run on emulator`

Attempt 2:

- 5 min: `Metro bundle process killed by OOM with default memory`
- `No Android SDK or Java in container`
- `npm audit reports 25 vulnerabilities`
- `TypeScript has 8 pre-existing type errors`
- `Publish/parseChangelog.js has ESM syntax error`

Attempt 3:

- 1 min: `Metro bundle build OOM-killed on first attempt (container memory limit)`
- `5 pre-existing TypeScript errors (Timer type mismatches, nullable listId)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
