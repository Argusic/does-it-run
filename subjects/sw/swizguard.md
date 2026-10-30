# SwizGuard

**Verdict: could not verify.** Argusic Score 6.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JakeSwiz/SwizGuard, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/swizguard

## Pinned environment

- Project commit: `39ff1af1f9e0f4534316f99c64c7ccc969e19819`
- Test commit: `39ff1af1f9e0f4534316f99c64c7ccc969e19819`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 5 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 13.33 | 11 | 12.3 | 3 | 2 | [run](https://argusic.com/run/b208585f-9c66-4d35-8cfe-f3a379b0b34d) |
| 2 | fail | 0 | 15 | 5 | 3 | 0 | [run](https://argusic.com/run/0be10712-ceb8-4009-ab38-7367152a9a2f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Standard install './swizguard setup' requires root ('sudo') which is not available in this container (runs as non-root user 'runner' with no sudo). Setup also needs apt to install wireguard/qrencode/iptables which cannot be installed withou`
- 3 min: `'regen-client-configs.sh' last line '[ -f "$CLIENT_DIR/private.key" ] && chmod 600' exits 1 under 'set -euo pipefail' and stops config generation when 'private.key' is missing, because a failed compound 'A && B' at the end of a script trigg`
- 5 min: `Generated 'singbox-client.json' used legacy DNS server format ('"address": "..."') which sing-box 1.14.0 removed; 'sing-box check' failed with "legacy DNS server formats are deprecated ... and removed in sing-box 1.14.0". Also the deprecate`

Attempt 2:

- `No root access , cannot install required system dependencies (wireguard, qrencode, unzip, iptables) or run server setup`
- `Cannot download/install Xray-core binary without root`
- `No test suite exists , project is a collection of bash scripts with zero automated tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
