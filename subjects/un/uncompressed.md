# uncompressed

**Verdict: could not verify.** Argusic Score 0 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Lackoftactics/uncompressed, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/uncompressed

## Pinned environment

- Project commit: `18c81597f25b7678313695bfd9d4df33764efd2d`
- Test commit: `18c81597f25b7678313695bfd9d4df33764efd2d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.5 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 0 | 8.1 | 1 | 0 | [run](https://argusic.com/run/bb16d87c-d62a-4316-9963-f60d68456a65) |
| 2 | fail | 0 | 5 | 5.5 | 1 | 0 | [run](https://argusic.com/run/1076c70b-9fd9-4bbc-ba88-9f95cbf70815) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Docker daemon cannot start in this container: no root access, seccomp level 2 blocks fork/exec for RootlessKit, unshare -U denied, no /var/run/docker.sock present`

Attempt 2:

- 5 min: `Docker is not installed and cannot be installed in this container environment (no root access, no user namespaces, no Docker socket available). The project is a Docker Compose infrastructure - both compose files require Docker to run.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
