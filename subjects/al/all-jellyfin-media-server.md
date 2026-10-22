# All-jellyfin-media-server

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Morzomb/All-jellyfin-media-server, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/all-jellyfin-media-server

## Pinned environment

- Project commit: `d0e84b8f7950048466ddfddc878f3566951697df`
- Test commit: `d0e84b8f7950048466ddfddc878f3566951697df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 9.9 to 54.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 49 | 54.4 | 7 | 7 | [run](https://argusic.com/run/191447a0-8455-43af-933f-f94935a83457) |
| 2 | fail | 20 | 30 | 9.9 | 4 | 4 | [run](https://argusic.com/run/8bdaa7ee-9ed7-4576-a042-bbe6d48fd91f) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `No Docker daemon in environment and unprivileged namespace syscalls are seccomp-blocked, so the repo's documented docker compose deployment could not run.`
- 8 min: `setup.sh ends its piped (non-tty) run with /bin/sh: 1: Bad substitution after printing ISYRR INSTALLATION COMPLETE.`
- 6 min: `FlareSolverr bundled Chromium failed to start: libwayland-server.so.0 not found.`
- 8 min: `Jellyseerr source build failed: pnpm missing and Node 18 below engines.node ^22.19.0.`
- 12 min: `Fresh Jellyfin 12.2 rejects X-Emby-Authorization/X-Emby-Token legacy headers (401) because EnableLegacyAuthorization is false and API keys lack xattr lookups.`
- 5 min: `qBittorrent nox first run requires --confirm-legal-notice and prints a temporary password; guessed defaults return 401.`
- 7 min: `Prowlarr indexer definition cache starts empty, so adding any Cardigann indexer fails with non-null fileKey (a known first-run crawl gap).`

Attempt 2:

- 15 min: `No Docker daemon available in this unprivileged container`
- 2 min: `Cannot install system packages via apt (not root)`
- 8 min: `containerd v2.4.2 starts but cannot mount overlayfs layers (mount syscall blocked)`
- 2 min: `no Docker socket found anywhere on filesystem`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
