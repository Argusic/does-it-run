# xplr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sayanarijit/xplr, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/xplr

## Pinned environment

- Project commit: `d96991f6b1d1ff9914716ebc1150cbb4a406abca`
- Test commit: `d96991f6b1d1ff9914716ebc1150cbb4a406abca`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 4.5 to 51.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 51.4 | 0 | 0 | [run](https://argusic.com/run/65192912-d2e3-4ee0-a6c7-1f6ea9a337a4) |
| 2 | pass | 100 | 33.5 | 34.1 | 5 | 5 | [run](https://argusic.com/run/addc1477-dd92-4fb4-837b-0b7524da5fab) |
| 3 | pass | 100 | 3 | 4.5 | 0 | 0 | [run](https://argusic.com/run/13f82cba-b0dc-4cda-b127-c669267caa07) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `No Rust toolchain installed`
- 20 min: `No C compiler or linker available`
- 2 min: `No make command available`
- 3 min: `Missing shared libraries (libisl, libmpc, libmpfr) for gcc-14 cc1`
- 3 min: `Linker ld couldn't find libbfd-2.47-system.so, libctf.so.0, libsframe.so.3`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
