# patent

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/r14dd/patent, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/patent

## Pinned environment

- Project commit: `15e563b45cbfa7cfb816f959a50e16fa9aaf73a7`
- Test commit: `15e563b45cbfa7cfb816f959a50e16fa9aaf73a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.5 to 16.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 10 | 16.4 | 3 | 2 | [run](https://argusic.com/run/774c3133-ac6a-488d-b6ea-4ade3d5f8009) |
| 2 | pass | 100 | 1.5 | 11.5 | 0 | 0 | [run](https://argusic.com/run/a2c9a49b-c927-4a2f-8b0d-b194bd3bf9b9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed in container`
- 1 min: `rustfmt and clippy components missing`
- 1 min: `live_pypi test fails: PyPI search bot-walled to non-browser clients (no keyless search API); app correctly surfaces this as sources_failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
