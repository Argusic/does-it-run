# run-on-arch-action

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/uraimo/run-on-arch-action, licensed BSD-3-Clause, written in Shell.

Evidence and recordings: https://argusic.com/subject/run-on-arch-action

## Pinned environment

- Project commit: `fa1f3e7de95534497266c7265950b5188355fbfb`
- Test commit: `fa1f3e7de95534497266c7265950b5188355fbfb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 5.2 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 5.2 | 3 | 3 | [run](https://argusic.com/run/14551b4a-3f9e-4b6a-b03b-1144f723a426) |
| 2 | pass with mocks | 92 | 1 | 9.3 | 3 | 3 | [run](https://argusic.com/run/ceebfd79-a35e-40b4-8a7d-f877838e222f) |

## What was observed on a clean machine

Attempt 1:

- 14 min: `No docker/podman/root/binfmt in the container, so real QEMU container execution was impossible; no in-repo test suite exists.`
- 3 min: `run-on-arch.sh failed with 'sudo: command not found' because this container has no root/sudo for its apt step.`
- 1 min: `First action run failed on 'env nested value must be flat', which is the action's intended validation, not a bug.`

Attempt 2:

- 15 min: `Docker daemon not available - no /var/run/docker.sock, no root for dockerd, no rootlesskit/slirp4netns for rootless mode`
- 5 min: `declare -a DOCKER_RUN_ARGS=${@:3:${#@}} in src/run-on-arch.sh collapses multiple args into one string instead of preserving array elements`
- 1 min: `@actions/core package locked at v1.1.1 but package.json requires ^1.9.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
