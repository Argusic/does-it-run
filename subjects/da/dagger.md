# dagger

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dagger/dagger, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/dagger

## Pinned environment

- Project commit: `e8f071cc2ab0a4ee1c8cc7ec9a72830b0cdaab6f`
- Test commit: `e8f071cc2ab0a4ee1c8cc7ec9a72830b0cdaab6f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 21.9 to 23.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 13 | 23.7 | 3 | 3 | [run](https://argusic.com/run/2b940875-7783-4c83-b412-3afee0bf104b) |
| 2 | fail | 50 | 3 | 21.9 | 2 | 2 | [run](https://argusic.com/run/4c5c48d6-3317-491b-a7cc-fbab4cb42522) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No container runtime available (Docker, containerd) , Dagger engine requires one to start`
- 4 min: `containerd cannot create /run/containerd (permission denied), and rootlesskit cannot fork user namespace (fork/exec /proc/self/exe: operation not permitted, Seccomp:2, AppArmor: enforce)`
- 1 min: `typescript codegen tests (cmd/codegen/generator/typescript/templates) panic during init: cannot download release checksums from dl.dagger.io (403 Forbidden)`

Attempt 2:

- 15 min: `No container runtime (Docker, Podman, containerd) available. The Dagger engine requires a container runtime to start the local engine.`
- 3 min: `Engine binary built from source panics during shutdown: 'cannot create context from nil parent' in dagger/otel-go Close()`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
