# mediabox

**Verdict: could not verify.** Argusic Score 10 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tom472/mediabox, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/mediabox

## Pinned environment

- Project commit: `4b411469fd6719c653761c03d60eb11facb222bc`
- Test commit: `4b411469fd6719c653761c03d60eb11facb222bc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 7.4 to 21.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 8 | 7.4 | 3 | 0 | [run](https://argusic.com/run/fba30d00-c9b8-482f-9267-a53cdd4c5d1a) |
| 2 | fail | 20 | 21 | 21.2 | 3 | 3 | [run](https://argusic.com/run/320c6263-2460-4ffa-b143-4566f6f0d96d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Docker is not installed and cannot be installed (no root/sudo in this container; apt and dpkg available but require root)`
- 4 min: `Rootless Docker setup failed , unshare fails (kernel has unprivileged_userns_clone=1 but user namespaces are blocked at the seccomp/capability level; dockerd requires root)`
- 1 min: `containerd requires /run/containerd (root-owned); no alternative workaround available without root`

Attempt 2:

- 10 min: `Docker daemon not available in the test container (no /var/run/docker.sock, no root access)`
- 6 min: `User namespace cloning blocked by seccomp (clone() operation not permitted)`
- 3 min: `mediabox.sh stopped at docker compose up because no Docker daemon is reachable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
