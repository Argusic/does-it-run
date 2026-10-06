# rclone

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rclone/rclone, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/rclone

## Pinned environment

- Project commit: `7ebef790b49add3d0610cea1a4b3d0ff270c383b`
- Test commit: `7ebef790b49add3d0610cea1a4b3d0ff270c383b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.1 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 19.1 | 5 | 5 | [run](https://argusic.com/run/5a76970b-a781-40a2-8614-d2783b799209) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No Go toolchain installed; repo requires go 1.26.0`
- 3 min: `Unit tests failed: TestLogger needed rsync (exec: rsync: not found)`
- 3 min: `Mount/docker tests needed FUSE (fusermount3 not found; fuse device absent)`
- 4 min: `cmd/serve/nfs TestCache/symlink failed: name_to_handle_at returns EOPNOTSUPP on overlayfs`
- 1 min: `serve http and rcd background servers were reaped between exec calls; first attempt transiently showed 000`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
