# cloudroom

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/davidondrej/cloudroom, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cloudroom

## Pinned environment

- Project commit: `63b335db40555ce3969d649afd5378e00f278f3e`
- Test commit: `63b335db40555ce3969d649afd5378e00f278f3e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 27.9 to 28.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 28.9 | 2 | 2 | [run](https://argusic.com/run/2fbcd85a-38e9-4054-9f0d-27225d88a525) |
| 2 | pass | 100 | 9 | 27.9 | 2 | 2 | [run](https://argusic.com/run/c8c385f7-487e-47fd-ab44-9daad3615e71) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `Two observability unit tests failed: private_stderr_rotation_counts_encoded_bytes_and_keeps_two_private_files and api_outage_keeps_local_diagnostics_and_overload_is_visible , both caused by Rust's fs::create_dir creating temp dirs with mode`
- 20 min: `runtime integration test harness_commits_drop_ai_co_authors_and_keep_human_ones failed , the Git config-based hook mechanism (hook.<name>.command/hook.<name>.event via GIT_CONFIG_COUNT env vars) is not supported by Git 2.43.0 on Ubuntu 24.0`

Attempt 2:

- 2 min: `observability test helper uses fs::create_dir which creates umask-sensitive directories (0775), failing write_stderr permission check`
- 4 min: `git 2.43 lacks config-based hooks support needed by strip_ai_co_authors_env (requires git 2.54+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
