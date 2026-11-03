# learn-harness-engineering

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/walkinglabs/learn-harness-engineering, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/learn-harness-engineering

## Pinned environment

- Project commit: `77e7a3e21469dcbece2558086c8d91657abeaa40`
- Test commit: `77e7a3e21469dcbece2558086c8d91657abeaa40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 14.8 to 16 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 14.8 | 2 | 2 | [run](https://argusic.com/run/9a9135f0-c33a-43fd-a8d5-e9044109094d) |
| 2 | fail | 80 | 8 | 16 | 3 | 3 | [run](https://argusic.com/run/36a3ab5a-5e54-48ed-8188-0e88895f7490) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `VitePress static build (npm run docs:build) exhausts heap on 512MB machine with 15 locales; OOM on node v18.19.1 even with --max-old-space-size=400`
- 3 min: `Electron startup errors: dbus connection failures, GPU process exit , expected in headless container`

Attempt 2:

- 2 min: `Electron SUID sandbox helper binary not configured correctly`
- 2 min: `Electron binary not fully installed in projects/project-{02,03,04,06}/starter and projects/project-{01,02,03,04,06}/solution`
- `npm engine warnings for langium and marked requiring node>=20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
