# xh

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ducaale/xh, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/xh

## Pinned environment

- Project commit: `3255393e10e5d2ed4c49eb036c0c7679d4653796`
- Test commit: `3255393e10e5d2ed4c49eb036c0c7679d4653796`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 31 | 2 | 2 | [run](https://argusic.com/run/4761dbf0-d465-488c-a198-18267f240447) |
| 2 | pass | 100 | 8 | 5.3 | 0 | 0 | [run](https://argusic.com/run/f4d5b454-44dd-4f27-b2f7-33f5ab8a6ba8) |
| 3 | pass | 100 | 13 | 5 | 1 | 1 | [run](https://argusic.com/run/de48f803-1b23-4269-b72e-f3347cca7793) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No C compiler (gcc/cc) available in container`
- 3 min: `No pkg-config available`

Attempt 3:

- 7 min: `no Rust toolchain installed (cargo/rustc missing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
