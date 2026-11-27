# wireguard-install

**Verdict: runs with mocks.** Argusic Score 46 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hwdsl2/wireguard-install, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/run/169c1b17-1ac8-499b-9ac0-3b46f7cadec9

## Pinned environment

- Project commit: `3f428774e61c95bca60d1e7b80f0c768ca2c6137`
- Test commit: `3f428774e61c95bca60d1e7b80f0c768ca2c6137`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 3.8 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 0 | 3.8 | 3 | 0 | [run](https://argusic.com/run/169c1b17-1ac8-499b-9ac0-3b46f7cadec9) |
| 2 | pass with mocks | 92 | 8 | 4.3 | 5 | 5 | [run](https://argusic.com/run/f16660b0-92bb-4617-ab91-8d980fc43174) |

## What was observed on a clean machine

Attempt 1:

- `Cannot run as root - no sudo or root access in container. The script requires root for apt-get install and WireGuard kernel module access.`
- `WireGuard kernel module not available - container lacks kernel support for WireGuard (no module, no NET_ADMIN capability).`
- `Script refuses to run inside containers (systemd-detect-virt -cq returns 0), which is by design.`

Attempt 2:

- 2 min: `Script check_root requires uid 0`
- 1 min: `ip command not found , script overrides PATH in wgsetup()`
- 1 min: `apt-get install fails without root`
- 1 min: `/etc/ sysctl/firewall/rc.local unwritable without root`
- 1 min: `wget/curl reach out to real services for public IP`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
