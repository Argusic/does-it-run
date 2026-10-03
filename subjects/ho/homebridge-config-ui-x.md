# homebridge-config-ui-x

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/homebridge/homebridge-config-ui-x, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/homebridge-config-ui-x

## Pinned environment

- Project commit: `bb94ef61d69fac7fe4c412e59397964f22eb6a2a`
- Test commit: `bb94ef61d69fac7fe4c412e59397964f22eb6a2a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 10.1 | 2 | 2 | [run](https://argusic.com/run/ab000f6a-999f-45bd-9b2d-acebd9543c84) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node.js v18.19.1 is too old for Angular CLI (needs >=22.22.3)`
- 1 min: `Prebuilt binary for @homebridge/node-pty-prebuilt-multiarch not available for node-v109-linux-x64, falling back to source build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
