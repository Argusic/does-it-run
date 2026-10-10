# node-hue-api

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/peter-murray/node-hue-api, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/node-hue-api

## Pinned environment

- Project commit: `0318111a39aa144bc944b1b629a4e2259e9ff087`
- Test commit: `0318111a39aa144bc944b1b629a4e2259e9ff087`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 53.8 to 53.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 1 | 53.8 | 1 | 0 | [run](https://argusic.com/run/2cd46330-ff01-4f64-9bbd-3179ddf31044) |

## What was observed on a clean machine

Attempt 1:

- 35 min: `23 of 49 tests fail because they require a real Philips Hue bridge on the local network (UPnP/mDNS found none) or access to discovery.meethue.com, which returned HTTP 429 from this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
