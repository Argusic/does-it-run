# rocketride-server

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rocketride-org/rocketride-server, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/rocketride-server

## Pinned environment

- Project commit: `37b5dd25af12d515b6852756febaac68d806b211`
- Test commit: `37b5dd25af12d515b6852756febaac68d806b211`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 22.3 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 22.3 | 5 | 5 | [run](https://argusic.com/run/df144289-f0d8-41fa-ba63-b538e16c3779) |
| 2 | fail | 50 | 25 | 27.3 | 3 | 3 | [run](https://argusic.com/run/9a3e2d88-81d6-4882-8c88-cf0183f8a0bf) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `LLVM/clang 18 tarball URL discovery via GitHub API hit rate limit , manually downloaded to ~/toolchains/llvm-18`
- 1 min: `pnpm install required but pnpm not in PATH , installed via npm with --prefix`
- 5 min: `server:build failed because system packages (zip, unzip, ninja-build, libc++1, etc.) require root`
- 3 min: `Engine finds local source paths and fails when run from inside the repo checkout`
- 1 min: `Engine's bundled depends.py needed uv binary in exec_dir/bin/uv`

Attempt 2:

- 15 min: `Missing system packages require root: autoconf, automake, libtool, ninja-build, uuid-dev, libffi-dev, libsqlite3-dev, libbz2-dev, libreadline-dev, libexpat1-dev, libncurses-dev, libgdbm-dev, libdb-dev, liblzma-dev, libxmlsec1-dev, zlib1g-de`
- `Node.js v18.19.1 is too old for UI apps (needs >=20), causing @rsbuild/core to crash`
- 3 min: `zip and unzip not found in container; downloaded static binaries from Debian packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
