# MeshLAN

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhaoxuya520/MeshLAN, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/meshlan

## Pinned environment

- Project commit: `591f5f5593ef5228eeb70003f10d63503ed37183`
- Test commit: `591f5f5593ef5228eeb70003f10d63503ed37183`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.8 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 7.8 | 0 | 0 | [run](https://argusic.com/run/707daec2-33f4-4ff3-ad5e-e6002093898b) |
| 2 | pass | 100 | 3 | 18.6 | 4 | 4 | [run](https://argusic.com/run/274b6b5a-9adb-4fc4-876c-2ed149d9e744) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `go: not found in container`
- 1 min: `nebula/nebula-cert 1.11.x missing`
- 1 min: `Nebula child cannot open TUN: /dev/net/tun missing, no root`
- 3 min: `printed MLNODE1 code secret does not match node-state secretHash; node agent returned 401 until I recovered the matching secret by recomputing the state hash`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
