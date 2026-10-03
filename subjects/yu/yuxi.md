# Yuxi

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xerrors/Yuxi, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/yuxi

## Pinned environment

- Project commit: `bd07ab4ac4faa2e5452507580b1c841543bbec61`
- Test commit: `bd07ab4ac4faa2e5452507580b1c841543bbec61`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 19.6 to 39.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 34 | 39.8 | 3 | 3 | [run](https://argusic.com/run/d5cec6ed-66f9-45ad-8694-ca136c1c8911) |
| 2 | pass with mocks | 92 | 5.2 | 19.6 | 3 | 3 | [run](https://argusic.com/run/6870f275-dfcd-492d-a1bd-c94ab701b91d) |
| 3 | pass | 100 | 9.7 | 24.6 | 3 | 3 | [run](https://argusic.com/run/790acf85-d359-4a42-9344-1324de4f1474) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `ImportError: 'test.live_api_cleanup' import fails because 'test' resolves to Python stdlib module (a regular package) instead of the project's namespace package at 'backend/test/'.`
- 10 min: `ImportError: 'libxcb.so.1' not found , OpenCV ('cv2') requires X11 system libraries missing from the container.`
- 3 min: `2 test failures: 'test_kubernetes_storage_init_migrates_only_real_entries' and 'test_runtime_identity_migration_preserves_symlink_without_following_target' assert directory mode '0o755' but get '0o775' due to container umask '0002' instead`

Attempt 2:

- 0.3 min: `test/unit/test_live_api_cleanup.py imported test.live_api_cleanup as package but test/ had no __init__.py`
- 0.2 min: `test/unit/backends/test_sandbox_provisioner_config.py and test/unit/storage_migrations/test_v072_runtime_identity.py assert directory mode == 0o755 but umask 002 produces 0o775`
- 2 min: `Front-end build and test fail: Node.js 18.19.1 lacks node:util.styleText used by rolldown/vite`

Attempt 3:

- 1.5 min: `test_kubernetes_storage_init_migrates_only_real_entries: umask 0002 causes 0775 vs expected 0755 on tmp_path directory`
- 1.5 min: `test_runtime_identity_migration_preserves_symlink_without_following_target: same umask 0002 issue`
- 3 min: `Node.js 18.19.1 (system) missing styleText export from node:util; rolldown native binding not resolved`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
