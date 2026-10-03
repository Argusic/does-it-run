# wireguard-install

**Verdict: could not verify.** Argusic Score 47.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/angristan/wireguard-install, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/wireguard-install

## Pinned environment

- Project commit: `832fb9833501a7220e2900cffb61082841dedba8`
- Test commits: `832fb9833501a7220e2900cffb61082841dedba8`, `775238b7f71bdb4f447179452e46eb4208a20b20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 4.2 to 13.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 0 | 4.2 | 1 | 0 | [run](https://argusic.com/run/99514207-b667-46f1-b87d-cf0db2a3d844) |
| 1 | pass with mocks | 92 | 12 | 13.3 | 4 | 4 | [run](https://argusic.com/run/44a48c3c-e1d0-40db-9c84-fb7024078514) |
| 2 | fail | 20 | 4.6 | 5 | 3 | 3 | [run](https://argusic.com/run/c120d7c3-f075-407d-8902-f0ddd6072721) |

## What was observed on a clean machine

Attempt 1:

- `Cannot run script directly: requires root, wireguard kernel module, and systemd, none of which are available in container`

Attempt 1:

- 2 min: `No root privileges to install system wireguard-tools package; script requires EUID 0`
- 3 min: `No TUN device available in container, no kernel wireguard module`
- 3 min: `Cannot modify /etc/wireguard or /etc/sysctl.d without root`
- 1 min: `firewall-cmd not installed in container`

Attempt 2:

- `Script requires root, no sudo available in container`
- `WireGuard kernel module not loaded/built-in`
- `WireGuard tools (wg, wg-quick, qrencode, iptables) not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
