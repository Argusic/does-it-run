# izwi

**Verdict: runs with mocks.** Argusic Score 52.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/izwi-ai/izwi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/izwi

## Pinned environment

- Project commit: `7804eee5a9445031a7668017502b9c24e6db4ba7`
- Test commit: `7804eee5a9445031a7668017502b9c24e6db4ba7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 27.6 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 27.6 | 0 | 0 | [run](https://argusic.com/run/b584e39e-95ff-49e2-af09-e4e948b1b16c) |
| 2 | pass with mocks | 85.33 | 10 | 30.3 | 3 | 2 | [run](https://argusic.com/run/6fbed49d-ccba-497a-ad14-aacacb2e1fd4) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not present`
- 2 min: `izwi-core test linker SIGSEGV (stack overflow)`
- `izwi-desktop (Tauri) build fails: glib-sys, gtk3, webkit2gtk system libraries missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
