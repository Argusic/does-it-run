# f3d

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/f3d-app/f3d, licensed BSD-3-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/f3d

## Pinned environment

- Project commit: `c07c07aa9fcdb8506e8c3ea316302538c097f08f`
- Test commit: `c07c07aa9fcdb8506e8c3ea316302538c097f08f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 26.9 to 36.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 26.9 | 0 | 0 | [run](https://argusic.com/run/ee378dd2-a89f-4bc7-bd9a-ac28c7b82411) |
| 2 | pass | 100 | 36 | 36.1 | 3 | 3 | [run](https://argusic.com/run/32335a49-159e-4a4b-80f3-d9493bcd34b3) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Missing VTK 9.4+ C++ dev libraries for source build (system has vtk9.1 packages, req 9.4)`
- 3 min: `Missing GL/X11/Wayland development headers for VTK source compilation`
- 30 min: `VTK source build (v9.7.1) still compiling after 36+ minutes - too large to complete in this environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
