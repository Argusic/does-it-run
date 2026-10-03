# openinterpreter

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openinterpreter/openinterpreter, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/openinterpreter

## Pinned environment

- Project commit: `5b07159c477920c159d8892d112b480e7307f257`
- Test commit: `5b07159c477920c159d8892d112b480e7307f257`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 42 to 71.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/44792fd6-2652-4b44-bfd5-8ad0863b7b4e) |
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/03fc97ab-0379-4c76-8c50-4c6138ea12ab) |
| 1 | pass with mocks | 92 | 49 | 71.1 | 8 | 8 | [run](https://argusic.com/run/ba66ed13-3fe9-45fd-bb7c-c09300490b54) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `No Rust toolchain installed`
- 4 min: `just command not found`
- 5 min: `cargo-nextest not found (required for test runner)`
- 2 min: `Disk full during incremental compilation (40GB overlay)`
- 3 min: `CLI test app_server_rejects_invalid_code_mode_host_urls fails: http:// URLs are now valid (gRPC support)`
- 5 min: `CLI test features_list_honors_cloud_managed_feature_requirements fails: features list subcommand doesn't wire up cloud config bundle loader`
- 1 min: `CLI test sandbox_fetches_and_enforces_cloud_managed_permission_profile fails: requires bubblewrap (bwrap) not available`
- 3 min: `Release build fails: cc compile error for tree-sitter native crate`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
