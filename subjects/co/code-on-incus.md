# code-on-incus

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mensfeld/code-on-incus, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/code-on-incus

## Pinned environment

- Project commit: `df175f0332666aa8984af9cefb1c5fc8b437736a`
- Test commit: `df175f0332666aa8984af9cefb1c5fc8b437736a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.5 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 12.6 | 4 | 4 | [run](https://argusic.com/run/897fafce-dd72-4c44-b56a-d58106a508e2) |
| 2 | pass | 100 | 12 | 7.5 | 3 | 3 | [run](https://argusic.com/run/2cb1d47b-adfe-4c86-b222-8e71c8b5bad7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `libsystemd-dev headers not installed (system package) on build host`
- 1 min: `nft binary not found - installer test TestInstallSh_NftAutoSetup_NonInteractive failed`
- 5 min: `incus binary not found - CLI integration tests requiring incus failed`
- 3 min: `4 CLI Python tests still fail - fundamentally require a running Incus daemon: test_shell_use_tmux_config.py tests, test_storage_pool_validation_* tests`

Attempt 2:

- 4 min: `Go toolchain not installed`
- 3 min: `libsystemd-dev headers not present`
- 3 min: `nft binary not found (used by installer test)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
