# wireguard-install

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Nyr/wireguard-install, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/run/44a48c3c-e1d0-40db-9c84-fb7024078514

## Pinned environment

- Project commit: `775238b7f71bdb4f447179452e46eb4208a20b20`
- Test commit: `775238b7f71bdb4f447179452e46eb4208a20b20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.3 to 13.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 13.3 | 4 | 4 | [run](https://argusic.com/run/44a48c3c-e1d0-40db-9c84-fb7024078514) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No root privileges to install system wireguard-tools package; script requires EUID 0`
- 3 min: `No TUN device available in container, no kernel wireguard module`
- 3 min: `Cannot modify /etc/wireguard or /etc/sysctl.d without root`
- 1 min: `firewall-cmd not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
