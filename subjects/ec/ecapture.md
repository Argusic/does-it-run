# ecapture

**Verdict: could not verify.** Argusic Score 65 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gojue/ecapture, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/ecapture

## Pinned environment

- Project commit: `08b25bab76fc478f83a7c1051d3c91cc8d0ac379`
- Test commit: `08b25bab76fc478f83a7c1051d3c91cc8d0ac379`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 20 to 26.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 17 | 20 | 4 | 4 | [run](https://argusic.com/run/389e1113-bfe5-47c9-b90a-2a48ed50434d) |
| 2 | fail | 80 | 26 | 26.2 | 6 | 6 | [run](https://argusic.com/run/d09dfc49-ebdd-48a2-aec0-af22fc305863) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go toolchain not installed`
- `clang/llc/bpftool missing , eBPF C compilation impossible`
- `flex/lex missing , libpcap static library cannot be built`
- `3 MySQL tests fail because /usr/sbin/mysqld doesn't exist on this host , pre-existing test fixture issue`

Attempt 2:

- 3 min: `Missing Go toolchain (go 1.26+ required)`
- 2 min: `Missing LLVM/Clang 9+ and llc (eBPF compilation)`
- 1 min: `Missing bpftool (eBPF BTF dump)`
- 3 min: `Missing libpcap build deps: flex, bison, m4, libsigsegv`
- 1 min: `bison m4 subprocess failed at runtime without BISON_PKGDATADIR and M4 env vars`
- `file command not found (make post-build check fails with exit 127)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
