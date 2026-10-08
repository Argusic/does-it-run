# windows

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dockur/windows, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/windows

## Pinned environment

- Project commit: `013ea27498e0e820a46b3861a0fa047d5b19d846`
- Test commit: `013ea27498e0e820a46b3861a0fa047d5b19d846`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 10.3 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 12.5 | 10.3 | 3 | 3 | [run](https://argusic.com/run/ca49c2c7-de5c-4708-9d49-63f22ac843fc) |
| 2 | fail | 50 | 0 | 13.1 | 3 | 3 | [run](https://argusic.com/run/75c916d3-09dc-4311-99c8-12609764ba9c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `compose.yml and codespaces.yml missing YAML document-start marker`
- 1 min: `hadolint 2.12.0 did not support Dockerfile --exclude COPY syntax`
- 0.5 min: `kubernetes.yml yamllint indentation warnings`

Attempt 2:

- `Docker daemon cannot start in this unprivileged container (unshare: Operation not permitted due to seccomp)`
- `Podman binary extracted but depends on libgpgme.so.11 not present in the environment`
- `/dev/kvm not available - cannot run QEMU with acceleration`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
