# coi

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coipond/coi, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/coi

## Pinned environment

- Project commit: `a6781344bd1c316c34190ea44b9c0ed206633f35`
- Test commit: `a6781344bd1c316c34190ea44b9c0ed206633f35`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 7.9 | 6 | 6 | [run](https://argusic.com/run/62c86031-7f1a-478b-b97b-adec47c4dde5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go toolchain not installed in container`
- 0.5 min: `Missing go.sum entries (jsonschema and dns transitive deps)`
- 0.5 min: `Missing embedded/dummy and embedded/default_config.toml`
- 1 min: `systemd/sd-journal.h header not available (needed by go-systemd/sdjournal CGo)`
- 0.5 min: `pkg-config cannot find libsystemd (only systemd.pc exists)`
- 1.5 min: `nft not found, causing installer test failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
