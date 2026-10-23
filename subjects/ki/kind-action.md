# kind-action

**Verdict: runs with mocks.** Argusic Score 76 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/helm/kind-action, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/kind-action

## Pinned environment

- Project commit: `27e253499b3053ff287c0fd79a7af0c41008c690`
- Test commit: `27e253499b3053ff287c0fd79a7af0c41008c690`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 1.5 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 18 | 19.1 | 1 | 1 | [run](https://argusic.com/run/a4a7eb12-601a-43be-bcd7-f275c1eccfe7) |
| 2 | pass with mocks | 72 | 2 | 1.5 | 2 | 0 | [run](https://argusic.com/run/78a4cb39-a074-43ab-9641-564782eb9003) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `Docker is not available in this container: no docker.sock, no dockerd binary runs (requires root), rootless mode blocked (unshare syscall not permitted). Kind requires Docker to create Kubernetes clusters; without it, cluster creation fails`

Attempt 2:

- 2 min: `docker not found in container , cluster creation, registry setup, and cleanup with Docker calls all fail`
- `GitHub Actions env vars (RUNNER_TOOL_CACHE, GITHUB_PATH, GITHUB_OUTPUT) unset in non-Actions shell; had to export manually`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
