# JeecgBoot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jeecgboot/JeecgBoot, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/jeecgboot

## Pinned environment

- Project commit: `87d7f938d47d2585618bcfc5a31d125801cbff27`
- Test commit: `87d7f938d47d2585618bcfc5a31d125801cbff27`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 49.7 to 55.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 54 | 55.4 | 8 | 8 | [run](https://argusic.com/run/ad243ee1-5d10-4447-ad47-fc7b77e4c6d0) |
| 2 | pass | 100 | 60 | 49.7 | 7 | 7 | [run](https://argusic.com/run/976cfe1c-7d2f-4b76-8e91-51cf3f9e9ac5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java JDK installed in container`
- 1 min: `No Maven installed in container`
- 1 min: `No pnpm available`
- 2 min: `pnpm lockfile had stale npmmirror tarball URLs causing policy rejection`
- 3 min: `pnpm 12 requires allowBuilds config in pnpm-workspace.yaml for postinstall scripts`
- 2 min: `Node.js 18.19.1 lacks 'styleText' export from node:util needed by Vite 8 / rolldown`
- 1 min: `Maven could not resolve jeecg private repo (maven.jeecg.com) artifacts`
- `3 of 70 backend tests failed due to DNS resolution failure (hostname could not be resolved) in isolated container`

Attempt 2:

- 5 min: `Node.js 18 insufficient for Vite 8 / Node.js 20+ required`
- 2 min: `pnpm 12 incompatible with lockfile; required pnpm 9`
- 1 min: `jest-environment-jsdom missing (Jest 28+ change)`
- 5 min: `Java/Maven not pre-installed in container`
- 1 min: `Maven download URL 404`
- 1 min: `3 DnsResolution failures in SsrfFileTypeFilterTest (container has no DNS for cdn.example.com)`
- 1 min: `18 system-start tests fail: ApplicationContext needs MySQL+Redis containers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
