# fcp

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Svetlitski/fcp, licensed BSD-3-Clause, written in Rust.

Evidence and recordings: https://argusic.com/subject/fcp

## Pinned environment

- Project commit: `f8db0603ff0fb66d34d3c461b8e6239b72e1cad2`
- Test commit: `f8db0603ff0fb66d34d3c461b8e6239b72e1cad2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 8.1 | 1 | 1 | [run](https://argusic.com/run/a8fd322b-f355-41ba-bed7-d43b822d43e9) |
| 2 | pass | 100 | 0.4 | 7 | 2 | 2 | [run](https://argusic.com/run/ecb38d01-b2a5-4435-9c34-dbaf94b34f9c) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `missing 'expect' system package: tests/character_device.exp has shebang #!/usr/bin/expect -f, container lacks /usr/bin/expect (CI installs it via sudo apt-get install expect; no root here)`

Attempt 2:

- `character_device test requires 'expect' (Tcl expect utility) which is not installed`
- `2 tests (linux, large_files) are #[ignore] by default , large file fixtures would be expensive to hydrate`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
