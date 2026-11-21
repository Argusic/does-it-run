# node-hue-api

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/peter-murray/node-hue-api, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/node-hue-api

## Pinned environment

- Project commit: `0318111a39aa144bc944b1b629a4e2259e9ff087`
- Test commit: `0318111a39aa144bc944b1b629a4e2259e9ff087`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 28.7 to 53.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 1 | 53.8 | 1 | 0 | [run](https://argusic.com/run/2cd46330-ff01-4f64-9bbd-3179ddf31044) |
| 2 | pass with mocks | 92 | 0.5 | 28.7 | 4 | 4 | [run](https://argusic.com/run/431366e4-1320-473e-a974-b6043cf90531) |

## What was observed on a clean machine

Attempt 1:

- 35 min: `23 of 49 tests fail because they require a real Philips Hue bridge on the local network (UPnP/mDNS found none) or access to discovery.meethue.com, which returned HTTP 429 from this container`

Attempt 2:

- 10 min: `Mock bridge required , no physical Hue Bridge on network`
- 1 min: `Discovery (nupnp.ts) hit real API and got rate-limited (HTTP 429)`
- 1 min: `No test config file (~/.node-hue-api)`
- 3 min: `Background mock bridge process killed between shell commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
