# Patter

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PatterAI/Patter, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/patter

## Pinned environment

- Project commit: `f01875136816c953151a0e61dcf3a0057027b2b4`
- Test commit: `f01875136816c953151a0e61dcf3a0057027b2b4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 17.5 to 41.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 5 | 17.5 | 3 | 3 | [run](https://argusic.com/run/743b0e19-56d1-45bf-829f-fbc246895c5c) |
| 2 | pass with mocks | 92 | 5 | 41.3 | 3 | 3 | [run](https://argusic.com/run/ed1a1270-463f-48b0-b7bd-3b51d49d5841) |

## What was observed on a clean machine

Attempt 1:

- `1 pre-existing test failed: test_find_call_dir_latest_and_by_id is flaky (equal mtime when files created in rapid succession , _find_call_dir uses max() which returns first with ties).`
- 3 min: `Python 3.12 makes ::ffff:* IPv6 addresses is_reserved=True, breaking is_internal_ip() for legitimate public IPv4-mapped addresses.`
- 3 min: `TypeScript vitest requires vite>=5 but npm resolved vite 7.x which needs node>=20; currently on node v18.19.1`

Attempt 2:

- 10 min: `SSRF is_internal_ip() incorrectly blocks IPv4-mapped public addresses like ::ffff:8.8.8.8 due to is_reserved on the IPv6 wrapper range`
- 2 min: `Python test_hermes_cli function _find_call_dir mtime tiebreaker fails when two dirs share the same filesystem timestamp`
- 8 min: `TypeScript tests fail with ERR_REQUIRE_ESM on Node 18 because vitest@3 bundles vite@7 requiring ESM`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
