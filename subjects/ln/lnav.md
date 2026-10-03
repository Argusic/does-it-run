# lnav

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tstack/lnav, licensed BSD-2-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/lnav

## Pinned environment

- Project commit: `e43baf0c202cb328c75a16947097b011a5279a11`
- Test commit: `e43baf0c202cb328c75a16947097b011a5279a11`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 4; wall time 39.3 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/6c3eeb53-2d03-47c6-9283-44d826bfad5b) |
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/8e759610-dba7-4ff0-acc8-f8e8d6ba2350) |
| 2 | pass | 100 | 38 | 39.3 | 4 | 4 | [run](https://argusic.com/run/78cf21ff-d96f-4aa2-89b7-02156a31d478) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/2d694562-51e2-4d1f-ae92-367a2b15c143) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `No C++ compiler or build tools installed in container`
- 10 min: `autotools configure needed patched paths for non-standard tool locations`
- 8 min: `zig libc++ headers conflict with glibc system headers when -I is used`
- 5 min: `Full source build didn't complete within time budget`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
