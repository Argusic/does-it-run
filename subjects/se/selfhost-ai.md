# selfhost-ai

**Verdict: could not verify.** Argusic Score 15 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kossakovsky/selfhost-ai, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/selfhost-ai

## Pinned environment

- Project commit: `d608f52fc90795eef57d2724411943d00cd2cbc1`
- Test commit: `d608f52fc90795eef57d2724411943d00cd2cbc1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 13.4 to 25.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 10 | 25 | 25.2 | 6 | 3 | [run](https://argusic.com/run/0d1a6eac-da5f-41d3-8536-172eb74f1586) |
| 2 | fail | 20 | 11 | 13.4 | 3 | 3 | [run](https://argusic.com/run/beec22b3-23b9-44c7-9cf8-4f6733862c0e) |

## What was observed on a clean machine

Attempt 1:

- `No Docker daemon available - dockerd requires root privileges, rootless failed with fork/exec /proc/self/exe: operation not permitted (user namespace restrictions)`
- `No sudo access - install scripts (01_system_preparation.sh, 02_install_docker.sh) require sudo`
- `Missing python-dotenv and PyYAML Python packages`
- `Missing docker compose CLI plugin`
- `Missing newuidmap/newgidmap binaries for rootless Docker`
- `rootless Docker still fails after uidmap install: rootlesskit cannot fork /proc/self/exe`

Attempt 2:

- 11 min: `Docker and Docker Compose not installed; no root access to install them; user namespaces disabled preventing rootless Docker`
- `apt-get not usable (no passwordless sudo); cannot install dependencies like uidmap, iptables`
- 2 min: `newuidmap binary from Ubuntu noble (libc 2.39) required an older version of the uidmap package than the one initially downloaded (which needed GLIBC 2.43)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
