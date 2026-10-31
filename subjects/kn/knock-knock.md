# knock-knock

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/djkurlander/knock-knock, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/knock-knock

## Pinned environment

- Project commit: `da33d6ae4a601ee5a5b926d5ac6800be82c4cd6e`
- Test commit: `da33d6ae4a601ee5a5b926d5ac6800be82c4cd6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.3 to 19.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 62 | 19.3 | 5 | 5 | [run](https://argusic.com/run/6cba2592-a85a-4248-bf67-436ef1f68eb6) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `RDP honeypot hard-coded c_listen 3389 so ENABLED_PROTOCOLS=RDP:<port> was ignored and the spawned honeypot died (port refused)`
- 6 min: `SSH honeypot ignored --port (only read SSH_PORT), so it never bound the ENABLED_PROTOCOLS port`
- 10 min: `GeoIP database paths hard-coded to /usr/share/GeoIP, which is root-owned and unpopulated in this non-root container; monitor blocked waiting forever`
- 3 min: `stats.py hard-coded data/knock_knock.db and crashed with 'no such table: country_intel' when DB_DIR pointed elsewhere`
- 2 min: `monitor.py failed with redis ConnectionError Errno 99 connecting to localhost:6379 (IPv6-first) when only IPv4 was bound`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
