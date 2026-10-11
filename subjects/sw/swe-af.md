# SWE-AF

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Agent-Field/SWE-AF, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/swe-af

## Pinned environment

- Project commit: `17d3160f20a2e2bd58810fb03a7f674c2a279415`
- Test commit: `17d3160f20a2e2bd58810fb03a7f674c2a279415`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 14.5 to 25.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 25.1 | 0 | 0 | [run](https://argusic.com/run/16de40a7-6e16-4580-87c1-9850edb8e7ec) |
| 2 | pass with mocks | 92 | 0.28 | 14.5 | 4 | 4 | [run](https://argusic.com/run/8e898b48-3082-47de-aa0e-91c0eb4ad34a) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `test_ac_3_fastbuildconfig_defaults failed because OPENROUTER_API_KEY in container env changed default runtime from claude_code to open_code`
- 1.5 min: `test_default_runtime_and_provider, test_empty_env_uses_claude_code, test_unset_env_uses_claude_code, test_default_resolution failed from same env-var interference`
- 0.5 min: `test_build_config_no_args (multi_repo_schemas) same env interference`
- 0.5 min: `test_ac_25 (multi_repo_integration) same env interference in child subprocess`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
