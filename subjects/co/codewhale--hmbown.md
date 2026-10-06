# Codewhale

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Hmbown/Codewhale, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/79c046d6-143f-4bc9-8e51-ef46bd55ceb2

## Pinned environment

- Project commit: `9b2eeca894413b178f8df02b79eac9a4c89a40c7`
- Test commit: `9b2eeca894413b178f8df02b79eac9a4c89a40c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 16.8 to 41.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 45 | 41.6 | 2 | 2 | [run](https://argusic.com/run/79c046d6-143f-4bc9-8e51-ef46bd55ceb2) |
| 2 | pass with mocks | 92 | 11 | 16.8 | 3 | 3 | [run](https://argusic.com/run/adc8f1fd-eb7b-4791-bf9f-98577fc0d3ab) |
| 3 | pass with mocks | 92 | 25 | 26.1 | 3 | 3 | [run](https://argusic.com/run/dd49f836-de6e-4770-a83a-ff4d61d02ce9) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `libdbus-sys requires dbus-1.pc and C headers (system package libdbus-1-dev)`
- 5 min: `cargo build --release (LTO) killed by SIGKILL (OOM)`

Attempt 2:

- 2 min: `npm install -g failed with EACCES (no permission for /usr/local/lib/node_modules)`
- `npm test 1 failure: test 46 'full local release fixture' , tries to run prepare-local-release-assets.js which is not shipped in npm package (project-level release script)`

Attempt 3:

- 3 min: `Missing libdbus-1-dev package headers and .pc file`
- 2 min: `Missing libdbus-1.so symlink for linker`
- 5 min: `cargo build --release OOM-killed in constrained container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
