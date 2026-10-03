# Vibe-Skills

**Verdict: runs.** Argusic Score 93.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/foryourhealth111-pixel/Vibe-Skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vibe-skills

## Pinned environment

- Project commit: `ddcaa2affca93c1efe026d008b6b93709e5fb7e2`
- Test commit: `ddcaa2affca93c1efe026d008b6b93709e5fb7e2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 37.2 to 58.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 58.9 | 10 | 10 | [run](https://argusic.com/run/a38a2599-05e1-4fbe-b51f-cedf088420f7) |
| 2 | pass | 95 | 2.1 | 37.2 | 4 | 3 | [run](https://argusic.com/run/267b4baf-56a4-4640-861d-efdfaa9d57a2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pwsh not installed in container`
- 2 min: `docs/architecture/ directory missing (layout contract failure)`
- 5 min: `Many reference/docs files missing (quick-start, cold-start, browserops contracts, tool-registry, etc.)`
- 1 min: `SKILL.md line count 286 exceeds test threshold of 245`
- 2 min: `_is_bash_command() fails on Linux for Windows-style paths (D:\...\bash.exe)`
- 1 min: `docs/README.md is English-only, tests expected Chinese content`
- 1 min: `README benchmark section has different numeric values than tests assert`
- 1 min: `Star-history chart embeds removed from README but tests expected 3 URLs`
- 1 min: `Fixture .md files missing from git index (test uses git ls-files)`
- 1 min: `Installed-runtime policy test writes to /work/.pytest-tmp-installed-runtime (permission denied)`

Attempt 2:

- 15 min: `test_local_kernel_execution.py::test_run_local_kernel_rejects_symlinked_files_inside_a_legacy_run fails because real config has legacy_write_mode: disabled, bypassing symlink validation`
- 2 min: `test_vibe_skill_entry_contract.py::test_vibe_skill_entry_stays_sop_sized_and_avoids_overtriggering_language fails because SKILL.md has 286 lines but threshold was 245`
- 1 min: `test_repo_layout_contract.py::test_clean_architecture_roots_exist fails because docs/architecture is a file not directory`
- `3 PowerShell-dependent tests fail: pwsh not installed in container (tests/runtime_neutral/test_simple_powershell_installer_wrappers.py, test_check_installed_runtime_root.py, test_bash_test_support.py)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
