# wireguard-docs

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pirate/wireguard-docs, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/wireguard-docs

## Pinned environment

- Project commit: `f87afb4f646d43054eaeca00384c1cbb06cc5d02`
- Test commit: `f87afb4f646d43054eaeca00384c1cbb06cc5d02`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 23.6 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 35 | 23.6 | 3 | 3 | [run](https://argusic.com/run/5978e6f1-2380-4ca4-927e-3523dd1a349b) |
| 2 | pass | 100 | 45 | 30.3 | 6 | 6 | [run](https://argusic.com/run/f2386d32-f400-40cb-bd94-8410b3188473) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `wg and wg-quick userspace tools not installed`
- 5 min: `ip command (iproute2) missing`
- 15 min: `Could not verify cross-namespace WireGuard tunnel encrypted traffic`

Attempt 2:

- 15 min: `No wg/wg-quick/ip binaries in container (non-root, no apt install possible)`
- 8 min: `example-lan-briding/vancouver key files stale: vancouver.key held the shared server1 private key 2P/3ll... and vancouver.key.pub held q/+jw... which did not match, while vancouver/wg0.conf and all peer references use WN+bvd.../8bSk5f...`
- 4 min: `wg-quick fails mid-start: resolvconf missing (DNS= lines)`
- 6 min: `wg-quick fails on laptop (AllowedIPs 0.0.0.0/0): ip6tables-restore and iptables-restore missing`
- 4 min: `example-lan-briding start.sh PostUp runs iptables, not installed in container`
- 8 min: `example-iptables/iptables.sh hardcodes /sbin/iptables which does not exist here; scripts has no install path and netfilter is unavailable in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
