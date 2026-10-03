# firezone

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/firezone/firezone, licensed Apache-2.0, written in Elixir.

Evidence and recordings: https://argusic.com/subject/firezone

## Pinned environment

- Project commit: `9d84ba2729b5f3f3d520e06ba8b46f5f0a46562f`
- Test commit: `9d84ba2729b5f3f3d520e06ba8b46f5f0a46562f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 20 to 20 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 20 | 6 | 6 | [run](https://argusic.com/run/234ec0a8-8ade-47c0-b882-065ea5276ff8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Rust workspace glib-sys v0.18.1 build failure: pkg-config could not find glib-2.0 system headers (missing libglib2.0-dev)`
- 3 min: `l4-tcp-dns-server and l4-udp-dns-server tests panic because 'dig' (dnsutils) is not installed in the container`
- 2 min: `firezone-headless-client token tests fail with EPERM writing to /etc/dev.firezone.client/token (not running as root)`
- 2 min: `known-dirs smoke test fails: dirs::cache_dir()/runtime_dir()/data_local_dir() return None in minimal container`
- 3 min: `firezone-relay eBPF build fails: bpf-linker requires LLVM development libraries (llvm-config not found)`
- 2 min: `Elixir web portal and Docker Compose environment cannot run: no erl/mix/docker binaries available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
