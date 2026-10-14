# isahc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sagebind/isahc, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/isahc

## Pinned environment

- Project commit: `e373ae3ae5b8e53aecf22280edd35a29d91713b5`
- Test commit: `e373ae3ae5b8e53aecf22280edd35a29d91713b5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 6.8 | 1 | 1 | [run](https://argusic.com/run/eb736fbd-6526-4a3a-9b70-e37f9af72541) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Net test failures (ipv4_only_will_not_connect_to_ipv6, any_ip_version_uses_ipv4_or_ipv6) because the container's IPv6 stack resolves localhost to ::1 but cannot bind IPv6 sockets`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
