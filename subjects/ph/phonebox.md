# phonebox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ersinkoc/phonebox, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/phonebox

## Pinned environment

- Project commit: `44ca501135de420bf6eff9f351a32c74496654b9`
- Test commit: `44ca501135de420bf6eff9f351a32c74496654b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.9 to 30.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 30.9 | 3 | 3 | [run](https://argusic.com/run/22407a7d-ae7c-48de-beb5-8d3c0ec82bb3) |
| 2 | pass | 100 | 10 | 5.9 | 1 | 1 | [run](https://argusic.com/run/ce562b67-b36c-45d8-b981-49db93e1e028) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No .NET SDK installed in container; dotnet command not found`
- 1 min: `2 ListeningPorts tests failed: IPv6 binding to ::1 fails in container (ipv6 disabled on loopback)`
- 3 min: `Node.js 18.19.1 too old for Playwright 1.65.0 (requires Node 20+)`

Attempt 2:

- 3 min: `IPv6 is disabled at the kernel level in this container but Socket.OSSupportsIPv6 returns true, causing two ListeningPorts tests (AnIpv6OnlyListenerIsReachedOnIpv6Loopback, BothFamiliesOnOnePortAreKept) to fail with SocketException: Cannot a`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
