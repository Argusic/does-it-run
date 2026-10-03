# learn-harness-engineering

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/walkinglabs/learn-harness-engineering, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/learn-harness-engineering

## Pinned environment

- Project commit: `77e7a3e21469dcbece2558086c8d91657abeaa40`
- Test commit: `77e7a3e21469dcbece2558086c8d91657abeaa40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.8 to 14.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 14.8 | 2 | 2 | [run](https://argusic.com/run/9a9135f0-c33a-43fd-a8d5-e9044109094d) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `VitePress static build (npm run docs:build) exhausts heap on 512MB machine with 15 locales; OOM on node v18.19.1 even with --max-old-space-size=400`
- 3 min: `Electron startup errors: dbus connection failures, GPU process exit , expected in headless container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
