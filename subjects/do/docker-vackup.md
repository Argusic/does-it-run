# docker-vackup

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BretFisher/docker-vackup, licensed Unlicense, written in Shell.

Evidence and recordings: https://argusic.com/subject/docker-vackup

## Pinned environment

- Project commit: `6b8a06f6cb4f9837eeba2beb17d04ae998617151`
- Test commit: `6b8a06f6cb4f9837eeba2beb17d04ae998617151`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 24.7 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 25 | 30.3 | 4 | 4 | [run](https://argusic.com/run/77ff715c-baff-4ef8-84a9-f00dc627050a) |
| 2 | pass with mocks | 92 | 18 | 24.7 | 2 | 2 | [run](https://argusic.com/run/8ed81024-a55d-486e-82c8-9db81c554153) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Docker CLI not installed or available in container environment`
- 10 min: `Cannot start dockerd: container lacks CAP_SYS_ADMIN and user namespace support (no newuidmap/newgidmap)`
- 8 min: `Started containerd v1.7.24 with patched paths but image pulling failed: overlay mount requires CAP_SYS_ADMIN`
- 2 min: `11 of 14 bats tests require Docker daemon for volume/container operations and fail with docker: command not found`

Attempt 2:

- 12 min: `Docker CLI not available in container`
- 1 min: `bats test framework not installed system-wide (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
