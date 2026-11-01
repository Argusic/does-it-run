# moby

**Verdict: runs.** Argusic Score 80.4 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moby/moby, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/moby

## Pinned environment

- Project commit: `c7b76b939576290b5daa5b3671fff06fcaeb6d2e`
- Test commit: `c7b76b939576290b5daa5b3671fff06fcaeb6d2e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 65.8 to 76.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 75 | 76.4 | 8 | 0 | [run](https://argusic.com/run/120021f2-c069-467b-b541-33c96c79dfd3) |
| 2 | pass with mocks | 80.89 | 20 | 65.8 | 9 | 4 | [run](https://argusic.com/run/0ead9e29-cbed-4be0-b80a-c086f9904b30) |

## What was observed on a clean machine

Attempt 1:

- `cmd/docker-proxy: 4 SCTP tests fail - protocol not supported in this container`
- `daemon/config: config merge/validation tests fail due to environment config differences`
- `daemon/graphdriver/vfs: tests require mount capability not available in unprivileged container`
- `daemon/graphdriver/windows: Windows-only platform tests incompatible with Linux`
- `daemon/volume/safepath: tests require mount capability not available in unprivileged container`
- `daemon/libnetwork/netutils: tests require netns capability not available in unprivileged container`
- `daemon/libnetwork/portallocator: tests require iptables/root not available in unprivileged container`
- `daemon/command: fails to compile due to missing libsystemd.pc systemd header`

Attempt 2:

- 6 min: `Go toolchain not installed`
- 5 min: `Missing libsystemd/libseccomp/libnftables dev headers and libs (unit suite builds with -tags journald)`
- 2 min: `docker-proxy not on PATH and /usr/local/bin not writable`
- 4 min: `systemd-journal-remote missing so journald fake-sender tests skipped/failed`
- 3 min: `IPv6 unavailable in container (::1 cannot bind); 5 cmd/docker-proxy IPv6 tests fail`
- 3 min: `No CAP_NET_ADMIN and cannot create net namespaces; daemon TestIfaceAddrs times out and panics the package`
- 2 min: `Mount and chown blocked (no CAP_SYS_ADMIN); safepath bind-mount and vfs chown tests fail`
- 1 min: `Cannot create dockremap user without root; userns-remap test fails on RemappedRoot default`
- 2 min: `Unprivileged user namespaces disabled (apparmor_restrict_unprivileged_userns=1), no root; rootlesskit and rootless dockerd cannot start, so no live Docker API socket`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
