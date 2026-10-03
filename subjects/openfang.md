# openfang

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RightNow-AI/openfang, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/openfang

## Pinned environment

- Project commit: `acf2587e46be174c10200489c9a2d23a39a98aeb`
- Test commit: `acf2587e46be174c10200489c9a2d23a39a98aeb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.7 to 22.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 22.7 | 2 | 2 | [run](https://argusic.com/run/d3be87d2-102e-4f72-aaac-4bd3b7bdc201) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `OPENROUTER_API_KEY env var set in container pollutes kernel boot, causing 2 test failures`
- 3 min: `openfang-desktop crate fails to build - missing GTK/WebKit -dev libraries on system (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
