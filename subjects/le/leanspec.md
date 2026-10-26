# leanspec

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/codervisor/leanspec, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/leanspec

## Pinned environment

- Project commit: `ee122d6fe4bdf3c22f2507e2944f5a213ddcf7a6`
- Test commit: `ee122d6fe4bdf3c22f2507e2944f5a213ddcf7a6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28 to 28 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 28 | 1 | 1 | [run](https://argusic.com/run/a29107fb-9cdb-41a5-a7ef-b73986429c7c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `ts-rs proc-macro #[ts(export, export_to = ...)] paths in leanspec-http/src/types/specs.rs and common.rs used ../../../../ from the crate root, which resolves above the filesystem root and causes EACCES PermissionDenied`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
