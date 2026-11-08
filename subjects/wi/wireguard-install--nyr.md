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
- Valid runs: 2; wall time 13.3 to 22.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 13.3 | 4 | 4 | [run](https://argusic.com/run/44a48c3c-e1d0-40db-9c84-fb7024078514) |
| 2 | pass with mocks | 92 | 25 | 22.6 | 5 | 5 | [run](https://argusic.com/run/9e4ec3e9-3404-49ee-a759-126628e8ca48) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No root privileges to install system wireguard-tools package; script requires EUID 0`
- 3 min: `No TUN device available in container, no kernel wireguard module`
- 3 min: `Cannot modify /etc/wireguard or /etc/sysctl.d without root`
- 1 min: `firewall-cmd not installed in container`

Attempt 2:

- 10 min: `Installer requires root (EUID=0); container user uid=1001 has no capabilities, no sudo, no user namespaces, and apt-get cannot acquire dpkg lock`
- 3 min: `No /dev/net/tun and no wireguard kernel module; systemd-detect-virt reports container so script wants BoringTun + TUN device`
- 1 min: `PATH lacked sbin so script aborted`
- 3 min: `Mock ip returned private address so script demanded public-IP lookup via failing network mocks`
- 8 min: `grep/sed/chmod/bash file tests could not see remapped files (missing stat/openat/fopen interpositions; chmod uses raw fchmodat2 syscall)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
