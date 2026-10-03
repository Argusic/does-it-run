# hermes-webui

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nesquena/hermes-webui, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hermes-webui

## Pinned environment

- Project commit: `ff26335b87610f70d74ff008608a321fb1281bd1`
- Test commit: `ff26335b87610f70d74ff008608a321fb1281bd1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.9 to 32.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 3 | 32.9 | 5 | 0 | [run](https://argusic.com/run/7deb98ea-170a-4463-94ae-b688b5fd5f7d) |

## What was observed on a clean machine

Attempt 1:

- `Test shard 0: test_smd_wrapper_runtime_matches_render_md_emphasis_policy fails because Node.js 18 treats smd.min.js (ES module with 'export' syntax) as CommonJS since package.json lacks "type": "module"`
- `Test shard 2: test_live_prose_rebuild_preserves_markdown_dom and test_live_prose_post_rewind_keeps_tail_word_identity fail from same Node.js ES module import issue`
- `Test shard 3: 3 test_real_smd_parser_* errors from same Node.js ES module import issue`
- `Test shard 1: test_lmstudio_has_key_true_via_config_yaml fails in sharded run due to test isolation ordering (passes individually)`
- `Test shard 2: test_openrouter_group_uses_live_fetch_when_available fails in sharded run due to test isolation ordering (passes individually)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
