# miniserve

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/svenstaro/miniserve, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/miniserve

## Pinned environment

- Project commit: `64f3c35c18cdb78c8faf9981091a650df421512d`
- Test commit: `64f3c35c18cdb78c8faf9981091a650df421512d`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 32.7 to 76.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 32.5 | 32.7 | 6 | 6 | [run](https://argusic.com/run/66886562-bbdc-45f2-8073-f22963e2a9aa) |
| 2 | pass | 100 | 15 | 76.3 | 1 | 1 | [run](https://argusic.com/run/8dea49ea-c420-4fda-af69-eb28860a5351) |
| 3 | pass | 100 | 72 | 66.8 | 2 | 2 | [run](https://argusic.com/run/c4011be7-107e-4adf-b521-8b4bd42ca761) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `C compiler (cc/gcc) not found in container - needed to build Rust crates with C dependencies (ring, etc.)`
- 0.5 min: `Zig was invoked without the 'cc' subcommand when used as linker (cargo config called zig directly)`
- 1 min: `Zig cc rejects '--target=x86_64-unknown-linux-gnu' (Rust triple format) - expects LLVM format 'x86_64-linux-gnu'`
- 5 min: `Tar archive creation fails with FilesystemLoop (ELOOP) on self-referencing broken symlink; test expects tar to contain subset of files`
- 2 min: `Zip archive creation fails with FilesystemLoop on broken symlink due to std::fs::metadata following symlinks`
- 1 min: `Test expectations for broken-symlink archive sizes incorrect after fixes (tar_gz now creates full archive, not just 10 bytes; zip now creates non-empty archive)`

Attempt 2:

- 8 min: `Broken symlink in test fixture (self-referencing symlink) causes ELOOP when tar builder tries to follow_symlinks(true)`

Attempt 3:

- 7 min: `archive_behave_differently_with_broken_symlinks (case tar) failed: tar 0.4.46 with follow_symlinks(true) hits ELOOP on a self-referential broken symlink, aborting the whole archive (1536-byte partial tarball vs expected 2048+)`
- 2 min: `3 bind_ipv4_ipv6 tests fail in container: no IPv6 localhost routing (timeout on ::1 reachability)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
