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
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 6.2 | 2 | 2 | [run](https://argusic.com/run/fda143ac-367f-4b9a-b6d5-a696423715cc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_openclaw_reverse_env_falls_back_without_patchable_config failed: OPENROUTER_API_KEY env var in container changed fallback provider detection`
- 3 min: `test_dsh_client_forward_proxy_captures_local_gateway failed: Node v18.19.1 does not support --use-env-proxy flag`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
