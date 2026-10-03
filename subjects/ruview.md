# RuView

**Verdict: runs.** Argusic Score 94.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ruvnet/RuView, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ruview

## Pinned environment

- Project commit: `dd02efe2fe129ae8068e9b805ea35aaa660e47dd`
- Test commit: `dd02efe2fe129ae8068e9b805ea35aaa660e47dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.8 to 35.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 94.29 | 32 | 35.8 | 7 | 5 | [run](https://argusic.com/run/722c21f2-8b8c-48c3-bb88-09b6f0784aae) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No rustc/cargo installed on system`
- 2 min: `Git submodules not initialized (vendor/rufield etc missing)`
- 5 min: `Python modules numpy/scipy/pydantic missing`
- 1 min: `pytest args --cov from pyproject.toml cause unrecognized argument error`
- 1 min: `pytest-asyncio missing: async tests fail`
- `Rust workspace build fails on glib-sys system library dependency (sensing-server crate chain)`
- `wifi-densepose-signal and dependent crates hang during compilation (heavy nalgebra/simba dep)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
