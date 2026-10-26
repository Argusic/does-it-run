# continuous-integration

**Verdict: runs with mocks.** Argusic Score 48 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bazelbuild/continuous-integration, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/continuous-integration

## Pinned environment

- Project commit: `080f19d6e3dc22dbfc710090e211abc1bd48f32d`
- Test commit: `080f19d6e3dc22dbfc710090e211abc1bd48f32d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.6 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 23.9 | 0 | 0 | [run](https://argusic.com/run/91c6e7ef-b8c4-4ba2-ad97-198a481600b6) |
| 2 | pass with mocks | 76 | 3 | 6.6 | 5 | 1 | [run](https://argusic.com/run/426ac973-5020-41ce-8f35-79279a8b2a36) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `aggregate_incompatible_flags_test_result_test.py calls get_pipeline_and_platform() which didn't exist; added the function but test data uses old platform labels (e.g. ':ubuntu: 18.04 (OpenJDK 11)') that don't match current emoji-name values`
- 1 min: `No Go compiler in container , agent/metrics/pipestats Go components cannot build`
- 1 min: `No Rust/cargo in container , agent/ Rust component cannot build`
- 1 min: `No Java/Maven in container , dashboard/server/ Java component cannot build`
- 1 min: `cherry_picker and update-lockfile actions require GH_TOKEN env var to import`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
