# no_human

**Verdict: runs.** Argusic Score 89.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/no-human-ai/no_human, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/no-human

## Pinned environment

- Project commit: `580a8793e6d0f02546d5e01581aa3e5ddcd31d9a`
- Test commit: `580a8793e6d0f02546d5e01581aa3e5ddcd31d9a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 60.3 to 71 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 1.2 | 71 | 3 | 1 | [run](https://argusic.com/run/4d453df9-8667-4778-83f6-0e7137ceeeb3) |
| 2 | pass with mocks | 92 | 13.5 | 60.3 | 4 | 4 | [run](https://argusic.com/run/4474e1aa-b14b-4331-b403-dd6d4115e742) |

## What was observed on a clean machine

Attempt 1:

- `bwrap (bubblewrap) not available - 7 tests in test_codex_sandbox_network.py fail because the container lacks non-privileged user namespaces`
- `gh CLI not installed - 1 test in test_review_fail_closed.py and 1 test in test_e2e_orchestrator.py fail because they shell out to 'gh' which is not present`

Attempt 2:

- 0.5 min: `'uv' not pre-installed in container`
- 1 min: `'gh' (GitHub CLI) binary not on PATH , needed by vcs/github.py::_existing_pr_url() which runs 'gh pr list' causing 'FileNotFoundError' in test_review_fail_closed.py`
- `7 tests fail in test_codex_sandbox_network.py , bwrap: No permissions to create a new namespace (kernel/user-namespace restriction in container)`
- `4 tests fail in test_base_tree_gate.py, 2 in test_flaky_rerun_attribution.py, 1 in test_handoff.py , pre-existing orchestrator logic issue: FakeBackend-driven tasks reach AWAITING_APPROVAL status when they should fail due to test breakage`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
