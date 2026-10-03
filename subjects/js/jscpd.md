# jscpd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kucherenko/jscpd, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/jscpd

## Pinned environment

- Project commit: `379057697f7176b75fda3c2bdab03e400f23f510`
- Test commit: `379057697f7176b75fda3c2bdab03e400f23f510`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 8.9 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/2fab8162-bf11-4f09-8d26-0e98559b6520) |
| 2 | pass | 100 | 2.5 | 20.1 | 1 | 1 | [run](https://argusic.com/run/213d33ac-5e3a-4b26-abba-0c624ad4a8cc) |
| 3 | pass | 100 | 1 | 8.9 | 0 | 0 | [run](https://argusic.com/run/2b775cf9-6a85-44ee-9937-643729da51bf) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Rust source build fails: no C compiler (gcc/cc) or system linker available in container; cannot install build-essential without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
