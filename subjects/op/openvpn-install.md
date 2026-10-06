# openvpn-install

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hwdsl2/openvpn-install, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/openvpn-install

## Pinned environment

- Project commit: `69faf877ecf6f73186fb7872f84695047f0d4f97`
- Test commit: `69faf877ecf6f73186fb7872f84695047f0d4f97`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 10.7 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 2.1 | 10.7 | 2 | 2 | [run](https://argusic.com/run/b33ed095-3014-4df0-aa38-9d2eca79f449) |
| 2 | fail | 20 | 0 | 14.2 | 4 | 4 | [run](https://argusic.com/run/cc11a3ea-a3be-49c8-b0ae-6cf1f2e4ccee) |

## What was observed on a clean machine

Attempt 1:

- 1.2 min: `Cannot run openvpn-install.sh install as non-root (no sudo, no root access in container). The script requires root for package installation (apt/dnf/yum), TUN device setup (/dev/net/tun missing + no mknod permission), systemd service manage`
- 0.3 min: `ShellCheck reports 8 info-level warnings (SC2086 unquoted $firewall, SC2162 read without -r, SC2001 sed over substitution). No errors.`

Attempt 2:

- 10 min: `Script requires root privileges (check_root exits if uid != 0)`
- 5 min: `Cannot install system packages (apt-get needs root)`
- 5 min: `/dev/net/tun does not exist , script's check_tun fails`
- 5 min: `No OpenVPN binary, no docker/podman for containerized tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
