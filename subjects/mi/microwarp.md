# MicroWARP

**Verdict: runs with mocks.** Argusic Score 46 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ccbkkb/MicroWARP, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/microwarp

## Pinned environment

- Project commit: `82a4c62042fb68030bb9e109d16bf8c17bd7e117`
- Test commit: `82a4c62042fb68030bb9e109d16bf8c17bd7e117`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 14 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 12 | 14 | 3 | 0 | [run](https://argusic.com/run/0d4854c3-9982-4b5a-9b28-3ab2eb977b71) |
| 2 | pass with mocks | 92 | 15 | 16.5 | 3 | 3 | [run](https://argusic.com/run/e02b59ee-bff1-4d5d-8236-73ee2a12975a) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Docker daemon cannot start (no root, user namespaces blocked by seccomp); cannot build the multi-stage Docker image inside the container`
- 2 min: `Linux networking tools (ip, wg, iptables, wg-quick) not available on host; cannot run real WireGuard tunnel`
- 2 min: `Usque (MASQUE client) fails to start with real configs because Cloudflare WARP registration requires real credentials`

Attempt 2:

- 8 min: `Docker daemon not available in container (no root, no rootlesskit support without slirp4netns)`
- 2 min: `WireGuard kernel module not loaded and mock wg-quick/ip used for kernel-level operations`
- 2 min: `Cannot mkdir /etc/wireguard (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
