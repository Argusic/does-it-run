# earthly

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/earthly/earthly, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/earthly

## Pinned environment

- Project commit: `6e641c15d3b4d7dd396363b61d2381faa2658f3d`
- Test commit: `6e641c15d3b4d7dd396363b61d2381faa2658f3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.7 to 83.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.3 | 2.7 | 0 | 0 | [run](https://argusic.com/run/acc10f3d-0c01-43db-84fe-f6d4daf17ffa) |
| 2 | pass | 92 | 13 | 83.5 | 5 | 3 | [run](https://argusic.com/run/2e816642-41d1-49f3-a9a9-e7239ccf1260) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `go: command not found in container`
- 4 min: `No docker/podman binary, so earthly's docker-shell frontend could not initialize`
- 2 min: `bootstrap/config warned 'could not construct new buildkit client ... failed to unmarshal container inspect output'`
- 25 min: `Real buildkit container cannot run: buildkitd requires root/user-namespace+mount privileges, but kernel seccomp blocks unshare, setuid, and mount(2) (Seccomp: 2, CapEff=0, no root, no docker/podman)`
- 35 min: `earthly build +target never reaches the build step: buildkit daemon cannot start in this sandbox (tried rootless buildkit, proot+containerd, patched source; containerd daemon boots under proot but image unpack needs mount(2))`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
