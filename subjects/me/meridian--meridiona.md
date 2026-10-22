# meridian

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Meridiona/meridian, licensed NOASSERTION, written in Rust.

Evidence and recordings: https://argusic.com/run/d24c4fdc-d3ce-47ea-bcf0-c64cebc4c3fe

## Pinned environment

- Project commit: `a100468211b3f1f79c1d71ff01921d9cc47327bb`
- Test commit: `a100468211b3f1f79c1d71ff01921d9cc47327bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.4 to 34.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 34 | 34.4 | 2 | 1 | [run](https://argusic.com/run/d24c4fdc-d3ce-47ea-bcf0-c64cebc4c3fe) |

## What was observed on a clean machine

Attempt 1:

- `Flaky timing test 'a_failed_process_with_an_inconclusive_verify_reports_the_process_failure' fails under concurrent load (documented race condition in source, grace/poll_interval may need widening)`
- `Tauri tray crate (meridian-tray) requires GTK/WebKit dev headers (libgtk-3-dev libwebkit2gtk) not available on Linux without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
