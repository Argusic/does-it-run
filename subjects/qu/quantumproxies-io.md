# quantumproxies.io

**Verdict: runs with mocks.** Argusic Score 51 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/quantumproxies/quantumproxies.io, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/quantumproxies-io

## Pinned environment

- Project commit: `7ff29f7b8a1efe12f8e55aa80ea733253c1717c4`
- Test commit: `7ff29f7b8a1efe12f8e55aa80ea733253c1717c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 5 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.4 | 0 | 0 | [run](https://argusic.com/run/55275a0b-bca4-43fc-9a57-f8768ea85766) |
| 2 | pass with mocks | 82 | 1 | 5 | 4 | 2 | [run](https://argusic.com/run/a01ff67b-5103-4d8d-a331-7b5be26de06d) |

## What was observed on a clean machine

Attempt 2:

- `SOCKS5 mock not implemented , curl via socks5h:// failed (empty response)`
- 2 min: `undici v8 requires Node 22+, pinned to v7.1.0 for Node 18`
- 1 min: `pip install blocked by externally-managed-environment, used --break-system-packages`
- `PHP, Go, Ruby, Java, C# runtimes unavailable , examples not executed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
