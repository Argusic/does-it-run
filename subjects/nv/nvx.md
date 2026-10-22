# nvx

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/nvx, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/nvx

## Pinned environment

- Project commit: `5b37b4f159ad006e6b78278a27477fa93a7b4e80`
- Test commit: `5b37b4f159ad006e6b78278a27477fa93a7b4e80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 77.6 to 77.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 70 | 77.6 | 7 | 7 | [run](https://argusic.com/run/7d2aa450-b1ee-4a7c-acb0-9fa7191f6015) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `system pip blocked by PEP 668 externally-managed environment`
- 7 min: `cargo/rustc and cargo-nextest missing for OpenVMM unit tests`
- 8 min: `cargo xflowey restore-packages wanted root apt for git/libarchive-tools and bsdtar`
- 18 min: `container 40G disk filled during OpenVMM debug build (linker SIGBUS then ENOSPC)`
- 12 min: `lxutil unit tests failed on overlayfs: 1024-byte symlink target hits ENAMETOOLONG (max 1023), and rename inode assertion 17!=39`
- 15 min: `NVMe storage_tests panic index out of bounds len 64 when thread lands on host cpu 71/147/167 (container cpuset), sparse_mmap NUMA mbind EPERM via seccomp`
- `microVM guest boot cannot run: no /dev/kvm or /dev/mshv in container and this OpenVMM build has no emulated hypervisor backend`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
