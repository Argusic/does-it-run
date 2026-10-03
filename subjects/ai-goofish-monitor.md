# ai-goofish-monitor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Usagi-org/ai-goofish-monitor, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-goofish-monitor

## Pinned environment

- Project commit: `f85d140b6b45029d9a0925feb96dad733b41396d`
- Test commit: `f85d140b6b45029d9a0925feb96dad733b41396d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 7.4 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 14.3 | 4 | 4 | [run](https://argusic.com/run/3962fa11-d6d4-4de5-8af7-4679944d50f0) |
| 2 | pass with mocks | 92 | 5.2 | 9.1 | 3 | 3 | [run](https://argusic.com/run/9f5543c2-ae04-485a-ac97-6a5629abef8e) |
| 3 | pass with mocks | 92 | 4 | 7.4 | 4 | 4 | [run](https://argusic.com/run/2b4f5eac-0c94-41b7-9286-deb7c3ee4724) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install failed: externally-managed-environment`
- 2 min: `test_save_to_jsonl assertion failed: load_all_result_records returns decorated records with extra visibility fields (_status, _matched_blacklist_keywords, etc.)`
- 1 min: `test_frontend_build_output_path_is_consistent_across_configs failed: web-ui/dist in .dockerignore`
- 3 min: `npm run build failed: Node 18 too old for Vite 7 (requires 20.19+), crypto.hash is not a function`

Attempt 2:

- 2 min: `test_save_to_jsonl failed because load_all_result_records now decorates records with _status/_matched_blacklist_keywords/_hidden_reason/_effective_hidden fields`
- 1 min: `test_frontend_build_output_path_is_consistent_across_configs failed because .dockerignore contained 'web-ui/dist' which the test expects absent`
- `Frontend Vite build requires Node.js >= 20.19 but environment has 18.19.1`

Attempt 3:

- `test_save_to_jsonl strict equality failed because result_storage_service decorates records with metadata fields`
- `test_failure_guard_auto_recovers_on_cookie_change failed due to filesystem mtime race on tmpfs`
- `test_frontend_build_output_path_is_consistent_across_configs failed because .dockerignore contained web-ui/dist`
- `Frontend build failed: Node 18.19.1 is too old for Vite 7.x (requires Node 20.19+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
