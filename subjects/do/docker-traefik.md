# Docker-Traefik

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SimpleHomelab/Docker-Traefik, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/docker-traefik

## Pinned environment

- Project commit: `5ab37c2f11b7b67dbd6b5c199b1e243748d47f02`
- Test commit: `5ab37c2f11b7b67dbd6b5c199b1e243748d47f02`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 3; wall time 11.1 to 20.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 15 | 20.5 | 4 | 4 | [run](https://argusic.com/run/8add51e4-59bb-4be9-86e4-aa71b403aadd) |
| 2 | fail | 50 | 8 | 12.8 | 3 | 3 | [run](https://argusic.com/run/b199dfa9-95fc-4fbf-acdc-4b6034529f31) |
| 3 | fail | 50 | 12 | 11.1 | 3 | 3 | [run](https://argusic.com/run/c998e99c-24df-443e-8a8f-72b211f6823f) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Docker Engine not installed in container`
- 2 min: `ds918 compose files referenced undefined network 'traefik_proxy'`
- 2 min: `Missing environment variables required by compose includes`
- 1 min: `ws-arm flowise.yml has ports mapping ${FLOWISE_PORT}:${FLOWISE_PORT} which becomes ':' when unset; also depends_on postgresql/redis not in default profile`

Attempt 2:

- 6 min: `Docker daemon cannot start inside this container: rootless Docker requires CLONE_NEWNS/CAP_SYS_ADMIN capabilities (seccomp enforce + no unshare) and newuidmap/newgidmap binaries were extracted but dockerd fork still fails with 'operation no`
- 2 min: `DS918 compose files reference network 'traefik_proxy' but traefik.yml defines it as 't2_proxy' , 10 service files affected (oauth, plex, portainer, tdarr, syncthing, rclone-gdrive, rclone-gcrypt, glances, qdirstat, vscode)`
- `Archive compose files use undefined YAML aliases (common-keys-core, common-keys-apps, common-keys-media, common-keys-monitoring, default-tz-puid-pgid) that were presumably provided by Deployrr's template system; 28 archive files affected`

Attempt 3:

- 8 min: `Docker daemon unavailable - no root access and user namespace creation disabled`
- 2 min: `9 YAML files had invalid Go template syntax inside double-quoted strings (e.g. customFrameOptionsValue: "allow-from https:{{env "DOMAIN.."}}") which broke YAML parsing`
- 1 min: `docker-compose-ds918.yml defined t2_proxy network but included services referenced traefik_proxy`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
