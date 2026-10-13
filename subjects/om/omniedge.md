# omniedge

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/omniedgeio/omniedge, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/omniedge

## Pinned environment

- Project commit: `aac202655a372b6f0ccd189172fcbc1b7780cede`
- Test commit: `aac202655a372b6f0ccd189172fcbc1b7780cede`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.3 to 19.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 19.5 | 0 | 0 | [run](https://argusic.com/run/a8746147-c90b-4295-a33b-b007dc6266e3) |
| 2 | pass | 100 | 7 | 9.3 | 2 | 2 | [run](https://argusic.com/run/b0c54625-5beb-40ad-865c-0b5f9c7c18e6) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Rust toolchain (rustc, cargo) not found in container`
- `Desktop/Tauri crate (ui/desktop/src-tauri) failed to build: missing glib-2.0 system library`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
