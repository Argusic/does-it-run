# claude-tap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liaohch3/claude-tap, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-tap

## Pinned environment

- Project commit: `4cc867d2e9689a7e5ca8623c67cabcb3fb7a456f`
- Test commit: `4cc867d2e9689a7e5ca8623c67cabcb3fb7a456f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.2 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 6.2 | 2 | 2 | [run](https://argusic.com/run/fda143ac-367f-4b9a-b6d5-a696423715cc) |
| 2 | pass | 100 | 7 | 7.7 | 2 | 2 | [run](https://argusic.com/run/34f8765b-f7bc-4830-88bf-600e5059b707) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_openclaw_reverse_env_falls_back_without_patchable_config failed: OPENROUTER_API_KEY env var in container changed fallback provider detection`
- 3 min: `test_dsh_client_forward_proxy_captures_local_gateway failed: Node v18.19.1 does not support --use-env-proxy flag`

Attempt 2:

- 1 min: `test_openclaw_reverse_env_falls_back_without_patchable_config failed because OPENROUTER_API_KEY env var caused wrong provider detection`
- 1 min: `test_dsh_client_forward_proxy_captures_local_gateway failed because Node lacks --use-env-proxy support`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
