# ODS

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Osmantic/ODS, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ods

## Pinned environment

- Project commit: `6ff9b4fc5190099705043acaab7e9b6ad9c8b8f1`
- Test commit: `6ff9b4fc5190099705043acaab7e9b6ad9c8b8f1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 15.3 to 26.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 27 | 26.8 | 8 | 8 | [run](https://argusic.com/run/f084b9f4-83f9-446f-b5a0-3718fedab126) |
| 2 | pass with mocks | 92 | 5 | 26.4 | 5 | 5 | [run](https://argusic.com/run/1b253565-4e95-4a68-913b-e65f469bc6a1) |
| 3 | pass with mocks | 92 | 48 | 15.3 | 4 | 4 | [run](https://argusic.com/run/f7d8b975-0007-4e79-897e-894d1ccf3431) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `service-registry.sh unconditionally overrides EXTENSIONS_DIR, breaking tests that set it externally (test-hooks.sh)`
- 0.5 min: `test-preset-import-export.sh: grep -A15 misses 'cd PRESETS_DIR' which is 16 lines after the match, and had a stray quote`
- `Docker not installed (and cannot be installed - no root)`
- `disk-space-preflight.sh requires rsync (not installed, no root to install it)`
- `network-security.sh reports 18 warnings about potentially externally exposed services (expected for this Docker AI server project)`
- `test-restore-safety-ux.sh expects exit 0 on cancel but ods-restore.sh exits 1`
- `test-hooks.sh test 1/2 failure originally due to EXTENSIONS_DIR override (fixed above)`
- 1 min: `Python packages pyyaml, pytest, jsonschema, requests required by tests not installed`

Attempt 2:

- `Docker not available in container (needed for full stack install/launch)`
- `2 BATS tests fail: docker phase skips, port conflict detection (need Docker runtime)`
- `5 tests fail due to no running services: test-streaming, test-concurrency, test-dashboard-integration, test-disk-space-preflight, test-cli-update-verification`
- 5 min: `test-preset-compatibility: 1 fail (cmd_preset does not call validate_preset_compatibility)`
- 2 min: `test-setup_card.py, test_hf_download_helper.py, validate-agent-templates.py: missing pytest and requests modules`

Attempt 3:

- `Docker not available in container; full install requires Docker`
- 2 min: `ai_err function called in 07-devtools.sh:189 but does not exist; the UI library defines ai_bad instead`
- `disk-space-preflight test fails because rsync is not installed`
- `CPU-only-path test fails because resolve-compose-stack.sh needs Docker`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
