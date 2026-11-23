# coi

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coipond/coi, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/coi

## Pinned environment

- Project commit: `a6781344bd1c316c34190ea44b9c0ed206633f35`
- Test commit: `a6781344bd1c316c34190ea44b9c0ed206633f35`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.9 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 7.9 | 6 | 6 | [run](https://argusic.com/run/62c86031-7f1a-478b-b97b-adec47c4dde5) |
| 2 | pass | 100 | 10 | 9.8 | 5 | 5 | [run](https://argusic.com/run/dfaadf10-c335-453b-9b37-1d10693f091a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go toolchain not installed in container`
- 0.5 min: `Missing go.sum entries (jsonschema and dns transitive deps)`
- 0.5 min: `Missing embedded/dummy and embedded/default_config.toml`
- 1 min: `systemd/sd-journal.h header not available (needed by go-systemd/sdjournal CGo)`
- 0.5 min: `pkg-config cannot find libsystemd (only systemd.pc exists)`
- 1.5 min: `nft not found, causing installer test failure`

Attempt 2:

- 2 min: `Go 1.27.4 needed (go.mod requires 1.26), not in PATH`
- 2 min: `cgo build failure: systemd/sd-journal.h not found (libsystemd-dev not installed)`
- 1 min: `make build needs embedded files: internal/image/embedded/dummy and internal/config/embedded/default_config.toml`
- 3 min: `TestInstallSh_NftAutoSetup_NonInteractive failed because nft not in PATH (pkg_install tried sudo apt-get)`
- `Python CLI tests fail because incus is not installed (13 failed due to incus: executable not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
