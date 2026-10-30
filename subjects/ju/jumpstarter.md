# jumpstarter

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jumpstarter-dev/jumpstarter, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/jumpstarter

## Pinned environment

- Project commit: `e84abc2dc59f6f517aee70a89567c0aa51c1a8cf`
- Test commit: `e84abc2dc59f6f517aee70a89567c0aa51c1a8cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 74.2 to 74.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 80 | 74.2 | 8 | 6 | [run](https://argusic.com/run/208d4db5-1911-43e6-9d92-e41cdd81d245) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `jumpstarter-cli-common oidc.py imports certifi and requests but pyproject.toml did not declare them; isolated pytest collection failed with ModuleNotFoundError`
- 3 min: `jumpstarter-driver-energenie driver.py imports requests but pyproject.toml did not declare it; isolated pytest collection failed with ModuleNotFoundError`
- 15 min: `jumpstarter-driver-dut-network has_passwordless_sudo() raised FileNotFoundError because sudo is not installed; test collection crashed`
- 30 min: `jumpstarter common _run_process passed pytest's DontReadFromInput (fileno raises UnsupportedOperation) to Popen; /bin/sh and /usr/bin/true exited 126 under capture`
- 25 min: `jumpstarter-driver-tmt pytest config log_cli=true broke click CliRunner capture; 4 CLI tests raised ValueError I/O operation on closed file`
- `jumpstarter-driver-qemu test_driver_qemu failed: [Errno 2] No such file or directory: 'qemu-img' (qemu-img binary not present and cannot be installed without root)`
- `jumpstarter-driver-uboot test_driver_uboot_console failed: [Errno 2] No such file or directory: 'qemu-system-aarch64' (qemu-system binary not present)`
- 5 min: `uv, go, rustc/cargo were not preinstalled; uv pip install is blocked by PEP 668`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
