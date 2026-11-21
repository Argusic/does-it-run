# gotatun

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mullvad/gotatun, licensed MPL-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/gotatun

## Pinned environment

- Project commit: `2a867b3f322d95dc08043498d34eb91fb4266590`
- Test commit: `2a867b3f322d95dc08043498d34eb91fb4266590`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6.8 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 7 | 4 | 4 | [run](https://argusic.com/run/294190d3-dc4a-4668-987e-9eba3ce837e7) |
| 2 | pass | 100 | 6 | 6.8 | 4 | 4 | [run](https://argusic.com/run/1f89a7a2-bf7b-4286-9887-50f41030b453) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `README cargo install --bin gotatun --path . fails: 'found a virtual manifest ... instead of a package manifest' (root Cargo.toml is a workspace)`
- 3 min: `cargo test --lib: 4 IPv6-bound UDP socket tests fail with 'Cannot assign requested address' (os error 99)`
- 1 min: `gotatun -f gotest fails 'NULL from getlogin' (drop_privileges, no controlling tty in container)`
- 2 min: `Default run and real tunnel bring-up cannot be completed: /dev/net/tun absent, mknod not permitted, no CAP_NET_ADMIN`

Attempt 2:

- 1 min: `Rust toolchain not installed`
- `4 unit tests fail with 'Cannot assign requested address' on IPv6 LOCALHOST bind`
- `Integration tests require sudo and docker`
- `Binary cannot start tunnel: no TUN device available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
