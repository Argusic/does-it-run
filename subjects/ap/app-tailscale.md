# app-tailscale

**Verdict: could not verify.** Argusic Score 10 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hassio-addons/app-tailscale, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/app-tailscale

## Pinned environment

- Project commit: `2f295975bcd52e0ffaf722ae43bae34bf7b8633f`
- Test commit: `2f295975bcd52e0ffaf722ae43bae34bf7b8633f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.5 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 5.2 | 5.5 | 1 | 0 | [run](https://argusic.com/run/22b891cb-2428-44eb-bf59-f9f55716b6ad) |
| 2 | fail | 20 | 7.2 | 9.1 | 2 | 2 | [run](https://argusic.com/run/b1b9b1ad-39b8-4b18-aa07-9b2b046df9a9) |

## What was observed on a clean machine

Attempt 1:

- 5.2 min: `Docker is not installed in this container. The project is a Home Assistant Docker addon and requires 'docker build' to produce an image. Without Docker, the addon cannot be assembled or launched.`

Attempt 2:

- 5 min: `Docker daemon unavailable (user namespaces disabled, no root)`
- 2 min: `Cannot build Docker image without running Docker daemon`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
