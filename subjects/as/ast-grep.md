# ast-grep

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ast-grep/ast-grep, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ast-grep

## Pinned environment

- Project commit: `29285d16757371a70a93190929940886e68618d3`
- Test commit: `29285d16757371a70a93190929940886e68618d3`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5.6 to 31.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 31.7 | 3 | 3 | [run](https://argusic.com/run/6686616e-ed69-4bdf-a35a-f7dda43daf99) |
| 2 | pass | 100 | 2.5 | 5.6 | 0 | 0 | [run](https://argusic.com/run/ec533b51-3d76-42b0-8359-d8b036c5f6c8) |
| 3 | pass | 100 | 6 | 9 | 0 | 0 | [run](https://argusic.com/run/211dbe0b-9b1c-42ee-994b-2e1e76f72bf1) |

## What was observed on a clean machine

Attempt 1:

- 9 min: `No Rust toolchain installed`
- 18 min: `No C compiler (cc) found on system`
- 2 min: `ar (archiver) not found by cc crate`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
