# shirudo

**Verdict: runs.** Argusic Score 98.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shirudo-dev/shirudo, licensed BSD-2-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/shirudo

## Pinned environment

- Project commit: `8a3b249b4be8a0422150d07ea027d50b657ec368`
- Test commit: `8a3b249b4be8a0422150d07ea027d50b657ec368`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.3 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 12.6 | 9 | 9 | [run](https://argusic.com/run/09565b68-2bed-448c-86ce-184c37a08054) |
| 2 | pass | 97.5 | 25 | 11.3 | 8 | 7 | [run](https://argusic.com/run/08b64882-72d9-455c-80ab-894ac937bb5d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing all system build dependencies: libelf-dev, zlib1g-dev, libcurl4-openssl-dev, libluajit-5.1-dev, libzstd-dev, libtss2-dev, clang-18, llvm-18-dev, libomp-18-dev. No root access for apt-get install.`
- 15 min: `OpenSSL 3.0.13 (Ubuntu 24.04) does not satisfy >= 3.5 requirement. ML-DSA signing not available.`
- 1 min: `curl/curl.h not found - headers in multiarch directory (x86_64-linux-gnu/) not standard location`
- 1 min: `gen-vmlinux-h link error: libelf.a requires libzstd (undefined ZSTD_* symbols)`
- 2 min: `BPF compilation fails against host kernel (6.8.0) BTF - missing BPF_SIG_VERIFIED, signature_size, DCACHE_MOUNTED, mnt_t_flags, T_SHARED, BPF_SIG_KEYRING_BPF`
- 1 min: `lua.h, lualib.h not found - luajit headers in versioned subdirectory`
- 2 min: `Linker: static libcurl.a requires gssapi_krb5, nghttp2, brotli, ssh and many transitive deps`
- 1 min: `Linker: static libluajit-5.1.a requires -lm (pow, log, sin, cos etc.)`
- 2 min: `mlockall(MCL_CURRENT|MCL_FUTURE) fails: RLIMIT_MEMLOCK (8192) too low, no CAP_IPC_LOCK`

Attempt 2:

- 3 min: `Missing system dev packages: libelf-dev, zlib1g-dev, libluajit-5.1-dev, libtss2-dev, libcurl4-openssl-dev, libzstd-dev`
- 3 min: `Missing clang/LLVM 23 with BPF target (project requires it for BPF compilation)`
- 8 min: `Missing OpenSSL >= 3.5 with ML-DSA (system has 3.0.13)`
- 1 min: `Linking failure: libelf.a references ZSTD symbols (libzstd not linked)`
- 1 min: `Linking failure: LuaJIT static lib needs -lm`
- 2 min: `BPF compilation failed against host kernel BTF (struct mismatches)`
- 2 min: `Linking failure: libcurl.a conflicts with system OpenSSL`
- `shirudo binary refuses to run: mlockall fails (ulimit -l 8192, needs unlimited)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
