# aide

**Verdict: could not verify.** Argusic Score 10 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/skyelan1999/aide, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/aide

## Pinned environment

- Project commit: `903de5aa948b4e5d812cb682d5ad6580834128d6`
- Test commit: `903de5aa948b4e5d812cb682d5ad6580834128d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.6 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 0 | 7.6 | 3 | 0 | [run](https://argusic.com/run/3e7ac12c-c2b9-4157-9d06-2886ce114e3b) |
| 2 | fail | 20 | 15 | 8.3 | 4 | 4 | [run](https://argusic.com/run/80ed4e67-b13a-444e-8be3-3b4f1233d4a7) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Docker is required but not installed (no root access to install)`
- 2 min: `Go toolchain is required but not installed (no root access to install)`
- `pdf-jpx-official.test.cjs requires external fixtures from GitLab and a C compiler for test-native.py`

Attempt 2:

- `Docker Engine and Docker Compose v2 are required but not installed in this container. The project depends on Docker for building and running the aide backend (Go service inside a container). Source install flow cannot proceed.`
- `test_launcher_contract: 'zip: command not found' - the 'zip' utility is required by scripts/package-release-assets.sh which is called by one of the launcher-contract tests.`
- `test_cad_step_curve_check: test_sha_guard_prevents_sdk_import_and_source_mutation fails because mocking builtins.__import__ on Python 3.12 triggers pathlib to import ntpath internally before reaching the SHA256 guard.`
- `desktop-capture.test.cjs: 'ReferenceError: File is not defined' - this test requires browser/desktop runtime APIs not available in Node.js CLI.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
