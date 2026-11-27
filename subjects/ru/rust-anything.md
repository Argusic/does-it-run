# rust-anything

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erkamyaman/rust-anything, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/rust-anything

## Pinned environment

- Project commit: `a3f40af356abc13be3baf33bfe1ddf860440d1c1`
- Test commit: `a3f40af356abc13be3baf33bfe1ddf860440d1c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 9.7 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 41 | 13.8 | 2 | 2 | [run](https://argusic.com/run/7448318f-cfcb-4d87-93a8-558984832bb5) |
| 2 | pass | 100 | 21 | 9.7 | 4 | 4 | [run](https://argusic.com/run/80f5bcf3-77ef-47fb-95d8-8d13832b3cfa) |

## What was observed on a clean machine

Attempt 1:

- `Node.js 18.19.1 (container default) cannot run .ts files directly; rust-anything needs Node 22.6+ for TypeScript execution. This caused 19 test failures across unit and integration tests (1 unit: node_writes_profile_to_a_temp_path_with_spac`
- `Optional language runtimes missing (Go, Ruby, Java, Kotlin, PHP, .NET) , tests that depend on them were skipped automatically.`

Attempt 2:

- `Node.js v18.19.1 in container cannot run .ts files directly (needs 22.6+)`
- `String.isWellFormed() not available in Node 18 (needs 20+)`
- `--cpu-prof not allowed in NODE_OPTIONS on Node 18 (needs 24+)`
- `Go, Ruby, Java, Kotlin, PHP, .NET runtimes not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
