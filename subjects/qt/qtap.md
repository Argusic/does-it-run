# qtap

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qpoint-io/qtap, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/qtap

## Pinned environment

- Project commit: `6d7dfa743c9a1ad4423ca2cc93bdfee9b5b0323e`
- Test commit: `6d7dfa743c9a1ad4423ca2cc93bdfee9b5b0323e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 5.6 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 13.7 | 4 | 4 | [run](https://argusic.com/run/612642e9-1cb5-4e88-8901-b626e9d47fdb) |
| 2 | pass with mocks | 92 | 2.3 | 5.6 | 3 | 3 | [run](https://argusic.com/run/f213205e-447f-48aa-b00b-0c58a18d7e49) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.27.1 not pre-installed; had to download tarball`
- 1 min: `clang not installed (required for eBPF code generation)`
- 1 min: `JVM embedded dist/ files missing (5 files for go:embed)`
- 1 min: `IPv6 disabled in container - 4 egress tests fail with 'bind: cannot assign requested address' for tcp6`

Attempt 2:

- 5 min: `IPv6 disabled on loopback in container causes 4 tests to fail in pkg/egress (bind tcp6 [::1] fails)`
- 1.5 min: `Go 1.27.4 not installed in container; downloaded and installed manually`
- 0.5 min: `Embedded binary assets (JARs, JRE, .so) missing for //go:embed directives in javassl/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
