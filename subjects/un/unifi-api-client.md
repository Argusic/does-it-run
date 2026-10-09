# UniFi-API-client

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Art-of-WiFi/UniFi-API-client, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/unifi-api-client

## Pinned environment

- Project commit: `ce7e6c84a05813ca52a03d5c6e6bac5e039d5b8f`
- Test commit: `ce7e6c84a05813ca52a03d5c6e6bac5e039d5b8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25 to 25 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 25 | 2 | 2 | [run](https://argusic.com/run/8c6c0245-549e-482d-97a9-a211f5b70c7d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP not pre-installed in container (no root for apt-get)`
- 5 min: `Static PHP's curl could not connect to localhost (musl libc issue)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
